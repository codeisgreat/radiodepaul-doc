# Events

## Event Fields

| field       | type     | description                  |
| ----------- | -------- | ---------------------------- |
| id          | integer  | primary identifier for event |
| title       | string   | event title                  |
| first_line  | string   | string for first line        |
| second_line | string   | string for second line       |
| description | string   | event description            |
| created_at  | datetime | event creation date          |
| update_at   | datetime | event updated date           |

## List Events

```bash
GET /events/getList.js
```

### Response

```bash
Status: 200 OK
```

```json
{
  "id":          11,
  "updated_at":  "2013-05-08T12:43:33-05:00",
  "title":       "DemonTHON Live Broadcasts!",
  "second_line": "Beginning this Friday at 5 PM",
  "location":    "We will be broadcasting live and giving away free station chotzkies!",
  "first_line":  "24 Hours of Fun",
  "description": "The mission of DemonTHON is to build a year-long fundraising effort that culminates in a 24-hour Dance Marathon to honor the patients and families treated at Ann & Robert H. Lurie Children’s Hospital of Chicago and to celebrate the efforts of the DePaul University students that work to support these patients and families.  DemonTHON was named Best New Dance Marathon of 2012 as well as breaking the first year record!\r\n\r\n",
  "created_at":  "2013-02-18T13:27:07-06:00"
}
```
