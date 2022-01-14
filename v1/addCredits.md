# Get links to add credits

Using the method you'll be able to find some information about adding credits.

# Example request

`https://api.hackvita.eu/v1/addCredits?login_key=APIKEY`

# Successful response

Parameter | Description
--------- | -----------
paypal_pool_link | link to the paypal pool where to make the payment (false if not available)
paypal_code | the code to be inserted in the reason for payment
cryptocurrencies_link | currently unsupported

```json
{
  "ok": true,
  "paypal_pool_link": "https://paypal.me/pools/c/8zDy8f5ov8",
  "paypal_code": "#CODEx",
  "cryptocurrencies_link": false
}
```

# Possible errors

* invalid or no login_key
* no payment method supported now