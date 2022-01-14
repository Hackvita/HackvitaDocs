# Get your cart elements

### Example request

`https://api.hackvita.eu/v2/orders/getMyOrders?api_key={api_key}`

### Corresponding site section

`https://hackvita.eu/dashboard?section=Orders`

### Successful response

```json
{
  "ok": true,
  "values": [
    {
      // order informations
      "order_id": 5,
      "order_quantity": 8,
      "order_date": "1618683764.056738",
      "order_status": "pending",
      "order_value": null,
      "order_discount": "5-perc",
      "order_subscription": 0,
      // element informations
      "element_id": 159,
      "element_category": "streaming",
      "element_name": "HackFlix",
      "element_description": "The best streaming service",
      "element_gc": 1,
      "element_in_stock": true,
      "element_is_hidden": false,
      "element_photo": "https://imgur.com/o109YvL.png",
      "element_price": 50
    },
    "..."
  ]
}
```

### Some informations

* **element_gc** is an indicator that differentiates shop-admins. It is not important to consider
* **element_is_hidden**: if your [role](getAccountInformations) is "member", it's always false
* **order_value** is always null if the order status is "pending"
* **order_subscription** is always 0 for the moment

### Pay attention to the order_discount!

In HackVita, discounts can be of two types: by percentage or by number. For percentage discounts, you will have a `number-perc` format; for example, if you have `5-perc`, there will be a 5% discount and then you will pay 95% of the original price. For number discounts, you will have a `number-numb` format; for example, if you have `5-numb` and the product costs 15€, you will pay 10€ (15€-5) instead of original price. If there is no discount code applied, you will get an `0-perc` value.

### Possible errors

* INVALID_API_KEY
* USER_IS_BANNED
* PERMISSION_DENIED
* INTERNAL_ERROR