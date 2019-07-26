# Create a new case from case template

In Postman, select the POST method.

Includes a bearer token in the Authorization request header. This type of token lets you complete an action on behalf of a resource owner.

`Authorization: Bearer Access-Token`

Enter the https://api-dev.pblcloud.com/api/case/create request URL.

On the Body tab, select raw with application/json.

Enter input data with format:
```json
{
  "templateId": 0, 
  "title": "string",
  "patientName": "string",
  "patientAge":0,
  "gender": 0,
  "freeNode": "string",
}
```
* All parameters is require

Click Send.

`Response Type:` int64.