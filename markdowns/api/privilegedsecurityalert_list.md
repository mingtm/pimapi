# List privilegedSecurityAlerts

Retrieve a list of privilegedsecurityalert objects.
### Prerequisites
The following **scopes** are required to execute this API: _Directory.AccessAsUser.All_

The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_. 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedSecurityAlerts
```
### Optional query parameters
This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.

### Request headers
| Name      |Description|
|:----------|:----------|
| Authorization  | Bearer <code>|

### Request body
Do not supply a request body for this method.
### Response
If successful, this method returns a `200 OK` response code and collection of [privilegedSecurityAlert](../resources/privilegedsecurityalert.md) objects in the response body.
### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_privilegedsecurityalerts"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedSecurityAlerts
```
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedSecurityAlert",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 276

{
  "value": [
    {
      "id": "id-value",
      "numberOfAffectedItems": 99,
      "additionalData": "additionalData-value",
      "alertName": "alertName-value",
      "alertDescription": "alertDescription-value",
      "lastModifiedDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List privilegedSecurityAlerts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->