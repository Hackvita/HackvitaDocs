# Get generation logs

Use this method to get logs of past generations on the site.

# Example request

`https://api.hackvita.eu/v1/getGenerationLogs?login_key=APIKEY`

# Successful response

Parameter | Description
--------- | -----------
log_id | specific log id
log_date | date on which the account was generated
log_alt | required credentials, usually username:password
log_is_private | true or false, depending on the type of generator used
log_user_id | your user id, usually useless
log_type | generator name

```json
{
  "ok": true,
  "values": [
    {
      "log_id": 1,
      "log_date": "2021-04-29",
      "log_alt": "hackvita@hackvita.eu:555spotify",
      "log_is_private": false,
      "log_user_id":"your_id",
      "log_type": "Netflix"
    },
    "..."
  ]
}
```

# Possible errors

* invalid or no login_key