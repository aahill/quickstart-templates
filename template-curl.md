---
title: "Quickstart: Text Analytics REST API | Microsoft Docs"
description: Get started with the Text Analytics REST API
services: cognitive-services
author: aahill
manager: nitinme
ms.service: cognitive-services
ms.subservice: text-analytics
ms.topic: quickstart
ms.date: 04/22/2020
ms.author: aahi
---

# Quickstart: Use cURL to call the Text Analytics REST API

This quickstart walks you calling the Text Analytics API using the REST API and cURL. Looking for code samples 

## Prerequisites

* The current version of [cURL](https://curl.haxx.se/).
* Once you have your Azure subscription, <a href="https://ms.portal.azure.com/#create/Microsoft.CognitiveServicesTextAnalytics"  title="Create a Text Analytics resource"  target="_blank">create a Text Analytics resource <span class="docon docon-navigate-external x-hidden-focus"></span></a> in the Azure portal to get your key and endpoint. After it deploys, click **Go to resource**.
    * You will need the key and endpoint from the resource you create to connect your application to the Text Analytics API. You'll paste your key and endpoint into the code below later in the quickstart.
    * You can use the free pricing tier (`F0`) to try the service, and upgrade later to a paid tier for production.

> [!NOTE]
> * The following BASH examples use the `\` line continuation character. If your console or terminal uses a different line continuation character, use that character.
> * Go to the Azure portal and find the key and endpoint for the Text Analytics resource you created in the prerequisites. They will be located on the resource's **key and endpoint** page, under **resource management**. Then replace the strings in the code below with your key and endpoint.

To call the Text Analytics API, you need the following information:
|parameter  |Description  |
|---------|---------|
|`-X POST <endpoint>`     | Specifies your endpoint for accessing the API.        |
|`-H Content-Type: application/json`     | The content type for sending JSON data.          |
|`-H "Ocp-Apim-Subscription-Key:<key>`    | Specifies the key for accessing the API.        |
|`-d <documents>`     | The JSON containing the documents you want to send.         |

he following cURL command are executed from a BASH shell. Edit these commands with your own endpoint name, resource key, and JSON values.

## Sentiment Analysis

#### [version 3.0](#tab/version-3)

```bash
curl -X POST https://<paste-your-text-analytics-endpoint-here>/text/analytics/v3.0/sentiment/ \
-H "Content-Type: application/json" \
-H "Ocp-Apim-Subscription-Key: <paste-your-text-analytics-key-here>" \
-d '{ documents: [{ id: "1", text: "I had the best day of my life. I wish you were there with me."}]}'
```

### JSON response

```json
{
  "documents":[
    {
      "id":"1",
      "sentiment":"positive",
      "documentScores":{
        "positive":1.0,
        "neutral":0.0,
        "negative":0.0
      },
      "sentences":[
        {
          "sentiment":"positive",
          "sentenceScores":{
            "positive":1.0,
            "neutral":0.0,
            "negative":0.0
          },
          "offset":0,
          "length":30
        }
      ]
    }
  ],
  "errors":[
  ],
  "modelVersion":"2019-10-01"
}
```

#### [version 3.1-preview](#tab/version-3-preview)

<!-- cURL command and JSON response -->

---

## Language detection

#### [version 3.0](#tab/version-3)

<!-- cURL command and JSON response -->

#### [version 3.1-preview](#tab/version-3)

<!-- cURL command and JSON response -->

---

## Named Entity Recognition (NER)

#### [version 3.0](#tab/version-3)

<!-- cURL command and JSON response -->

#### [version 3.1-preview](#tab/version-3)

<!-- cURL command and JSON response -->
 
### Detecting personal information

<!-- cURL command and JSON response -->
 
---

## Entity linking

#### [version 3.0](#tab/version-3)

<!-- cURL command and JSON response -->

#### [version 3.1-preview](#tab/version-3)

<!-- cURL command and JSON response -->

## Clean up resources

If you want to clean up and remove a resource, you can delete it or its resource group. Deleting the resource group also deletes any other resources associated with it.

* [Portal](https://docs.microsoft.com/azure/cognitive-services/cognitive-services-apis-create-account#clean-up-resources)
* [Azure CLI](https://docs.microsoft.com/azure/cognitive-services/cognitive-services-apis-create-account-cli#clean-up-resources)

## Next steps

> [!div class="nextstepaction"]
>[Explore a solution](https://docs.microsoft.com/azure/cognitive-services/text-analytics/text-analytics-user-scenarios#analyze-recorded-inbound-customer-calls)
