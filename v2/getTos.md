# Get HackVita TOS

### Example request

`https://api.hackvita.eu/v2/informations/getTos?api_key={api_key}&language={it/en}`

### Corresponding site section

`https://hackvita.eu/dashboard?section=Informations`

### Successful response

```json
{
  "ok": true,
  "values": {
    "Terms Of Service": [
      "a) When you register with HackVita you agree to our Terms of Service.",
      "b) We reserve the right to change the TOS and subscription fees at any time without notice."
    ],
    "Sale": [
      "a) You cannot sell your HackVita account, especially if it has an active plan. The penalty is a permanent ban with no refund.",
      "b) The sale of accounts is similarly prohibited, especially if in large quantities.",
      "c) The resale of entire plans is also prohibited."
    ],
    "..."
  }
}
```

### Possible errors

* INVALID_LANGUAGE
* INVALID_API_KEY
* USER_IS_BANNED
* PERMISSION_DENIED
* INTERNAL_ERROR