# Get accounts list

### Example request

`https://api.hackvita.eu/v2/generators/getAccountsList?api_key=APIKEY`

### Corresponding site section

`https://hackvita.eu/dashboard?section=AccountsList`

### Successful response

```json
{
  "ok": true,
  "values": [
    {
      "generator_id": 1,
      "generator_name": "Netflix",
      "generator_link": "https://netflix.com/",
      "generator_is_private": false,
      "generator_time_limit": 3600,
      "generator_count": 9999,
      "generator_is_starred": false
    },
    "..."
  ]
}
```

### Some informations

* **generator_time_limit** is the time limit imposed by the specific generator. For example, if it is 3600, you can make a generation every 3600 seconds (1 hour)

### Possible errors

* INVALID_API_KEY
* USER_IS_BANNED
* PERMISSION_DENIED
* INTERNAL_ERROR