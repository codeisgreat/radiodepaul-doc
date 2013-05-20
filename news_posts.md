# News Posts

# News Post Fields

| field        | type    | description              |
| ------------ | ------- | ------------------------ |
| id           | integer | primary post identifier  |
| headline     | string  | post headline            |
| snippet      | string  | short post teaser        |
| content      | string  | post content             |
| author       | user    | post author              |
| published_at | string  | formatted published date |

## List News Posts

```bash
GET /news_posts/getList.js
```

### Response

```bash
Status: 200 OK
```

```json
[{
  "published_at": "March 4th, 2013",
  "author": {
    "name": "Scott Vyverman"
  },
  "content":  "<p>Radio DePaul took home 3 grand prize trophies from the Intercollegiate Broadcasting System national conference in NYC on Saturday March 2, 2013.  We were named the Best Online College Station for the second straight year.  Taylor Tingle won the best talk show grand prize for her interview with DePaul Professor and author Paul Booth on &ldquo;The DePaul Authors' Series&rdquo; and Jessica Schell, Natalie Vanderlaan, and Clay Guse won the grand prize for best spot news for their work on election night.  Congrats to all of our finalists and winner!</p>\n",
  "snippet":  "<p>Radio DePaul took home 3 grand prize trophies from the Intercollegiate Broadcasting System national conference in NYC on Saturday March 2, 2013. We were named the Best Online College Station...",
  "headline": "Radio DePaul is a Winner!",
  "id": 1
}]
```

# Get a News Post

```bash
GET /news_posts/getList.js?id=[id]
```

### Response

```bash
Status: 200 OK
```

```bash
Status: 200 OK

# Response is the singular version of above
```
