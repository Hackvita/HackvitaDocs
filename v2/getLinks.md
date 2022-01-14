# Get HackVita Links

### Example request

`https://api.hackvita.eu/v2/informations/getLinks?api_key={api_key}&language={it/en}`

### Corresponding site section

`https://hackvita.eu/dashboard?section=Informations`

### Successful response

```json
{
  "ok": true,
  // original dashboard links
  "values": [
    "https://hackvita.eu/dashboard?section=Dashboard", 
    "https://hackvita.eu/dashboard?section=AccountsList", 
    "https://hackvita.eu/dashboard?section=Referreal", 
    "https://hackvita.eu/dashboard?section=Credits",
    "..."
  ],
  // alternative links with hackvita.eu
  "alternate": [
    "https://hackvita.eu/dashboard/Dashboard", 
    "https://hackvita.eu/dashboard/AccountsList", 
    "https://hackvita.eu/dashboard/Referreal", 
    "https://hackvita.eu/dashboard/Credits",
    "..."
  ],
  // alternative links with dashboard.hackvita.eu
  "alternate_short": [
    "https://dashboard.hackvita.eu/Dashboard",
    "https://dashboard.hackvita.eu/AccountsList",
    "https://dashboard.hackvita.eu/Referreal",
    "https://dashboard.hackvita.eu/Credits",
    "..."
  ]
}
```

### Possible errors

* INVALID_API_KEY
* USER_IS_BANNED
* PERMISSION_DENIED
* INTERNAL_ERROR