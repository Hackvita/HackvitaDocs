# V2 API Documentation

## API Base URL

`https://api.hackvita.eu/v2/{type}/{method}?api_key={api_key}&other_params`

## Methods List

* [/account/getAccountInformations](getAccountInformations)
* [/account/getReferrealInformations](getReferrealInformations)
* [/account/getPaymentsLogs](getPaymentsLogs)
* [/account/getMyPermissions](getMyPermissions)

* [/plans/getPlansList](getPlansList)
* [/plans/buyPlanCredits](buyPlanCredits)
* [/plans/buyPlanReferreal](buyPlanReferreal)
* [/plans/getPlanInformations](getPlanInformations)

* [/orders/getCartElements](getCartElements)
* [/orders/getShopElements](getShopElements)
* [/orders/getMyOrders](getMyOrders)
* [/orders/getUpgradesElements](getUpgradesElements)
* [/orders/getUpgradesOrders](getUpgradesOrders)

* [/generators/getAccountsList](getAccountsList)
* [/generators/getStarredAccountsList](getStarredAccountsList)
* [/generators/generatePublicAccount](generatePublicAccount)
* [/generators/generatePrivateAccount](generatePrivateAccount)
* [/generators/getGenerationLogs](getGenerationLogs)
* [/generators/getGenerationGraphValues](getGenerationGraphValues)
* [/generators/getGeneratorInformations](getGeneratorInformations)

* [/news/getAllNews](getAllNews)
* [/news/getGeneratorNews](getGeneratorNews)
* [/news/getSiteNews](getSiteNews)

* [/informations/getLinks](getLinks)
* [/informations/getFaq](getFaq)
* [/informations/getTos](getTos)

## API changelogs

### 2022-05-17: **Introducing some new methods.**

Here are the new features of this update:
* we hae added [/account/getMyPermissions](getMyPermissions) to allow you to see the list of permissions that is active for that particular key
* we have added [/orders/getUpgradesElements](getUpgradesElements) to allow you to get the full list of items available in the upgrade section
* we have added [/orders/getUpgradesOrders](getUpgradesOrders) to allow you to obtain the history list containing upgrades already performed in the past
* we have added [/plans/getPlanInformations](getPlanInformations) to allow you to see the information of an individual plan directly, without having to go through the complete list

For API keys already created up to this point, all new commands will be turned off by default except [/account/getMyPermissions](getMyPermissions). To use them, activate them from our dashboard.

### 2021-12-31: **Check guaranteedDuration in shopElements!**

As of 31/12/21, the element_description value is also used to describe the duration guaranteed by that specific element. More informations here: [/orders/getShopElements](getShopElements).

### 2021-11-16: **Introducing plan_informations value.**

We know that knowing active plan information is very helpful, and we also know that it is difficult to make many requests at once with limits. As of now, plan_informations is available in /account/getAccountInformations to quickly get the plan information.
It's used in [/account/getAccountInformations](getAccountInformations).

### 2021-11-16: **Introducing A_PLAN_IS_PAUSED error.**

Although it has not yet been announced on the channel, it will soon be possible to suspend the plans. During the suspension, no other plans can be purchased.
It's used in [/plans/buyPlanCredits](buyPlanCredits) and [/plans/buyPlanReferreal](buyPlanReferreal).

### 2021-11-02: **Introducing plan_cbrenew.**

As indicated on the channel, it is now possible to renew your plan if it is about to expire; however, not all plans are renewable. For the moment it is not possible to renew from api, but you can find out which plans can be renewed and which cannot.
It's used in [/plans/getPlansList](getPlansList).

### 2021-07-06: **Big HackVita update.**

Although the update has not yet been announced on the channel and other sources, the latest changes are already available to everyone. From now on, it is possible to choose which methods a single API key can use (this is how the PERMISSION_DENIED error arises). Find out more by going to the dedicated section of the panel.