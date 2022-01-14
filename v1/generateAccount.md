# Generate an account from the private/public generator

You can generate as many daily private accounts as your plan allows. Here there is no distinction between public and private generators, you can specify a generator_id of either one or the other.

# Example request

`https://api.hackvita.eu/v1/generateAccount?login_key=APIKEY&gen_id=GENERATORID`

# Successful response

Parameter | Description
--------- | -----------
alt | The account and password, in the form of `username:password`.

```json
{
  "ok": true,
  "alt": "friends@hackvita.it:helloguy"
}
```

# Possible errors

* invalid or no generator_id 
* invalid or no login_key
* you don't have enough generations
* you can generate only one account every x seconds on this generator
* there are no accounts at the moment