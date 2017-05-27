---
title: "Azure CLI 2.0 を使用して Azure サブスクリプションを管理する"
description: "Linux、Mac、または Windows 上で Azure CLI 2.0 を使用して Azure サブスクリプションを管理します。"
keywords: "Azure CLI 2.0, Linux, Mac, Windows, OS X, サブスクリプション"
author: kamaljit
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 98fb955e-6dbf-47e2-80ac-170d6d95cb70
ms.openlocfilehash: a28b24dd186fc567f36e52f8a0f5a7c2b0af060c
ms.sourcegitcommit: c2d380f4ad8e7606850530db690855bcccfd6e86
ms.translationtype: HT
ms.contentlocale: ja-JP
---
# <a name="manage-multiple-azure-subscriptions"></a>複数の Azure サブスクリプションの管理

Azure を使い始めたばかりの場合、所有しているサブスクリプションは 1 つだけだと思われます。
一方、しばらく前から Azure を使用している場合は、複数の Azure サブスクリプションを作成済みであることも考えられます。
その場合は、特定のサブスクリプションに対してコマンドを実行するように Azure CLI 2.0 を構成できます。

1. アカウント内のすべてのサブスクリプションの一覧を取得します。

   ```azurecli
   az account list --output table
   ```

   ```Output
   Name                                         CloudName    SubscriptionId                        State     IsDefault
   -------------------------------------------  -----------  ------------------------------------  --------  -----------
   My Production Subscription                   AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled
   My DevTest Subscription                      AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled   True
   My Demos                                     AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled
   ```

1. 既定値を設定します。
 
   ```azurecli
   az account set --subscription "My Demos"
   ```

   > [!NOTE]
   > `--subscription` パラメーターには、サブスクリプション名またはサブスクリプション ID を指定します。

`az account list --output table` コマンドをもう一度実行して、変更を検証できます。

既定のサブスクリプションを設定すると、後続のすべての Azure CLI コマンドは、このサブスクリプションに対して実行されます。