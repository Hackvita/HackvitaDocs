# Generate public account

### Example request

`https://api.hackvita.eu/v2/generators/generatePublicAccount?api_key={api_key}&generator_id={generator_id}`

### Corresponding site section

`https://hackvita.eu/dashboard?section=PublicGenerator`

### Successful response

```json
{
  "ok": true,
  "alt": "HackStream@phoenix.com:hackflix2021"
}
```

### Possible errors

* INVALID_API_KEY
* INVALID_GENERATOR_ID
* GENERATOR_IS_PRIVATE
* TIME_LIMIT
* NO_ACCOUNT_AVAILABLE
* NO_GENERATIONS_LEFT
* USER_IS_BANNED
* PERMISSION_DENIED
* INTERNAL_ERROR