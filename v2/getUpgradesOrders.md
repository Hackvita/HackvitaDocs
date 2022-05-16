# Get your upgrade history

### Example request

`https://api.hackvita.eu/v2/orders/getUpgradesOrders?api_key={api_key}`

### Corresponding site section

`https://hackvita.eu/dashboard?section=UpgradeHistory`

### Successful response

```json
{
  "ok": true,
  "values": [
    {
      // order informations
      "order_id": 43,
      "order_element": 5,
      "order_date": "1618683764.056738",
      "order_status": "pending",
      "order_email": "test@gmail.com",
      "order_notes": "null",
      // upgrade informations
      "upgrade_id": 1,
      "upgrade_name": "Netflix",
      "upgrade_subscription": "Ultra HD",
      "upgrade_image": "https://i.imgur.com/yps6dS0.png",
      "upgrade_price": 24.99,
      "upgrade_duration": 31536000,
      "upgrade_instock": 1
    },
    "..."
  ]
}
```

### Pay attention to the order_notes parameter!

More information will be added as soon as possible.

### Possible errors

* INVALID_API_KEY
* USER_IS_BANNED
* PERMISSION_DENIED
* INTERNAL_ERROR