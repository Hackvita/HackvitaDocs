# Get generation logs

### Example request

`https://api.hackvita.eu/v2/generators/getGenerationLogs?api_key={api_key}`

### Corresponding site section

`https://hackvita.eu/dashboard?section=GenLogs`

### Successful response

```json
{
  "ok": true,
  "values": [
    {
      "log_id": 6,
      "log_date": "2021-06-29",
      "log_alt": "HackStream@phoenix.com:hackflix2021",
      "log_is_private": false,
      "log_type": "HackFlix"
    },
    "..."
  ]
}
```

### Possible errors

* INVALID_API_KEY
* USER_IS_BANNED
* PERMISSION_DENIED
* INTERNAL_ERROR