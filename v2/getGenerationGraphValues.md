# Get generation graph values

### Example request

`https://api.hackvita.eu/v2/generators/getGenerationGraphValues?api_key={api_key}`

### Corresponding site section

`https://hackvita.eu/dashboard`

### Successful response

```json
{
  "ok": true,
  "values": [
    {
      "log_date": "2021-10-24",
      "log_generations": 14
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