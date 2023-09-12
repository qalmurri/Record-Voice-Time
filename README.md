# Record-Voice-Time
When the bot is run, it will create a JSON file automatically. how it works is quite easy, see below
### If the JSON file has been created, and trigger join voice channel. JSON will change as below
```
{
    "join": {
        "573453482707770000": 1,
        "662714356810900000": 0
    },
    "total": {
        "573453482707770000": {
            "total_time": 54.972437143325806,
            "start_time": 1694533413.181148
        },
        "662714356810900000": {
            "total_time": 8.079585790634155
        }
    }
}
```
### When all members are not in the voice channel, the JSON will be like below
```
{
    "join": {
        "573453482707770000": 0,
        "662714356810900000": 0
    },
    "total": {
        "573453482707770000": {
            "total_time": 78.912337143325806
        },
        "662714356810900000": {
            "total_time": 8.079585790634155
        }
    }
}
```
If you are on a voice channel, the join in JSON will change to 1. If not, it will change to 0.
