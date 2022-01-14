# Get your cart elements

### Example request

`https://api.hackvita.eu/v2/orders/getCartElements?api_key={api_key}`

### Corresponding site section

`https://hackvita.eu/dashboard?section=Cart`

### Successful response
```json
{
  "ok": true,
  "values": [
    {
      // cart informations
      "cart_quantity": 7,
      // element informations
      "element_id": 159,
      "element_category": "streaming",
      "element_name": "HackFlix",
      "element_description": "The best streaming service",
      "element_gc": 1,
      "element_in_stock": true,
      "element_is_hidden": false,
      "element_photo": "https://imgur.com/o109YvL.png",
      "element_price": 49.99
    }
  ]
}
```

### Some informations

* **element_gc** is an indicator that differentiates shop-admins. It is not important to consider
* **element_is_hidden**: if your [role](getAccountInformations) is "member", it's always false

### Possible errors

* INVALID_API_KEY
* USER_IS_BANNED
* PERMISSION_DENIED
* INTERNAL_ERROR