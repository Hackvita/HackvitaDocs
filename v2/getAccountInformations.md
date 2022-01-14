# Get your account informations

### Example request

`https://api.hackvita.eu/v2/account/getAccountInformations?api_key={api_key}`

### Corresponding site section

`https://hackvita.eu/dashboard`

### Successful response

```json
{
  "ok":true,
  "values": {
    // user basic informations
    "user_infos": {
      "username": "kuogitg",
      "email": "kuogitg@hackvita.eu",
      "role": "member",
      "id": "we9083434",
      "plan": 1,
      "credits": 23.45,
      "2fa": false
    },
    // user generations informations
    "generations":{
      "user_generations_today_private": 0,
      "user_generations_today_public": 0,
      "plan_generations_for_day_public": 0,
      "plan_generations_for_day_private": 0,
      "total_accounts_available": 1504820,
      "user_referreals": 0
    },
    // user selected plan informations
    "plan_informations":{
      "plan_id": 32,
      "plan_name": "Godddd",
      "plan_price": 40,
      "plan_price_ref": 0,
      "plan_public_day": 0,
      "plan_private_day": 0,
      "plan_is_hidden": false,
      "plan_duration": 640840,
      "plan_cbrenew": true
    }
  }
}
```

### Some informations

* **role** is your role on hackvita ("admin", "refiller", "shopadmin", "member")
* **plan** is your plan id (more informations on [/plans/getPlansList](getPlansList))
* **total_accounts_available** is the counter of total accounts available on the site

### Possible errors

* INVALID_API_KEY
* USER_IS_BANNED
* PERMISSION_DENIED
* INTERNAL_ERROR