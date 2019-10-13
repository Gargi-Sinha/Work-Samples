Set Auto Reply to Email Upon Receipt
===  
***This API can be used to set OOF messages***
----

>Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user. For example, an [automatic reply](https://docs.microsoft.com/en-us/graph/api/resources/automaticrepliessetting?view=graph-rest-1.0) to notify that the signed-in user is unavailable to respond to emails.

Properties
---
|Property        |Type                 |Description                                      |
|---------      |      ----------   |-------------------------------------------------|
|externalAudiance|externalAudienceScope|The set of audience external to signed-in user's organization who will receive the ExternalReplyMessage, if Status is `AlwaysEnabled `or `Scheduled`. The possible values are: none, `contactsOnly`, all.|
|externalReplyMessage|string|The automatic reply to send to the specified external audience, if Status is `AlwaysEnabled` or `Scheduled`.|
|internalReplyMessage|string|The automatic reply to send to the audience internal to the signed-in user's organization, if Status is   `AlwaysEnabled` or `Scheduled`.|
 

Code Sample in JSON
````json
{
  "externalAudience": "String",
  "externalReplyMessage": "string",
  "internalReplyMessage": "string",
  "scheduledEndDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "String"
}
````

##  Key attributes

+ Email
+ Timezone
+ Message
