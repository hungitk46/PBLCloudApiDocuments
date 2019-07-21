Get Information of the case by id

In Postman, select the GET method.

Includes a bearer token in the Authorization request header. This type of token lets you complete an action on behalf of a resource owner.

`Authorization: Bearer Access-Token`

Enter the https://api-dev.pblcloud.com/api/learner/openCase/caseInfo/{caseId} request URL.

- `{caseId}`: Id of the case will get information.

Click Send.

`Response Type:` The information of case.
```json
{
  "CurrentId": 0,
  "CurrentTime": 0,
  "NextTime": 0,
  "Narrative": "string",
  "FinilizedCase": true,
  "CaseId": 0,
  "Title": "string",
  "Description": "string",
  "PatientName": "string",
  "PatientAge": 0,
  "Gender": true,
  "IsGuardian": true,
  "GuardianName": "string",
  "GuardianRelationship": "string",
  "ChiefComplain": "string",
  "InitialOverview": "string",
  "Diagnosis": "string",
  "HistoryImage": "string",
  "HistoryContent": "string",
  "Gold": 0,
  "Silver": 0,
  "Bronze": 0,
  "Pass": 0,
  "GenderName": "string",
  "InitalLocationName": "string",
  "GuardianDescription": "string"
}
```
