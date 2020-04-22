---
title: "Quickstart: [Product Name] REST API | Microsoft Docs"
description: Get started with the [Product Name] REST API...
services: cognitive-services
author: 
manager: 
ms.service: cognitive-services
ms.subservice: 
ms.topic: quickstart
ms.date: 
ms.author: 
---

# Quickstart: Use cURL to call the [Product Name] REST API

Use this article to call the [Product Name] API using the REST API and cURL.

## Prerequisites

* The current version of [cURL](https://curl.haxx.se/).
* Once you have your Azure subscription, <a href="https://ms.portal.azure.com/#create/Microsoft.CognitiveServicesTextAnalytics"  title="Create a [Product Name] resource"  target="_blank">create a [Product Name] resource <span class="docon docon-navigate-external x-hidden-focus"></span></a> in the Azure portal to get your key and endpoint. After it deploys, click **Go to resource**.
    * You will need the key and endpoint from the resource you create to connect your application to the [Product Name] API. You'll paste your key and endpoint into the code below later in the quickstart.
    * You can use the free pricing tier (`F0`) to try the service, and upgrade later to a paid tier for production.

> [!NOTE]
> * The following BASH examples use the `\` line continuation character. If your console or terminal uses a different line continuation character, use that character.
> * Go to the Azure portal and find the key and endpoint for the [Product Name] resource you created in the prerequisites. They will be located on the resource's **key and endpoint** page, under **resource management**. Then replace the strings in the code below with your key and endpoint.

<!-- remember to change the cURL parameters to work with your service. -->

To call the [Product Name] API, you need the following information:
|Parameter  |Description  |
|---------|---------|
|`-X POST <endpoint>`     | Specifies your endpoint for accessing the API.        |
|`-H Content-Type: application/json`     | The content type for sending JSON data.          |
|`-H "Ocp-Apim-Subscription-Key:<key>`    | Specifies the key for accessing the API.        |
|`-d <documents>`     | The JSON containing the documents you want to send.         |

he following cURL command are executed from a BASH shell. Edit these commands with your own endpoint name, resource key, and JSON values.

## Example task

<!-- remember to change the example cURL command to work with your service. -->

```bash
curl -X POST https://<paste-your-[product-name]-endpoint-here>/.../... \
-H "Content-Type: application/json" \
-H "Ocp-Apim-Subscription-Key: <paste-your-[product-name]-key-here>" \
-d '{}'
```

### JSON response

```json

```

## Clean up resources

If you want to clean up and remove a resource, you can delete it or its resource group. Deleting the resource group also deletes any other resources associated with it.

* [Portal](https://docs.microsoft.com/azure/cognitive-services/cognitive-services-apis-create-account#clean-up-resources)
* [Azure CLI](https://docs.microsoft.com/azure/cognitive-services/cognitive-services-apis-create-account-cli#clean-up-resources)

## Next steps

> [!div class="nextstepaction"]
>[Explore a solution](https://docs.microsoft.com/azure/cognitive-services/text-analytics/text-analytics-user-scenarios#analyze-recorded-inbound-customer-calls)
