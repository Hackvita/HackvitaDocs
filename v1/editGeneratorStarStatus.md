# Add or remove from favorites a generator

By "generators" here we mean the list you can find by pressing on "account list" in the panel.

# Example request

`https://api.hackvita.eu/v1/editGeneratorStarStatus?login_key=APIKEY&generator_id=GEN_ID&is_starred=TRUE/FALSE`

# Successful response

We won't give you any information, just obviously "ok" to tell you if everything is ok.

```json
{
  "ok": true
}
```

# Possible errors

* invalid or no is_starred
* invalid or no generator_id
* invalid or no login_key
* selected generator is already starred
* selected generator isn't starred
* you have reached the maximum number of selectable generators (20)