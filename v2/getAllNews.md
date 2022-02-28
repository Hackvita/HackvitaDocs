# Get all news

### Example request

`https://api.hackvita.eu/v2/news/getAllNews?api_key={api_key}`

### Corresponding site section

`https://hackvita.eu/dashboard`

### Successful response

```json
{
  "ok": true,
  "values": [
    {
      "news_id": 5,
      "news_text": "Hello friends!",
      "news_time": 1618862953,
      "news_category": "general",
      "news_edited": true,
      "news_media": null
    },
    {
      "news_id": 6,
      "news_text": "What are you doing?",
      "news_time": 1618862953,
      "news_category": "generator",
      "news_edited": false,
      "news_media": "https://i.imgur.com/7BNPDsf.jpg"
    },
    "..."
  ]
}
```

### Some informations

* **news_category** is the news type ("general", "generator"). Use [/news/getGeneratorNews](getGeneratorNews) or [/news/getSiteNews](getSiteNews) to get single-type news
* **news_edited**: has the news been modified by the administrators?
* **news_media**: imgur.com media url or null

### Possible errors

* INVALID_API_KEY
* USER_IS_BANNED
* PERMISSION_DENIED
* INTERNAL_ERROR