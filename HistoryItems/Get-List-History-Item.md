Get List History Items by CaseId

In Postman, select the GET method.

Includes a bearer token in the Authorization request header. This type of token lets you complete an action on behalf of a resource owner.

`Authorization: Bearer Access-Token`

Enter the https://api-dev.pblcloud.com/api/history-item/list/{caseId} request URL.
- `{caseId}`: Id of the case will get list history items

Click Send.

`Response Type:` The collection history items in the case.
```json
[
  {
    "HistoryItemId": 0,
    "CaseId": 0,
    "HistoryItemName": "string",
    "HistoryItemAnswer": "string",
    "Tags": "string",
    "InstitutionId": 0,
    "Status": 0,
    "CreateDate": "2019-07-21T15:05:31.376Z",
    "CreateById": 0,
    "UpdateDate": "2019-07-21T15:05:31.376Z",
    "UpdateById": 0
  }
]
```