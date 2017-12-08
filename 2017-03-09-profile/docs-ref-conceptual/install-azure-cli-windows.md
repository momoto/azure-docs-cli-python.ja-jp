---
title: "Windows での Azure CLI のインストール"
description: "Windows で Azure CLI 2.0 をインストールする方法"
keywords: "Azure CLI,Azure CLI のインストール,azure インストール windows, azure cli windows, azure windows"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 11/01/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: 96a123575226f281accf125cb5bb29ee7d14ef2a
ms.sourcegitcommit: 905939cc44764b4d1cc79a9b36c0793f7055a686
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/20/2017
---
# <a name="install-azure-cli-20-on-windows"></a>Windows での Azure CLI 2.0 のインストール

Windows では、MSI からネイティブ バイナリをインストールできます。これは、Windows コマンド プロンプトまたは PowerShell から使用できます。 Windows Subsystem for Linux (WSL) を使用している場合は、実行しているディストリビューションで使用できるパッケージがあります。 サポートされているパッケージ マネージャーの一覧または WSL での手動インストール方法については、[メインのインストール ページ](install-azure-cli.md)を参照してください。

## <a name="install-or-update-with-msi"></a>MSI でのインストールまたは更新

再頒布可能 MSI は、Windows での `az` コマンドのインストール、更新、およびアンインストールに使用されます。 [MSI インストーラーをダウンロード](https://aka.ms/InstallAzureCliWindows)して実行し、インストールまたは更新できます。

インストーラーによって、コンピューターに変更を加えるかどうかを尋ねるメッセージが表示されたら、[はい] をクリックします。

これで、Windows コマンド プロンプトまたは PowerShell のいずれかから、`az` コマンドで Azure CLI を実行できるようになりました。

## <a name="uninstall-with-msi"></a>MSI でのアンインストール

Azure CLI が不要であると判断した場合は、アンインストールすることができます。 アンインストールする前に、`az feedback` コマンドを使用して、アンインストールの理由と、CLI エクスペリエンスの改善方法について、ご意見をお聞かせください。 Microsoft では、できる限り Azure CLI のバグをなくし、使いやすいものにしたいと考えています。 また、[GitHub に問題を提出](https://github.com/Azure/azure-cli/issues)していただくこともできます。

アンインストールするには、MSI をもう一度実行して、"アンインストール" オプションを選択します。 MSI インストーラーが使用できなくなっている場合は、[ダウンロード](https://aka.ms/InstallAzureCliWindows)できます。