# Recurrence Parsing

This library takes in schedules in json format with recurrent plannings and converts these into timelines compatible with the supertimeline project.

## Example schedule

```
[
    {
        "type": "group",
        "days": [0,1,2,3,4,5,6],
        "weeks": [0, 52, 14],
        "dates": [
            ["2017-1-1", "2017-1-31"],
            ["2017-12-1", "2017-12-31"]
        ],
        "times": [
            "10:00:00",
            "22:00:00"
        ],
        "children": [
            {
                "type": "folder",
                "days": [0],
                "path": "path"
            },
            {
                "type": "file",
                "path": "path"
            }
        ]
    }
]
```
