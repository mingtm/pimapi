# privilegedSignupStatus: canSignUp

Check if the requestor is able to sign up the tenant to Privileged Identity Management.
### Prerequisites
The following **scopes** are required to execute this API: _Directory.AccessAsUser.All_ 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedSignupStatus/canSignUp
```
### Request headers
| Name       | Description|
|:---------------|:----------|
| Authorization  | Bearer <code>|

### Request body

### Response
If successful, this method returns `200, OK` response code and boolean object in the response body.

### Example
Here is an example of how to call this API.
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "privilegedsignupstatus_cansignup"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedSignupStatus/canSignUp
```

##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "boolean"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 19

{
  "value": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedSignupStatus: canSignUp",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->