Download Postman for your environment.

In Postman, select the POST method.

Enter the https://api-dev.pblcloud.com/token request URL.

On the Body tab, select x-www-form-urlencoded.

- Type grant_type in the key box, and type client_credentials in the value box.
- Type username in the key box, and type your username in the value box.
- Type password in the key box, and type your password in the value box.

Click Send.

In exchange for these credentials, the PBL Cloud authorization server returns your access token in the access_token field:
```json
{
    "access_token": "your token at here",
    "token_type": "bearer",
    "expires_in": 31535999
}
```

Include this bearer token in the Authorization header with the Bearer authentication scheme in REST API calls to prove your identity and access protected resources. This sample request includes a bearer token:
```bat
curl -v -X GET https://api-dev.pblcloud.com/api/learner/opencase/caseinfo/340 \
  -H "Content-Type: application/json" \
  -H "Authorization: Bearer Access-Token"
```
Access tokens have a finite lifetime. The expires_in field contains the number of seconds after which the token expires. For example, an access token with an expiry value of 3600 expires in one hour from when the response was generated.

To detect when an access token expires, write code to either:

Keep track of the expires_in value in the token response.
Handle the HTTP 401 Unauthorized status code. The API endpoint issues this status code when it detects an expired token.
Re-use the access token until it expires. Then, get a new token.
