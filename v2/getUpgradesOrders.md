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

`order_notes` is used to tell the site what to show in the notes section. It contains keywords and they are associated like this:
* `order_notes` = `success` => `The procedure have been completed successfully: change your password for security reasons and enjoy your {0} subscription.`
* `order_notes` = `credentials` => `We were unable to log you in, probably due to incorrect credentials. We have refunded the credits you spent.`
* `order_notes` = `support` => `Sorry, we could not complete the procedure: please contact support to proceed.`
Or, sometimes, the staff can insert a customised value to be shown to the user. If no value is entered, `order_notes` will be null.

### Possible errors

* INVALID_API_KEY
* USER_IS_BANNED
* PERMISSION_DENIED
* INTERNAL_ERROR