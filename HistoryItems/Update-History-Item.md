Get List History Items by CaseId

In Postman, select the POST method.

Includes a bearer token in the Authorization request header. This type of token lets you complete an action on behalf of a resource owner.

`Authorization: Bearer Access-Token`

Enter the https://api-dev.pblcloud.com/api/history-item request URL.

On the Body tab, select raw with application/json.

Enter historyItem data with format:
```json
{
  "Id": 0,
  "CaseId": 0,
  "Name": "string",
  "Answer": "string",
  "Tags": "string"
}
```
- <b>Insert</b> a new HistoryItem: `Id=0`.
- <b>Update</b> an existing HistoryItem: `ID={historyItemId}`.

Click Send.

`Response Type:` int64.