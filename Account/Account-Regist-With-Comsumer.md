Register a new account with pbl cloud api

In Postman, select the POST method.

Enter the https://api-dev.pblcloud.com/api/v1/account/registerwithconsumer request URL.

On the Body tab, select raw with application/json.
Enter RegisterWithComsumerDTO data with format:
```json
{
  "FirstName": "string",
  "LastName": "string",
  "Email": "string",
  "Password": "string",
  "ConsumerKey": "string",
  "SecretKey": "string"
}
```
Click Send.

`Response Type:` int (Id of new account has been created)