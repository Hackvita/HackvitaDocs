# Get the information of a generator type

You can get generator information by using the ID that is for example proposed to you in [/getGeneratorsList](getGeneratorsList).

# Example request

`https://api.hackvita.eu/v1/getGeneratorInformations?login_key=APIKEY&gen_id=GENERATORID`

# Successful response

Parameter | Description
--------- | -----------
generator_id | the id of the generator, can be used for example with the methods of the generations
generator_name | the name of the generator
generator_link | the link of the generator
generator_is_private | is the generator private? (bool)
generator_count | number of available accounts
generator_time_limit | minimum time between requests

```json
{
  "ok": true,
  "informations": {
    "generator_id": 6,
    "generator_name": "Disney+",
    "generator_link": "https://www.disneyplus.com/",
    "generator_is_private": true,
    "generator_count": 600,
    "generator_time_limit": 3600
  }
}
```

# Possible errors

* invalid or no login_key
* invalid or no generator_id