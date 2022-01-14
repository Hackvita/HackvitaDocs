# Get your informations

Get information regarding your profile and generations.

# Example request

`https://api.hackvita.eu/v1/getMyStatus?login_key=APIKEY`

# Successful response

Parameter | Description
--------- | -----------
user_infos | basically contains your data
generations | contains information about generations

```json
{
  "ok": true,
  "values": {
    "user_infos": {
      "username": "harmster",
      "email": "top@hackvita.eu",
      "id": "idk",
      "plan": {
        "plan_id": 29,
        "plan_name": "Trial",
        "plan_price": 5,
        "plan_price_ref": 5,
        "plan_duration": 120
      },
      "twofactor": false
    },
    "generations": {
      "user_generations_today_private": 0,
      "user_generations_today_public": 0,
      "plan_generations_for_day_public": 5,
      "plan_generations_for_day_private": 0,
      "total_accounts_available": 21565,
      "user_referreals": 2
    }
  }
}
```

# Possible errors

* invalid or no login_key