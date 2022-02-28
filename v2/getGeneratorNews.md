# Get all generator-related news

### Example request

`https://api.hackvita.eu/v2/news/getGeneratorNews?api_key={api_key}`

### Corresponding site section

`https://hackvita.eu/dashboard`

### Successful response

```json
{
  "ok": true,
  "values": [
    {
      "news_id": 6,
      "news_text": "What are you doing?",
      "news_time": 1618862953,
      "news_category": "generator",
      "news_edited": false,
      "news_media": null
    },
    "..."
  ]
}
```

### Some informations

* **news_category** is always "general" for this method
* **news_edited**: has the news been modified by the administrators?
* **news_media**: imgur.com media url or null

### Possible errors

* INVALID_API_KEY
* USER_IS_BANNED
* PERMISSION_DENIED
* INTERNAL_ERROR