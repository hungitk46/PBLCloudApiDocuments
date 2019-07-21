Get account information by your token.
The your access token to prove your identity and access protected resources.

Includes a bearer token in the Authorization request header. This type of token lets you complete an action on behalf of a resource owner.
```bash
curl -v -X GET https://api-dev.pblcloud.com/api/v1/account/get-info \
  -H "Content-Type: application/json" \
  -H "Authorization: Bearer Access-Token"
```
The response shows the account information details:
```json
{
    "AccountId": 1,
    "UserName": "name@med2lab.com",
    "FirstName": "first_name",
    "LastName": "_last_name",
    "Email": "email@med2lab.com",
    "InstitutionId": 2,
    "InstitutionName": "Med2Lab"
}
```
