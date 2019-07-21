Get HistoryItem By Id

In Postman, select the GET method.

Includes a bearer token in the Authorization request header. This type of token lets you complete an action on behalf of a resource owner.

`Authorization: Bearer Access-Token`

Enter the https://api-dev.pblcloud.com/api/historyItem/{Id} request URL.

- `{Id}`: Id of the HistoryItem will get information.

Click Send.

`Response Type:` The information of history items.
```json
{
  "CaseId": 0,
  "HistoryItemId": 0,
  "HistoryItemName": "string",
  "HistoryItemAnswer": "string",
  "Tags": "string",
  "InstitutionId": 0,
  "Status": 0,
  "CreateDate": "2019-07-21T15:05:31.383Z",
  "CreateById": 0,
  "UpdateDate": "2019-07-21T15:05:31.383Z",
  "UpdateById": 0
}
```