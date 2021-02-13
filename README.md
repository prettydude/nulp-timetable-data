# nulp-timetable-data
Timetable data for NULP in JSON format
All data files are stored on `data` branch and updated every day on 3AM
Available at https://raw.githubusercontent.com/prettydude/nulp-timetable-data/data/

# Structure
### `institutes.json`
Sorted JSON array with valid institutes

### `groups.json`
Sorted JSON array with all valid groups in university

### `timetables/GROUP_NAME.json`
JSON array with lessons

## Lesson
Example structure of a lesson:
``` json
{
    "subject": "Програмування веб-кравлерів",
    "lecturer": "Пупкін В.І., ",
    "location": "213 V н.к.,  Практична",
    "url": "https://us02web.zoom.us/j/******",
    "type": "practical",
    "isFirstWeek": true,
    "isSecondWeek": true,
    "isFirstSubgroup": true,
    "isSecondSubgroup": true,
    "day": 1,
    "number": 1
}
```

`subject` - subject name

`lecturer` - lecturer name and initials

`location` - location and type of a lesson

`url` - URL for distance learning

`type` - extracted type of a lesson

`isFirstWeek` - whether this lesson is on odd numbered weeks (чисельник)

`isSecondWeek` - whether this lesson is on even numbered weeks (знаменник)

`isFirstSubgroup` - whether the first subgroup has this class

`isSecondSubgroup` - whether the second subgroup has this class

`day` - numeric day, 1 - Monday, 2 - Tuesday, etc.

`number` - lesson position in a day (counting from 1)
