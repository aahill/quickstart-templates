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

<!--
    Include the following single line of links targeting the library's companion content at the bottom of the introduction; make adjustments as necessary, but try not to include any other links or content in the introduction.
-->

[Reference documentation](tbd) | [Library source code](tbd) | [SDK download](tbd) | [Samples](tbd)

## Prerequisites

* An Azure subscription - [create one for free](https://azure.microsoft.com/free/)
* The latest version of [Go](https://golang.org/dl/)

## Setting up

### Create a [Product Name] Azure resource

Azure Cognitive Services are represented by Azure resources that you subscribe to. Create a resource for [Product name] using the [Azure portal](https://docs.microsoft.com/azure/cognitive-services/cognitive-services-apis-create-account) or [Azure CLI](https://docs.microsoft.com/azure/cognitive-services/cognitive-services-apis-create-account-cli) on your local machine. You can also:

* Get a [trial key](https://azure.microsoft.com/try/cognitive-services/#decision) valid for seven days for free. After you sign up, it will be available on the [Azure website](https://azure.microsoft.com/try/cognitive-services/my-apis/).
* View your resource on the [Azure portal](https://portal.azure.com).

<!-- rename TBD_KEY to something meaningful for your service, like TEXT_ANALYTICS_KEY -->
After you get a key from your trial subscription or resource, [create an environment variable](https://docs.microsoft.com/azure/cognitive-services/cognitive-services-apis-create-account#configure-an-environment-variable-for-authentication) for the key, named `TBD_KEY`.

### Create a Go project directory

In a console window (cmd, PowerShell, Terminal, Bash), create a new workspace for your Go project, named `my-app`, and navigate to it.

```
$ mkdir -p my-app/{src, bin, pkg}  
$ cd my-app
```

Your workspace will contain three folders:

* **src** - This directory will contain source code and packages. Any packages installed with the `go get` command will go here.
* **pkg** - This directory will contain the compiled Go package objects. These files all have an `.a` extension.
* **bin** - This directory will contains the binary executable files that are created when you run `go install`.

> [!TIP]
> To learn more about the structure of a Go workspace, see the [Go language documentation](https://golang.org/doc/code.html#Workspaces). This guide includes information for setting `$GOPATH` and `$GOROOT`.

### Install the client library for Go

Next, install the client library for Go:

```bash
$ go get -u <library-location-or-url>
```

or if you use dep, within your repo run:

```bash
$ dep ensure -add <library-location-or-url>
```

### Create a Go application

Next, create a file in the **src** directory named `sample-app.go`:

```bash
$ cd src
$ touch sample-app.go
```

Open `sample-app.go` in your preferred IDE or text editor. Then add the package name and import the following libraries:

```Go
package main

import (
	"..."
	"..."
)
```

## Object model

The following classes and interfaces handle some of the major features of the [Product Name] Go SDK.

|Name|Description|
|---|---|
| | |

## Code examples

These code samples show you how to complete basic tasks using the [Product Name] client library for Go:

* [Authenticate the client](#)
* [Example task 1 (anchor link)](#)
* [Example task 2 (anchor link)](#)
* [Example task 3 (anchor link)](#)

## Authenticate the client

> [!NOTE] 
> This quickstart assumes you've [created an environment variable](https://docs.microsoft.com/azure/cognitive-services/cognitive-services-apis-create-account#configure-an-environment-variable-for-authentication) for your [Product Name] key, named `TBD_KEY`.

In a new method, instantiate a client with your endpoint and key. Create a [CognitiveServicesCredentials](https://docs.microsoft.com/python/api/msrest/msrest.authentication.cognitiveservicescredentials?view=azure-python) object with your key, and use it with your endpoint to create an [ApiClient]() object.

```go

```

## Example task 1

Example: Create a new method to read in the data and add it to a [Request](https://docs.microsoft.com/dotnet/) object as an array of [Points](https://docs.microsoft.com/dotnet/). Send the request with the [send()](https://docs.microsoft.com/dotnet/) method

```Go

```

<!-- 
    If this code sample is in a function, tell the reader to call it. For example:

    Call the `example()` function.

-->

## Example task 2

Example: Create a new method to read in the data and add it to a [Request](https://docs.microsoft.com/dotnet/) object as an array of [Points](https://docs.microsoft.com/dotnet/). Send the request with the [send()](https://docs.microsoft.com/dotnet/) method

```Go

```

<!-- 
    If this code sample is in a function, tell the reader to call it. For example:

    Call the `example()` function.

-->

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