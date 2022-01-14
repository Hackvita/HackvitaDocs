# Get single generator informations

### Example request

`https://api.hackvita.eu/v2/generators/getGeneratorInformations?api_key={api_key}&generator_id={generator_id}`

### Corresponding site section

`https://hackvita.eu/dashboard?section=AccountsList`

### Successful response

```json
{
  "ok": true,
  "values": {
    "generator_id": 155,
    "generator_name": "Ableton",
    "generator_link": "https://www.ableton.com",
    "generator_is_private": false,
    "generator_time_limit": 0,
    "generator_count": 43
  }
}
```

### Some informations

* **generator_time_limit** is the time limit imposed by the specific generator. For example, if it is 3600, you can make a generation every 3600 seconds (1 hour)

### Possible errors

* INVALID_API_KEY
* INVALID_GENERATOR_ID
* USER_IS_BANNED
* PERMISSION_DENIED
* INTERNAL_ERROR