# Get your payments logs

### Example request

`https://api.hackvita.eu/v2/account/getPaymentsLogs?api_key={api_key}`

### Corresponding site section

`https://hackvita.eu/dashboard?section=Credits`

### Successful response

```json
{
  "ok": true,
  "values": [
    {
      "payment_time": 1624641968,
      "payment_method": "PayPal by Salvatore",
      "payment_amount": 30
    },
    {
      "payment_time": 1641843328,
      "payment_method": "Crypto",
      "payment_amount": 18
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