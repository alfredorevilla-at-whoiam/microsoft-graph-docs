---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var orgContact = await graphClient.Contacts["delta"]
	.Request()
	.Select( e => new {
			 e.DisplayName,
			 e.JobTitle,
			 e.Mail 
			 })
	.GetAsync();

```