# Get specified apikey permissions

### Example request

`https://api.hackvita.eu/v2/account/getMyPermissions?api_key={api_key}`

### Successful response

```json
{
  "ok": true,
  "values": {
    "news": {
      "getAllNews": true,
      "getSiteNews": true,
      "getGeneratorNews": true
    },
    "orders": {
      "getMyOrders": true,
      "getCartElements": true,
      "getShopElements": true,
      "getUpgradesOrders": true,
      "getUpgradesElements": true
    },
    "..."
  }
}
```

### Possible errors

* INVALID_API_KEY
* USER_IS_BANNED
* PERMISSION_DENIED
* INTERNAL_ERROR