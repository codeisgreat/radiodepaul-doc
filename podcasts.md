# Podcasts

## Postcast Fields
| field        | type    | description           |
| ------------ | ------- | --------------------- |
| id           | integer | primary id of podcast |
| title        | string  | podcast title         |
| type         | string  | podcast type          |
| description  | string  | podcast description   |
| contributors | string  | podcast contributors  |
| file_url     | string  | media url             |


## List Podcasts

```bash
GET /getPodcasts.js
```

### Response

```bash
Status: 200 OK
```

```json
[{
  "id":           3
  "file_url":     "https://radiodepaul.s3.amazonaws.com/uploads/podcast/file/3/32fc4f9a-a0e6-44f2-bae1-39fd6d6b968b.mp3",
  "contributors": "Various Staff Members // This is the file that we submitted for the 2012 IBS Best Streaming Station Award.",
  "description": "This is the file that we submitted for the 2012 IBS Best Streaming Station Award.",
  "title":       "2011-2012 Station Showcase",
  "type":        "station",
}]
```
