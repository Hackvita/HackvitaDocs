# Get shop elements

### Example request

`https://api.hackvita.eu/v2/orders/getShopElements?api_key={api_key}`

### Corresponding site section

`https://hackvita.eu/dashboard?section=Shop`

### Successful response

```json
{
  "ok": true,
  "values": [
    {
      "element_id": 159,
      "element_name": "HackFlix",
      "element_description": "The best streaming service",
      "element_category": "streaming",
      "element_gc": 1,
      "element_in_stock": true,
      "element_is_hidden": false,
      "element_photo": "https://imgur.com/o109YvL.png",
      "element_price": 50
    }
  ]
}
```

### Some informations

* **element_gc** is an indicator that differentiates shop-admins. It is not important to consider
* **element_is_hidden**: it's always false for users

### Pay attention to the guaranteed duration!

As of 31/12/21, the element_description value is also used to describe the duration guaranteed by that specific element. Specifically, you will find the description in this format:
```guaranteedDuration:"ENGLISH DURATION";Rest of description```

**NOT ALL ELEMENTS WILL HAVE THIS FORMAT!** You can use a similar code (python):

```python
element_description = 'example'
if element_description.startsWith('guaranteedDuration:'):
  element_duration = element_description.split('guaranteedDuration:"')[1]
  element_duration = element_duration.split('"')[0]
  element_description = element_description.replace(f'guaranteedDuration:"{element_duration}";', '')
else:
  element_duration = 'random'

# element_duration is your desired duration
# element_description is your desired decription
```

### Possible errors

* INVALID_API_KEY
* USER_IS_BANNED
* PERMISSION_DENIED
* INTERNAL_ERROR