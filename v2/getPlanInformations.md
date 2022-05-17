# Get single plan informations

### Example request

`https://api.hackvita.eu/v2/plans/getPlanInformations?api_key={api_key}&plan_id={plan_id}`

### Corresponding site section

`https://hackvita.eu/dashboard?section=Plans`

### Successful response

```json
{
  "ok": true,
  "values": {
    "plan_id": 30,
    "plan_name": "Basic",
    "plan_price": 14.99,
    "plan_price_ref": 10,
    "plan_public_day": 15,
    "plan_private_day": 0,
    "plan_is_hidden": 0,
    "plan_duration": 1555200,
    "plan_cbrenew": 1
  }
}
```

### Possible errors

* INVALID_API_KEY
* INVALID_PLAN_ID
* USER_IS_BANNED
* PERMISSION_DENIED
* INTERNAL_ERROR