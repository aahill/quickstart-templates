---
title: "Quickstart: [Product name] client library for Python | Microsoft Docs"
description: Get started with the [Product Name] client library for Python...
services: cognitive-services
author: 
manager: nitinme
ms.service: cognitive-services
ms.subservice: 
ms.topic: quickstart
ms.date: 
ms.author: 
---

<!-- 
You can find more guidance for formatting these quickstarts at: 
https://review.docs.microsoft.com/en-us/help/contribute/contribute-how-to-write-library-quickstart-v2?branch=pr-en-us-2187


Title: 
    The H1 of your Quickstart should be in the format: # Quickstart: [Product Name] client library for [Language]
-->

# Quickstart: [Product Name] client library for Python

Get started with the [Product Name] client library for Python. Follow these steps to install the package and try out the example code for basic tasks. 

<!-- 
    After the above line, briefly describe the service. You can often use the first line of the service's docs landing page for this.

    Next, add a bulleted list of the most common tasks supported by the library, prefaced with "Use the [Product Name] client library for [Language] to:". You provide code snippets for these tasks in the Code examples section later in the Quickstart. Keep the list short but include those tasks most developers need to perform with the library.

    Lastly, include the following single line of links targeting the library's companion content at the bottom of the introduction; make adjustments as necessary, for example NuGet instead of PyPi:
-->

Use the [Product Name] client library for Python to:

* TBD
* TBD

<!--
    Include the following single line of links targeting the library's companion content at the bottom of the introduction; make adjustments as necessary, but try not to include any other links or content in the introduction.
-->

[Reference documentation](https://docs.microsoft.com/dotnet/api/Microsoft.Azure.CognitiveServices.AnomalyDetector?view=azure-dotnet-preview) | [Library source code](https://github.com/Azure/azure-sdk-for-net/tree/master/sdk/cognitiveservices/AnomalyDetector) | [Package (PiPy)](https://www.nuget.org/packages/Microsoft.Azure.CognitiveServices.AnomalyDetector/) | [Samples](https://github.com/Azure-Samples/anomalydetector)

## Prerequisites

* Azure subscription - [Create one for free](https://azure.microsoft.com/free/cognitive-services/)
* [Python 3.x](https://www.python.org/)
<!-- this <a> link opens the Azure portal in a new tab/window. Replace the link with one to your service's resource create blade-->
* Once you have your Azure subscription, <a href="https://ms.portal.azure.com/#create/Microsoft.CognitiveServicesTextAnalytics"  title="Create a [Product Name] resource"  target="_blank">create a [Product Name] resource <span class="docon docon-navigate-external x-hidden-focus"></span></a> in the Azure portal to get your key and endpoint. Wait for it to deploy and click the **Go to resource** button.
    * You will need the key and endpoint from the resource you create to connect your application to [Product Name]. You'll paste your key and endpoint into the code below later in the quickstart.
    You can use the free pricing tier (`F0`) to try the service, and upgrade later to a paid tier for production.
    
## Setting up

<!--
    Walk the reader through preparing their environment for working with the client library. Include instructions for creating the Azure resources required to make calls to the service, obtaining credentials, and setting up their local development environment.

    See the "setting up" section for more details: 
    https://review.docs.microsoft.com/en-us/help/contribute/contribute-how-to-write-library-quickstart-v2?branch=pr-en-us-2187#setting-up 
-->

<!-- 
    Consider turning this setup section into a reusable include file for your service 
-->

### Install the client library

After installing Python, you can install the client library with:

```console
pip install --upgrade azure-cognitiveservices-[Product Name]
```

### Create a new python application

Create a new Python file and import the following libraries.

> [!TIP]
> Want to view the whole quickstart code file at once? You can find it on [GitHub](), which contains the code examples in this quickstart.

```python
import ...
```

Create variables for your resource's Azure endpoint and key.


> [!IMPORTANT]
> Go to the Azure portal. If the [Product name] resource you created in the **Prerequisites** section deployed successfully, click the **Go to Resource** button under **Next Steps**. You can find your key and endpoint in the resource's **key and endpoint** page, under **resource management**. 
>
> Remember to remove the key from your code when you're done, and never post it publicly. For production, consider using a secure way of storing and accessing your credentials. For example, [Azure key vault](https://docs.microsoft.com/azure/key-vault/key-vault-overview).

```python
key = "<paste-your-[product-name]-key-here>"
endpoint = "<paste-your-[product-name]-endpoint-here>"
```

## Object model

<!-- 
    Briefly introduce and describe the functionality of the library's main classes. Include links to their reference pages.

    Explain the object hierarchy and how the classes work together to manipulate resources in the service.
-->

## Code examples

<!--
    Include code snippets and short descriptions for each task you list in the the bulleted list. Briefly explain each operation, but include enough clarity to explain complex or otherwise tricky operations.

    Include links to the service's reference content when introducing a class for the first time
-->

These code snippets show you how to do the following with the [Product Name] client library for Python:

* [Authenticate the client](#)
* [Example task 1 (anchor link)](#)
* [Example task 2 (anchor link)](#)
* [Example task 3 (anchor link)](#)

## Authenticate the client

<!-- 
    The authentication section (and its H3) is required and must be the first code example in the section if your library requires authentication for use.
-->

Instantiate a client with your endpoint and key. Create an [ApiKeyServiceClientCredentials]() object with your key, and use it with your endpoint to create an [ApiClient]() object.

```python

```

## Example task 1

Example: Create a new method to read in the data and add it to a [Request](https://docs.microsoft.com/dotnet/) object as an array of [Points](https://docs.microsoft.com/dotnet/). Send the request with the [send()](https://docs.microsoft.com/dotnet/) method

```python

```

<!-- 
    Show the application output from each task, if output exists
    If this code sample is in a function, tell the reader to call it. For example:

    Call the `example()` function.

-->

## Example task 2

Example: Create a new method to read in the data and add it to a [Request](https://docs.microsoft.com/dotnet/) object as an array of [Points](https://docs.microsoft.com/dotnet/). Send the request with the [send()](https://docs.microsoft.com/dotnet/) method

```python

```

<!-- 
    If this code sample is in a function, tell the reader to call it. For example:

    Call the `example()` function.

-->

## Run the application

Run the application with the `python` command on your quickstart file.

```console
python quickstart-file.py
```

## Clean up resources

If you want to clean up and remove a Cognitive Services subscription, you can delete the resource or resource group. Deleting the resource group also deletes any other resources associated with it.

* [Portal](https://docs.microsoft.com/azure/cognitive-services/cognitive-services-apis-create-account#clean-up-resources)
* [Azure CLI](https://docs.microsoft.com/azure/cognitive-services/cognitive-services-apis-create-account-cli#clean-up-resources)

## Troubleshooting

<!--
    This section is optional. If you know of areas that people commonly run into trouble, help them resolve those issues in this section
-->

## Next steps

> [!div class="nextstepaction"]
>[Next article]()

* [What is the [Product Name] API?](../overview.md)
* [Article2](../overview.md)
* [Article3](../overview.md)