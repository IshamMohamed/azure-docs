---
title: Azure CLI Script Example - Reset your account credentials | Microsoft Docs
description: Use the Azure CLI script to reset your account credentials and get the app.config settings back.
services: media-services
documentationcenter: ''
author: Juliako
manager: femila
editor: 

ms.assetid:
ms.service: media-services
ms.devlang: azurecli
ms.topic: sample
ms.tgt_pltfrm: multiple
ms.workload: na
ms.date: 08/20/2019
ms.author: juliako
---

# CLI example: Reset the account credentials

The Azure CLI script in this article shows how to reset your account credentials and get the app.config settings back.

## Prerequisites 

[Create a Media Services account](create-account-cli-how-to.md).

[!INCLUDE [media-services-cli-instructions.md](../../../includes/media-services-cli-instructions.md)]

## Example script

```
# Update the following variables for your own settings:
resourceGroup=amsResourceGroup
amsAccountName=amsmediaaccountname

az ams account sp reset-credentials \
  --account-name $amsAccountName \
  --resource-group $resourceGroup 
 ```

## Next steps

* [az ams](https://docs.microsoft.com/cli/azure/ams?view=azure-cli-latest)
* [Reset credentials](https://docs.microsoft.com/cli/azure/ams/account/sp?view=azure-cli-latest#az-ams-account-sp-reset-credentials)
