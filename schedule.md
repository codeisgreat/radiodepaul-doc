# Schedule

# Slot Fields
| field      | type     | description             |
| ---------- | -------- | ----------------------- |
| show       | show     | slot show               |
| start_time | datetime | start time of broadcast |
| end_time   | datetime | end time of broadcast   |
| days       | array    | days broadcasting       |
| quarter    | string   | slot quarter            |

# List Schedule Slots

```bash
GET /getSchedule.js
```

### Response

```bash
Status: 200 OK
```

```json
[{
  "show": *see show resource documentation*,
  "end_time_date":   "2000-01-01T02:00:00-06:00",
  "start_time_date": "2000-01-01T00:00:00-06:00",
  "end_time":        "02:00AM CST",
  "start_time":      "12:00AM CST",
  "days": [
    "thursday"
  ],
  "quarter": "SQ2013"
}]
```
