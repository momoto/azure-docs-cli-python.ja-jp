---
title: Azure CLI 2.0
description: "Azure CLI 2.0 の概要。"
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 5f3d514200b138d498043e0efb2cf5c2f478d108
ms.sourcegitcommit: f3ab5da6019083ef2482b62c7355817e6170dcfb
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/28/2018
---
# <a name="azure-cli-20"></a>Azure CLI 2.0

Azure CLI 2.0 は、Azure リソースを管理するための、Azure の新しいコマンド ライン エクスペリエンスです。
ブラウザーの [Azure Cloud Shell](/azure/cloud-shell/overview) で使用できるほか、macOS、Linux、Windows に[インストール](install-azure-cli.md)してコマンド ラインで実行することもできます。

Azure CLI 2.0 は、コマンド ラインから Azure リソースを管理したり、Azure Resource Manager を操作対象とする自動化スクリプトを作成したりするために最適化されています。 Azure CLI 2.0 を使用すると、次のコマンドを入力するだけで、簡単に Azure 内に VM を作成できます。

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

[Cloud Shell](/azure/cloud-shell/overview) を使用して CLI をブラウザーで実行することも、macOS、Linux、または Windows に[インストール](install-azure-cli.md)することもできます。
CLI を実際に使う際には、[概要](get-started-with-azure-cli.md)の記事をお読みください。
最新リリースについては、[リリース ノート](release-notes-azure-cli.md)をご覧ください。

Azure CLI 2.0 の基本的な使い方については、次のサンプルが参考になります。
- [Linux 仮想マシン](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Windows 仮想マシン](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Web Apps](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [SQL Database](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

個々の Azure CLI 2.0 コマンドの使用方法が記載された詳細な[リファレンス](/cli/azure/)も用意されています。

Azure CLI 2.0 を今すぐ[使ってみましょう](get-started-with-azure-cli.md)。


> [!NOTE]
> 以前のバージョンの CLI (Azure CLI) を使用している場合は、引き続きそれを使用できます。
> 両方の CLI を使用する場合は、`azure` が古い CLI (Azure CLI) で、`az` が新しい CLI (Azure CLI 2.0) であることを覚えておいてください。