# Shows

## Show Fields

| field             | type    | description                    |
| ----------------- | ------- | ------------------------------ |
| id                | integer | Primary id of a show           |
| genres            | string  | comma separated genres         |
| hosts             | array   | array of hosts                 |
| scheduled_slots   | array   | array of scheduled slots       |
| short_description | string  | show description               |
| long_description  | string  | long description               |
| facebook          | string  | facebook page username         |
| twitter           | string  | twitter username               |
| email             | string  | email address                  |
| website           | string  | website url                    |
| show_url          | string  | url for show                   |
| podcasts          | array   | array of podcasts              |
| photo_thumb       | string  | url for 50px,50px show image   |
| photo_small       | string  | url for 150px,150px show image |
| photo_medium      | string  | url for 300px,300px show image |
| photo_large       | string  | url for 600px,600px show image |

## List Shows

```bash
GET /shows/getList.js
```

### Response
```bash
Status: 200 OK
```

```json
[{
  "id":     40,
  "title":  "1Heart1Love1Soul",
  "genres": "R&b, Soul",
  "hosts": [{
    "id":        10,
    "name": "    James Hopkins",
    "nickname": "BrothaBinary",
    "shows": [{
      "show_title":       "1Heart1Love1Soul",
      "show_id": "        40",
      "show_photo_thumb": "https://radiodepaul.s3.amazonaws.com/uploads/show/avatar/40/square_thumb_0b624195-3152-45ac-b081-b2748c54c3df.jpg"
    }],
    "bio": "James Hopkins is a 31 year old Chicago college student, DJ, father, and tech enthusiast. He is BrothaBinary. The brand of BrothaBinary is many things. First, I’m a God fearing man. I make sure that He leads me in everything I do. Second, my motivation in everything that I do is for my 2 boys (ages 8 and 4). Yes, I’m a geek (respect my geekdum!... lol), nerd, dork, and in some people’s eyes, a lame because I LOVE TECHNOLOGY! Guess what… so be it. Technology is my passion and it’s the reason it’s my career.",
    "influences":   "God and the women that raised me.",
    "major":        "Information Systems",
    "hometown":     "",
    "class_year":   "Junior",
    "email":        "brothabinary@gmail.com",
    "facebook":     "",
    "twitter":      "1HeartLoveSoul",
    "linkedin":     "",
    "website":      "brothabinary.com",
    "person_url":   "http://radio.depaul.edu/person?id=10",
    "photo_thumb":  "https://radiodepaul.s3.amazonaws.com/uploads/person/avatar/10/square_thumb_2ed41496-aabb-4c67-b41b-99f68046e551.jpg",
    "photo_small":  "https://radiodepaul.s3.amazonaws.com/uploads/person/avatar/10/square_small_2ed41496-aabb-4c67-b41b-99f68046e551.jpg",
    "photo_medium": "https://radiodepaul.s3.amazonaws.com/uploads/person/avatar/10/square_medium_2ed41496-aabb-4c67-b41b-99f68046e551.jpg",
    "photo_large":  "https://radiodepaul.s3.amazonaws.com/uploads/person/avatar/10/square_large_2ed41496-aabb-4c67-b41b-99f68046e551.jpg"
  },{
    "id":       87,
    "name":     "Sierra Candi'a",
    "nickname": "",
    "shows": [{
      "show_title":       "1Heart1Love1Soul",
      "show_id":          "40",
      "show_photo_thumb": "https://radiodepaul.s3.amazonaws.com/uploads/show/avatar/40/square_thumb_0b624195-3152-45ac-b081-b2748c54c3df.jpg"
    }],
    "bio":        "",
    "influences": "",
    "major":      "",
    "hometown":   "",
    "class_year": "",
    "email":      "",
    "facebook":   "",
    "twitter":    "",
    "linkedin":   "",
    "website":    "",
    "person_url":   "http://radio.depaul.edu/person?id=87",
    "photo_thumb":  "https://radiodepaul.s3.amazonaws.com/uploads/person/avatar/87/square_thumb_dec75388-7508-452f-a5fc-b1420ffa3973.jpg",
    "photo_small":  "https://radiodepaul.s3.amazonaws.com/uploads/person/avatar/87/square_small_dec75388-7508-452f-a5fc-b1420ffa3973.jpg",
    "photo_medium": "https://radiodepaul.s3.amazonaws.com/uploads/person/avatar/87/square_medium_dec75388-7508-452f-a5fc-b1420ffa3973.jpg",
    "photo_large":  "https://radiodepaul.s3.amazonaws.com/uploads/person/avatar/87/square_large_dec75388-7508-452f-a5fc-b1420ffa3973.jpg"
  }],
  "scheduled_slots": [{
    "slot": "Thursdays 06:00PM CST - 08:00PM CST"
  }],
  "short_description": "The best in R&B and Soul!",
  "long_description":  "1Heart1Love1Soul has evolved over the years. Since September of 2009 we have always focused on bringing you great music. Today we are still music enthusiasts. We comb through local, national and international R&B to expose new and little known artists to the world. As the one and only ALL R&B SHOW for Radio DePaul we are back and stronger than ever. We believe our blend of new and old R&B/Soul and popular theme shows, also show the generational gaps are not quite so wide. ",
  "facebook": "http://www.facebook.com/pages/Welcome-to-1Heart1Love1Soul/193442069220?fref=ts",
  "twitter":  "1HeartLoveSoul",
  "email":    "1Heart1Love1Soul@gmail.com",
  "website":  "brothabinary.com",
  "show_url": "http://radio.depaul.edu/show?id=40",
  "podcasts": [],
  "photo_thumb":  "https://radiodepaul.s3.amazonaws.com/uploads/show/avatar/40/square_thumb_0b624195-3152-45ac-b081-b2748c54c3df.jpg",
  "photo_small":  "https://radiodepaul.s3.amazonaws.com/uploads/show/avatar/40/square_small_0b624195-3152-45ac-b081-b2748c54c3df.jpg",
  "photo_medium": "https://radiodepaul.s3.amazonaws.com/uploads/show/avatar/40/square_medium_0b624195-3152-45ac-b081-b2748c54c3df.jpg",
  "photo_large":  "https://radiodepaul.s3.amazonaws.com/uploads/show/avatar/40/square_large_0b624195-3152-45ac-b081-b2748c54c3df.jpg"
}]
```

## Get a Show

```bash
GET /shows/getShow.js?id=[id]
```

### Response

```bash
Status: 200 OK

# Response is the singular version of above
```

## List Random Shows

```bash
GET /shows/getRandom.js
```

### Response

```bash
Status: 200 OK

# Response is the same version of above
```
