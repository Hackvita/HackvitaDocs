# Get HackVita FAQ

### Example request

`https://api.hackvita.eu/v2/informations/getFaq?api_key={api_key}&language={it/en}`

### Corresponding site section

`https://hackvita.eu/dashboard?section=Informations`

### Successful response

```json
{
  "ok": true,
  "values": [
    {
      "question": "What is Hackvita?",
      "answer": "Hackvita is a ge..."
    },
    {
      "question": "I want to generate...",
      "answer": "You must have a subscr...."
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