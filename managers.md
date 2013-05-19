# Managers

## Manager Fields

| field          | type    | description                       |
| -------------- | ------- | --------------------------------- |
| id             | integer | primary id of a manager           |
| name           | string  | manager name                      |
| position       | string  | manager position                  |
| office_hours   | string  | manager office hours              |
| email          | string  | manager email address             |
| phone          | string  | manager phone number              |
| facebook       | string  | facebook username                 |
| twitter        | string  | twitter username                  |
| website        | string  | manager website url               |
| linkedin       | string  | manager linkedin username         |
| photo          | string  | url for 300px,300px manager image |

## List Managers

```bash
GET /people/getManagers.js
```

### Response

```bash
Status: 200 OK
```

```json
[{
  "photo":        "https://radiodepaul.s3.amazonaws.com/uploads/person/avatar/16/square_medium_e76616a3-db75-40fe-a5c2-bc3e5379e1fb.jpg",
  "website":      null,
  "linkedin":     null,
  "id":           16,
  "name":         "Zenaya Williams",
  "position":     "Podcast Programmer",
  "office_hours": null,
  "email":        "radiodepaulpd3@gmail.com",
  "phone":        "Email Only",
  "facebook":     "zenaya.williams.cain",
  "twitter":      "ZayDoll5"
}]
```
