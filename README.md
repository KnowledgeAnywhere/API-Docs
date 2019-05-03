# Knowledge Anywhere LMS API

Repository containing resources for using the [Knowledge Anywhere Public API](https://www.knowledgeanywhere.com).

## Getting Started.

See this article on the Knowledge Anywhere Helpdesk for information on getting started.

[Developer API](https://knowany.zendesk.com/hc/en-us/articles/360003301234-Knowledge-Anywhere-Public-API)

## Swagger Definition

**swagger.json** documents the available resources for using the LMS public API.  Swagger definition can also be viewed [online via Swagger Hub](https://app.swaggerhub.com/apis-docs/Knowledge-Anywhere/LMS_API/1.0.0).

## Postman Collection

A importable collection of Postman requests are available to use as a reference for developing an API collection.

You will need to [setup an environment](https://developers.onelogin.com/api-docs/1/getting-started/postman-collections) in Postman to use the collection.

Your environment should contain the following variables.

- `url` (value will be `https://publicapi.knowledgeanywhere.com` unless otherwise directed)
- `client` (client_id obtained from the **Client** column in your LMS administration panel)
- `secret` (client_secret obtained from the **Secret** column in your LMS administration panel)

After setting up your environment, the collection can be run out of the box.    Most requests in the collection contains a **Pre-Request** script that grabs and sets a token for you.   We still provide a **Get Auth Token** request as an example.

### Tips

- The request bodys are filled with sample/placeholder data that will need to be swapped out for real values in your system.
- The **Search Users** request comes with prefilled params.  Select the params section in postman and click the checkbox on the left to activate the selected criteria.   The values are placeholders and will need to be replaced with values from your current system.

## SDK

A Node SDK available via `npm install knowledgeanywhere`.   [Further reading](https://github.com/knowledgeAnywhere/FortunaSDK)

## Help

You can file a support ticket with our helpdesk if you need any assistance with getting setup with the Knowledge Anywhere API.

[Submit a Request for Support](https://knowany.zendesk.com/hc/en-us/requests/new)
