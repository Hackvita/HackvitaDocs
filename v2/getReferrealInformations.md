# Get your referreal informations

### Example request

`https://api.hackvita.eu/v2/account/getReferrealInformations?api_key={api_key}`

### Corresponding site section

`https://hackvita.eu/dashboard?section=Referreal`

### Successful response

```json
{
  "ok": true,
  "values": {
    "paid": {
      "counter": 1,
      "list": ["bbede5a"]
    },
    "unpaid": {
      "counter": 1,
      "list": ["bsald0s"]
    },
    "total_counter": 2,
    "share_url": {
      "base": "https://ref.hackvita.eu/bbede5a", 
      "gmail": "https://mail.google.com/mail/u/0/?fs=1&to&su=https://ref.hackvita.eu/bbede5a&tf=cm", 
      "twitter": "https://twitter.com/intent/tweet?url=https://ref.hackvita.eu/bbede5a", 
      "facebook": "https://www.facebook.com/sharer.php?u=https://ref.hackvita.eu/bbede5a", 
      "reddit": "https://reddit.com/submit?url=https://ref.hackvita.eu/bbede5a", 
      "linkedin": "https://www.linkedin.com/sharing/share-offsite/?url=https://ref.hackvita.eu/bbede5a", 
      "tumblr": "https://www.tumblr.com/widgets/share/tool?canonicalUrl=https://ref.hackvita.eu/bbede5a", 
      "blogger": "https://www.blogger.com/blog-this.g?u=https://ref.hackvita.eu/bbede5a", 
      "skype": "https://web.skype.com/share?url=https://ref.hackvita.eu/bbede5a", 
      "telegram": "https://t.me/share/url?url=https://ref.hackvita.eu/bbede5a", 
      "sms": "sms:?body=https://ref.hackvita.eu/bbede5a", 
      "vk": "http://vk.com/share.php?url=https://ref.hackvita.eu/bbede5a", 
      "whatsapp": "whatsapp://send/?text=https://ref.hackvita.eu/bbede5a"
    }
  }
}
```

### Some informations

* **list** is the list of user IDs that have registered with your referreal id
* **paid** means all users registered with your referreal id who have purchased at least one plan
* **unpaid**  means all users registered with your referreal id who haven't purchased at least one plan

### Possible errors

* INVALID_API_KEY
* USER_IS_BANNED
* PERMISSION_DENIED
* INTERNAL_ERROR