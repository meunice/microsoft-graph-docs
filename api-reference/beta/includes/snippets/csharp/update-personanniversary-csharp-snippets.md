---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personAnnualEvent = new PersonAnnualEvent
{
	AllowedAudiences = AllowedAudiences.Contacts
};

await graphClient.Me.Profile.Anniversaries["{id}"]
	.Request()
	.UpdateAsync(personAnnualEvent);

```