---
title: "Quickstart: [Product name] client library for Go | Microsoft Docs"
description: Get started with the [Product Name] client library for Go...
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

# Quickstart: [Product Name] client library for Go

Get started with the [Product Name] client library for Go. Follow these steps to install the library and try out our examples for basic tasks. 

Use the [Product Name] client library for Go to: 

* Task 1
* Task 2
* ...

## Prerequisites

* An Azure subscription - [create one for free](https://azure.microsoft.com/free/)
* The latest version of [Go](https://golang.org/dl/)

## Setting up

<!-- 
    Consider turning this setup section into a reusable include file for your service 
-->

### Create a [Product Name] Azure resource 

Begin using the [Product Name] by creating an Azure resource. Choose the resource type below that's right for you:
<!--
    replace the links below with ones for your service
-->

* A [trial resource](https://azure.microsoft.com/try/cognitive-services/#decision) (no Azure subscription needed): 
    * Valid for seven days, for free. After signing up, a trial key and endpoint will be available on the [Azure website](https://azure.microsoft.com/try/cognitive-services/my-apis/). 
    * This is a great option if you want to try [Product Name], but don’t have an Azure subscription.
<!-- Link to the 'create' blade in the azure portal -->
* A [ [Product Name] resource](https://ms.portal.azure.com/#create/Microsoft.CognitiveServicesAnomalyDetector):
    * Available through the Azure portal until you delete the resource.
    * Use the free pricing tier to try the service, and upgrade later to a paid tier for production.
<!-- remove the below text if your service is not supported by the multi-service option. -->
* A [Multi-Service resource](https://ms.portal.azure.com/#create/Microsoft.CognitiveServicesAllInOne):
    * Available through the Azure portal until you delete the resource.  
    * Use the same key and endpoint for your applications, across multiple Cognitive Services.


### Create an environment variable

>[!NOTE]
> The endpoints for non-trial resources created after July 1, 2019 use the custom subdomain format shown below. For more information and a complete list of regional endpoints, see [Custom subdomain names for Cognitive Services](https://docs.microsoft.com/azure/cognitive-services/cognitive-services-custom-subdomains). 

Using your key and endpoint from the resource you created, create two environment variables for authentication:
<!-- replace the below variable names with the names expected in the code sample.-->
* `PRODUCT_NAME_KEY` - The resource key for authenticating your requests.
* `PRODUCT_NAME_ENDPOINT` - The resource endpoint for sending API requests. It will look like this: 
  * `https://<your-custom-subdomain>.api.cognitive.microsoft.com` 

Use the instructions for your operating system.
<!-- replace the below endpoint and key examples -->
#### [Windows](#tab/windows)

```console
setx PRODUCT_NAME_KEY <replace-with-your-product-name-key>
setx PRODUCT_NAME_ENDPOINT <replace-with-your-product-name-endpoint>
```

After you add the environment variable, restart the console window.

#### [Linux](#tab/linux)

```bash
export PRODUCT_NAME_KEY=<replace-with-your-product-name-key>
export PRODUCT_NAME_ENDPOINT=<replace-with-your-product-name-endpoint>
```

After you add the environment variable, run `source ~/.bashrc` from your console window to make the changes effective.

#### [macOS](#tab/unix)

Edit your `.bash_profile`, and add the environment variable:

```bash
export PRODUCT_NAME_KEY=<replace-with-your-product-name-key>
export PRODUCT_NAME_ENDPOINT=<replace-with-your-product-name-endpoint>
```

After you add the environment variable, run `source .bash_profile` from your console window to make the changes effective.
***

### Create a new Go project

In a console window (cmd, PowerShell, Terminal, Bash), create a new workspace for your Go project and navigate to it. Your workspace will contain three folders: 

* **src** - This directory contains source code and packages. Any packages installed with the `go get` command will reside here.
* **pkg** - This directory contains the compiled Go package objects. These files all have an `.a` extension.
* **bin** - This directory contains the binary executable files that are created when you run `go install`.

> [!TIP]
> Learn more about the structure of a [Go workspace](https://golang.org/doc/code.html#Workspaces). This guide includes information for setting `$GOPATH` and `$GOROOT`.

Let's create a workspace called `my-app` and the required sub directories for `src`, `pkg`, and `bin`:

```
$ mkdir -p my-app/{src, bin, pkg}  
$ cd my-app
```

### Install the client library for Go

Now, let's install the client library for Go: 

```bash
$ go get -u <library-location-or-url>
```

or if you use dep, within your repo run:

```bash
$ dep ensure -add <library-location-or-url>
```

### Create your Go application

Next, let's create a file named `src/sample-app.go`:

```bash
$ cd src
$ touch sample-app.go
```

Open `sample-app.go` in your favorite IDE or text editor. Then add the package name and import the following libraries:

```Go
package main

import (
	"..."
	"..."
)
```


## Object model 

## Code examples

These code samples show you how to complete basic tasks using the [Product Name] client library for Go:

* [Authenticate the client](#)
* [Example task 1 (anchor link)](#)
* [Example task 2 (anchor link)](#)
* [Example task 3 (anchor link)](#)

## Authenticate the client

> [!NOTE] 
> This quickstart assumes you've [created an environment variable](https://docs.microsoft.com/azure/cognitive-services/cognitive-services-apis-create-account#configure-an-environment-variable-for-authentication) for your [Product Name] key, named `TBD_KEY`.

In a new method, instantiate a client with your endpoint and key. Create an [ApiKeyServiceClientCredentials]() object with your key, and use it with your endpoint to create an [ApiClient]() object.

```go

```

## Example task 1

Example: Create a new method to read in the data and add it to a [Request](https://docs.microsoft.com/dotnet/) object as an array of [Points](https://docs.microsoft.com/dotnet/). Send the request with the [send()](https://docs.microsoft.com/dotnet/) method

```Go

```

## Example task 2

Example: Create a new method to read in the data and add it to a [Request](https://docs.microsoft.com/dotnet/) object as an array of [Points](https://docs.microsoft.com/dotnet/). Send the request with the [send()](https://docs.microsoft.com/dotnet/) method

```Go

```

## Run the application

Run your Go application with the `go run [arguments]` command from your application directory.

```Go
go run sample-app.go
```

## Clean up resources

If you want to clean up and remove a Cognitive Services subscription, you can delete the resource or resource group. Deleting the resource group also deletes any other resources associated with it.

* [Portal](../../cognitive-services-apis-create-account.md#clean-up-resources)
* [Azure CLI](../../cognitive-services-apis-create-account-cli.md#clean-up-resources)

## Troubleshooting

<!--
    This section is optional. If you know of areas that people commonly run into trouble, help them resolve those issues in this section
-->

## Next steps

> [!div class="nextstepaction"]
>[Next article]()

## See also

* [What is the [Product Name]?](#)
* [API reference](#)
* The source code for this sample can be found on [GitHub](#).