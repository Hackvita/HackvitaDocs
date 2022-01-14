# Buy plan using paid referreals

### Example request

`https://api.hackvita.eu/v2/plans/buyPlanReferreal?api_key={api_key}&plan_id={plan_id}`

### Successful response

```json
{
  "ok": true
}
```

### Possible errors

* INVALID_API_KEY
* INVALID_PLAN_ID
* PLAN_ALREADY_SELECTED
* PLAN_FORBIDDEN
* NOT_ENOUGH_PAID_REFERREALS
* USER_IS_BANNED
* PERMISSION_DENIED
* A_PLAN_IS_PAUSED
* INTERNAL_ERROR