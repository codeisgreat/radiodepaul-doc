# Hosts

## Host Fields

| field         | type    | description                    |
| ------------- | ------  | ------------------------------ |
| id            | integer | Primary id of a host           |
| name          | string  | host name                      |
| hometown      | string  | host hometown                  |
| major         | string  | host major                     |
| bio           | string  | host bio                       |
| nickname      | string  | host nickname                  |
| class_year    | string  | host class year                |
| email         | string  | host email address             |
| facebook      | string  | host facebook username         |
| twitter       | string  | host twitter username          |
| linkedin      | string  | host linkedin username         |
| website       | string  | host website url               |
| shows         | array   | host shows                     |
| person_url    | string  | host url                       |
| photo_thumb   | string  | url for 50px,50px host image   |
| photo_small   | string  | url for 150px,150px host image |
| photo_medium  | string  | url for 300px,300px host image |
| photo_large   | string  | url for 600px,600px host image |


## List Hosts

```bash
GET /people/getList.js
```

### Response

```bash
Status: 200 OK
```

```json
[{
  "photo_large":  "https://radiodepaul.s3.amazonaws.com/uploads/person/avatar/147/square_large_b4cbdd46-81aa-4d4f-b67e-b4bfc6ed5047.jpg",
  "photo_medium": "https://radiodepaul.s3.amazonaws.com/uploads/person/avatar/147/square_medium_b4cbdd46-81aa-4d4f-b67e-b4bfc6ed5047.jpg",
  "photo_small":  "https://radiodepaul.s3.amazonaws.com/uploads/person/avatar/147/square_small_b4cbdd46-81aa-4d4f-b67e-b4bfc6ed5047.jpg",
  "hometown":     "Nashville, TN",
  "major":        "Management",
  "influences":   "",
  "bio":          "",
  "shows": [
    {
      "show_photo_thumb": "https://radiodepaul.s3.amazonaws.com/uploads/show/avatar/87/square_thumb_524784ec-2086-491d-8d1c-256f658f9bca.jpg",
      "show_id":          "87",
      "show_title":       "Music City Mondays"
    }
  ],
  "nickname":    "",
  "name":        "Aaron Spalding",
  "id":          147,
  "class_year":  "Freshmen",
  "email":       "a.spalding93@yahoo.com",
  "facebook":    "aaron.spalding1",
  "twitter":     "",
  "linkedin":    "",
  "website":     "",
  "person_url":  "http://radio.depaul.edu/person?id=147",
  "photo_thumb": "https://radiodepaul.s3.amazonaws.com/uploads/person/avatar/147/square_thumb_b4cbdd46-81aa-4d4f-b67e-b4bfc6ed5047.jpg"
}]
```

## Get a Host

```bash
GET /people/getList.js?id=[id]
```

### Response

```bash
Status: 200 OK

# Response is the singular version of above
```
