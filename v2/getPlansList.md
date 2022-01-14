# Get plans list

### Example request

`https://api.hackvita.eu/v2/plans/getPlansList?api_key={api_key}`

### Corresponding site section

`https://hackvita.eu/dashboard?section=PlansList`

### Successful response

```json
{
  "ok": true,
  "values": [
    {
      "plan_id": 29,
      "plan_name": "Trial",
      "plan_price": 4.99,
      "plan_price_ref": 5,
      "plan_public_day": 5,
      "plan_private_day": 0,
      "plan_is_hidden": 0,
      "plan_duration": 604800,
      "plan_cbrenew": 0
    },
    {
      "plan_id": 30,
      "plan_name": "Basic",
      "plan_price": 14.99,
      "plan_price_ref": 10,
      "plan_public_day": 15,
      "plan_private_day": 0,
      "plan_is_hidden": 0,
      "plan_duration": 1555200,
      "plan_cbrenew": 1
    },
    "..."
  ]
}
```

### Some informations

* **plan_price**: if "0", the plan is used internally and cannot be purchased
* **plan_is_hidden**: if your role is "member" it's always 0
* **plan_duration**: "-1" if the plan is permanent and used internally
* **plan_cbrenew**: indicates whether the plan can be renewed from the panel

### Possible errors

* INVALID_API_KEY
* USER_IS_BANNED
* PERMISSION_DENIED
* INTERNAL_ERROR