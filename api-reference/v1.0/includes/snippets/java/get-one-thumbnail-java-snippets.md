---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Content {size} = graphClient.me().drive().items("{item-id}").thumbnails("{thumb-id}").{size}()
	.buildRequest()
	.get();

```