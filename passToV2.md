# Pass from V1 TO V2

### Methods

* [/getGeneratorsList](v1/getGeneratorsList) -> [/generators/getAccountsList](v2/getAccountsList)
* [/generateAccount](v1/generateAccount) -> [/generators/generatePublicAccount](v2/generatePublicAccount) and [/generators/generatePrivateAccount](v2/generatePrivateAccount)
* [/getGeneratorInformations](v1/getGeneratorInformations) -> [/generators/getGeneratorInformations](v2/getGeneratorInformations)
* [/editGeneratorStarStatus](v1/editGeneratorStarStatus) -> **deprecated**
* [/getGenerationLogs](v1/getGenerationLogs) -> [/generators/getGenerationLogs](v2/getGenerationLogs)
* [/getMyStatus](v1/getMyStatus) -> [/account/getAccountInformations](v2/getAccountInformations)
* [/addCredits](addCredits) -> **deprecated**

### Responses

Most of the answers have changed. The most important feature is that now all values are under one and the same index: "values". We recommend reviewing all [documentation](v2/).

### Errors

Errors are no longer found under "description" but under "error" and include a code, no longer a sentence. Some examples:

* INTERNAL_ERROR
* INVALID_API_KEY