# Get upgrades elements list

### Example request

`https://api.hackvita.eu/v2/plans/getUpgradesElements?api_key={api_key}`

### Corresponding site section

`https://hackvita.eu/dashboard?section=Upgrade`

### Successful response

```json
{
  "ok": true,
  "values": [
    {
      "upgrade_id": 1,
      "upgrade_name": "Netflix",
      "upgrade_subscription": "Ultra HD",
      "upgrade_image": "https://i.imgur.com/yps6dS0.png",
      "upgrade_price": 24.99,
      "upgrade_instock": 1
    },
    {
      "upgrade_id": 2,
      "upgrade_name": "Spotify",
      "upgrade_subscription": "Premium individual",
      "upgrade_image": "https://i.imgur.com/1r3SgXW.png",
      "upgrade_price": 14.99,
      "upgrade_duration": 31536000,
      "upgrade_instock": 0
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