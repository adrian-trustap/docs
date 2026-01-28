# Authentication

The Trustap API uses authentication to ensure that only authorized
clients can access and interact with resources. This guide explains the
types of authentication supported, how to use them, and when to use each
method.

Trustap uses authentication to do the following.
* Identify who is making a request.
* Prevent unauthorized access to user or transaction data.



## Types of Authentication Supported

Trustap supports multiple ways to authenticate API requests. We recommend Basic Authentication for most integrations. If you need to perform actions on behalf of a specific user, include the `Trustap-User` header. OAuth 2.0 is also available, but generally not required for partner integrations



## Authentication examples
### Basic Authentication

In cURL you can use `--user` and use the key you received during [setup](../intro/auth.md). Alternatively, you can use the header object `--header "Authorization: Basic $(echo -n '<YOUR_TOKEN_HERE>:' | base64)"`.


```CURL {% title="Basic Authentication - Create a guest buyer" %}
curl --location 'https://dev.stage.trustap.com/api/v1/guest_users' \
--header 'Content-Type: application/json' \
--user '<API_KEY>:' \
--data-raw '{"email":"bert.gray@my-mail.com","first_name":"Bert","last_name":"Gray","country_code":"at","tos_acceptance":{"unix_timestamp":1736354931,"ip":"127.0.0.1"}}'
```



### Basic Authentication with `Trustap-User`

```CURL {% title="Basic Authentication with Trustap-User - Confirm delivery" %}
curl -i -X POST \
  'https://dev.stage.trustap.com/api/v1/transactions/{transaction_id}/confirm_delivery_with_guest_buyer' \
  --user '<API_KEY>:' \
  --header 'Trustap-User: <USER_ID>'
```



### Authentication using Bearer token

```CURL {% title="Authentication with Bearer token - Confirm delivery" %}
curl -i -X POST \
  'https://dev.stage.trustap.com/api/v1/transactions/{transaction_id}/confirm_delivery_with_guest_buyer' \
  --header 'Authorization: Bearer <BEARER_API_TOKEN>' \
```
