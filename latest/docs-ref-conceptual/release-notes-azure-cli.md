---
title: "Azure CLI 2.0 リリース ノート"
description: "Azure CLI 2.0 の最新情報について説明します"
keywords: "Azure CLI 2.0, リリース ノート"
author: sptramer
ms.author: sttramer
manager: douge
ms.date: 04/03/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ce0428f7-0a59-4e72-9237-d907b171af51
ms.openlocfilehash: e893b99349bbf2a5eec8af254158eb07001f1da7
ms.sourcegitcommit: f107cf927ea1ef51de181d87fc4bc078e9288e47
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2017
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="77658-104">Azure CLI 2.0 リリース ノート</span><span class="sxs-lookup"><span data-stu-id="77658-104">Azure CLI 2.0 release notes</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="77658-105">2017 年 8 月 28 日</span><span class="sxs-lookup"><span data-stu-id="77658-105">August 28, 2017</span></span>

<span data-ttu-id="77658-106">バージョン 2.0.15</span><span class="sxs-lookup"><span data-stu-id="77658-106">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="77658-107">CLI</span><span class="sxs-lookup"><span data-stu-id="77658-107">CLI</span></span>

* <span data-ttu-id="77658-108">`--version` に法的事項を追加しました。</span><span class="sxs-lookup"><span data-stu-id="77658-108">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="77658-109">ACS</span><span class="sxs-lookup"><span data-stu-id="77658-109">ACS</span></span>

* <span data-ttu-id="77658-110">プレビュー リージョンを修正しました。</span><span class="sxs-lookup"><span data-stu-id="77658-110">Corrected preview regions.</span></span>
* <span data-ttu-id="77658-111">既定の `dns_name_prefix` を正しい形式にしました。</span><span class="sxs-lookup"><span data-stu-id="77658-111">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="77658-112">ACS コマンド出力を最適化しました。</span><span class="sxs-lookup"><span data-stu-id="77658-112">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="77658-113">Appservice</span><span class="sxs-lookup"><span data-stu-id="77658-113">Appservice</span></span>

* <span data-ttu-id="77658-114">[重大な変更] `az webapp config appsettings [delete|set]` の出力の不整合を修正しました</span><span class="sxs-lookup"><span data-stu-id="77658-114">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="77658-115">`az webapp config container set --docker-custom-image-name` の `-i` の新しいエイリアスを追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-115">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="77658-116">`az webapp log show` を公開しました</span><span class="sxs-lookup"><span data-stu-id="77658-116">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="77658-117">App Service プラン、メトリック、または DNS 登録を保持するために、`az webapp delete` の新しい引数を公開しました</span><span class="sxs-lookup"><span data-stu-id="77658-117">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="77658-118">修正済み: スロット設定の正常な検出</span><span class="sxs-lookup"><span data-stu-id="77658-118">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="77658-119">IoT</span><span class="sxs-lookup"><span data-stu-id="77658-119">IoT</span></span>

* <span data-ttu-id="77658-120">修正済み #3934: ポリシーの作成で既存のポリシーが消去されなくなりました</span><span class="sxs-lookup"><span data-stu-id="77658-120">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="77658-121">ネットワーク</span><span class="sxs-lookup"><span data-stu-id="77658-121">Network</span></span>

* <span data-ttu-id="77658-122">[重大な変更] 名前を `vnet list-private-access-services` から `vnet list-endpoint-services` に変更しました</span><span class="sxs-lookup"><span data-stu-id="77658-122">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="77658-123">[重大な変更] `vnet subnet [create|update]` のオプション `--private-access-services` の名前を `--service-endpoints` に変更しました</span><span class="sxs-lookup"><span data-stu-id="77658-123">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="77658-124">`nsg rule [create|update]` に対する複数 IP およびポート範囲のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-124">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="77658-125">`lb create` に対する SKU のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-125">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="77658-126">`public-ip create` に対する SKU のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-126">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="77658-127">プロファイル</span><span class="sxs-lookup"><span data-stu-id="77658-127">Profile</span></span>

* <span data-ttu-id="77658-128">仮想マシンの ID を使用してログインするために、`--msi` と `--msi-port` を公開しました</span><span class="sxs-lookup"><span data-stu-id="77658-128">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="77658-129">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="77658-129">Service Fabric</span></span>

* <span data-ttu-id="77658-130">プレビュー リリース</span><span class="sxs-lookup"><span data-stu-id="77658-130">Preview release</span></span>
* <span data-ttu-id="77658-131">コマンドに対するレジストリのユーザー/パスワード規則を簡略化しました</span><span class="sxs-lookup"><span data-stu-id="77658-131">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="77658-132">パラメーターを渡した後でもユーザーにパスワードの入力が求められる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77658-132">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="77658-133">空の `registry_cred` のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-133">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="77658-134">Storage</span><span class="sxs-lookup"><span data-stu-id="77658-134">Storage</span></span>

* <span data-ttu-id="77658-135">BLOB 層の設定を有効にしました</span><span class="sxs-lookup"><span data-stu-id="77658-135">Enabled setting blob tier</span></span>
* <span data-ttu-id="77658-136">サービス トンネリングをサポートするために、`--bypass` 引数と `--default-action` 引数を `storage account [create|update]` に追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-136">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="77658-137">VNET ルールと IP ベースのルールを `storage account network-rule` に追加するためのコマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-137">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>  
* <span data-ttu-id="77658-138">顧客管理キーによるサービスの暗号化を有効にしました</span><span class="sxs-lookup"><span data-stu-id="77658-138">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="77658-139">[重大な変更] `az storage account create and az storage account update` コマンドの `--encryption` オプションの名前を `--encryption-services` に変更しました</span><span class="sxs-lookup"><span data-stu-id="77658-139">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="77658-140">修正済み #4220: `az storage account update encryption` - 構文の不一致</span><span class="sxs-lookup"><span data-stu-id="77658-140">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="77658-141">VM</span><span class="sxs-lookup"><span data-stu-id="77658-141">VM</span></span>

* <span data-ttu-id="77658-142">`vmss get-instance-view` で `--instance-id *` を使用した場合に、余分な間違えた情報が表示される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77658-142">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="77658-143">`vmss create` に `--lb-sku` のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77658-143">Added support for `--lb-sku` to `vmss create`:</span></span> 
* <span data-ttu-id="77658-144">`[vm|vmss] create` の管理者名ブラックリストから人物名を削除しました</span><span class="sxs-lookup"><span data-stu-id="77658-144">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span> 
* <span data-ttu-id="77658-145">イメージからプラン情報を抽出できない場合に `[vm|vmss] create` がエラーをスローする問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77658-145">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="77658-146">内部 LB で vmms scaleset を作成するときのクラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="77658-146">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="77658-147">`vm availability-set create` で `--no-wait` 引数が機能しない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77658-147">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="77658-148">2017 年 8 月 15 日</span><span class="sxs-lookup"><span data-stu-id="77658-148">August 15, 2017</span></span>

<span data-ttu-id="77658-149">バージョン 2.0.14</span><span class="sxs-lookup"><span data-stu-id="77658-149">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="77658-150">ACS</span><span class="sxs-lookup"><span data-stu-id="77658-150">ACS</span></span>

* <span data-ttu-id="77658-151">kubernetes の sshMaster0 ポート番号を修正しました</span><span class="sxs-lookup"><span data-stu-id="77658-151">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="77658-152">Appservice</span><span class="sxs-lookup"><span data-stu-id="77658-152">Appservice</span></span>

* <span data-ttu-id="77658-153">新しい Git ベースの Linux Web アプリを作成するときの例外を修正しました</span><span class="sxs-lookup"><span data-stu-id="77658-153">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="77658-154">Event Grid</span><span class="sxs-lookup"><span data-stu-id="77658-154">Event Grid</span></span>

* <span data-ttu-id="77658-155">SDK 依存関係を追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-155">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="77658-156">2017 年 8 月 11 日</span><span class="sxs-lookup"><span data-stu-id="77658-156">August 11, 2017</span></span>

<span data-ttu-id="77658-157">バージョン 2.0.13</span><span class="sxs-lookup"><span data-stu-id="77658-157">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="77658-158">ACS</span><span class="sxs-lookup"><span data-stu-id="77658-158">ACS</span></span>

* <span data-ttu-id="77658-159">プレビュー リージョンを追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-159">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="77658-160">Batch
</span><span class="sxs-lookup"><span data-stu-id="77658-160">Batch</span></span>

* <span data-ttu-id="77658-161">Batch SDK 3.1.0 と Batch Management SDK 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="77658-161">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="77658-162">ジョブのタスク数を表示する新しいコマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-162">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="77658-163">リソース ファイルの SAS URL 処理のバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="77658-163">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="77658-164">Batch アカウントのエンドポイントで、オプションの "https://" プレフィックスがサポートされるようになりました</span><span class="sxs-lookup"><span data-stu-id="77658-164">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="77658-165">ジョブに対する 100 を超えるタスクのリストの追加をサポートします</span><span class="sxs-lookup"><span data-stu-id="77658-165">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="77658-166">拡張機能コマンド モジュールの読み込みのデバッグ ログを追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-166">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="77658-167">コンポーネント</span><span class="sxs-lookup"><span data-stu-id="77658-167">Component</span></span>

* <span data-ttu-id="77658-168">"az component" コマンドに非推奨警告を追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-168">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="77658-169">コンテナー</span><span class="sxs-lookup"><span data-stu-id="77658-169">Container</span></span>

* <span data-ttu-id="77658-170">`create`: 環境変数内で等号を使用できない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77658-170">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="77658-171">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="77658-171">Data Lake Store</span></span>

* <span data-ttu-id="77658-172">プログレス コントロールを有効にしました</span><span class="sxs-lookup"><span data-stu-id="77658-172">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="77658-173">Event Grid</span><span class="sxs-lookup"><span data-stu-id="77658-173">Event Grid</span></span>

* <span data-ttu-id="77658-174">最初のリリース</span><span class="sxs-lookup"><span data-stu-id="77658-174">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="77658-175">ネットワーク</span><span class="sxs-lookup"><span data-stu-id="77658-175">Network</span></span>

* <span data-ttu-id="77658-176">`lb`: 特定の子リソース名が省略された場合に正しく解決されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77658-176">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="77658-177">`application-gateway {subresource} delete`: `--no-wait` が受け入れられない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77658-177">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="77658-178">`application-gateway http-settings update`: `--connection-draining-timeout` を無効にできない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77658-178">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="77658-179">`az network vpn-connection ipsec-policy add` での予期しないキーワード引数 `sa_data_size_kilobyes` のエラーを修正しました</span><span class="sxs-lookup"><span data-stu-id="77658-179">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="77658-180">プロファイル</span><span class="sxs-lookup"><span data-stu-id="77658-180">Profile</span></span>

* <span data-ttu-id="77658-181">`account list`: サーバーの最新のサブスクリプションを同期する `--refresh` を追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-181">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="77658-182">Storage</span><span class="sxs-lookup"><span data-stu-id="77658-182">Storage</span></span>

* <span data-ttu-id="77658-183">システムによって割り当てられた ID によるストレージ アカウントの更新を有効にします</span><span class="sxs-lookup"><span data-stu-id="77658-183">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="77658-184">VM</span><span class="sxs-lookup"><span data-stu-id="77658-184">VM</span></span>

* <span data-ttu-id="77658-185">`availability-set`: 変換時の障害ドメイン数を公開しました</span><span class="sxs-lookup"><span data-stu-id="77658-185">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="77658-186">`list-skus` コマンドを公開しました</span><span class="sxs-lookup"><span data-stu-id="77658-186">Exposed `list-skus` command</span></span>
* <span data-ttu-id="77658-187">ロールの割り当てを作成しない ID の割り当てをサポートします</span><span class="sxs-lookup"><span data-stu-id="77658-187">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="77658-188">データ ディスクのアタッチ時にストレージ SKU を適用します</span><span class="sxs-lookup"><span data-stu-id="77658-188">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="77658-189">管理ディスクを使用する場合の既定の os-disk 名とストレージ SKU を削除しました</span><span class="sxs-lookup"><span data-stu-id="77658-189">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="77658-190">2017 年 7 月 28 日</span><span class="sxs-lookup"><span data-stu-id="77658-190">July 28, 2017</span></span>

<span data-ttu-id="77658-191">バージョン 2.0.12</span><span class="sxs-lookup"><span data-stu-id="77658-191">Version 2.0.12</span></span>

* <span data-ttu-id="77658-192">コンテナー コマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-192">Added container commands</span></span>
* <span data-ttu-id="77658-193">請求および使用量モジュールを追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-193">Added billing and consumption modules</span></span>

```
azure-cli (2.0.12)  

acr (2.0.9)  
acs (2.0.11)  
appservice (0.1.11)  
batch (3.0.3)  
billing (0.1.3)  
cdn (0.0.6)  
cloud (2.0.7)  
cognitiveservices (0.1.6)  
command-modules-nspkg (2.0.1)  
component (2.0.6)  
configure (2.0.10)  
consumption (0.1.3)  
container (0.1.7)  
core (2.0.12)  
cosmosdb (0.1.11)  
dla (0.0.10)  
dls (0.0.11)  
feedback (2.0.6)  
find (0.2.6)  
interactive (0.3.7)  
iot (0.1.10)  
keyvault (2.0.8)  
lab (0.0.9)  
monitor (0.0.8)  
network (2.0.11)  
nspkg (3.0.1)  
profile (2.0.9)  
rdbms (0.0.5)  
redis (0.2.7)  
resource (2.0.11)  
role (2.0.9)  
sf (1.0.5)  
sql (2.0.8)  
storage (2.0.11)  
vm (2.0.11) 
```

### <a name="core"></a><span data-ttu-id="77658-194">コア</span><span class="sxs-lookup"><span data-stu-id="77658-194">Core</span></span>

* <span data-ttu-id="77658-195">サービス プリンシパルの SDK 認証情報と証明書を出力します</span><span class="sxs-lookup"><span data-stu-id="77658-195">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="77658-196">デプロイの進行状況の例外を修正しました</span><span class="sxs-lookup"><span data-stu-id="77658-196">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="77658-197">サブスクリプション クライアントを作成するために、現在のクラウドの ARM エンドポイントを使用します</span><span class="sxs-lookup"><span data-stu-id="77658-197">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="77658-198">clouds.config ファイルの同時処理機能が向上しました (#3636)</span><span class="sxs-lookup"><span data-stu-id="77658-198">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="77658-199">コマンド実行のたびにクライアント要求 ID を更新します</span><span class="sxs-lookup"><span data-stu-id="77658-199">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="77658-200">正しい SDK プロファイルでサブスクリプション クライアントを作成します (#3635)</span><span class="sxs-lookup"><span data-stu-id="77658-200">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="77658-201">テンプレート デプロイの進行状況レポート (#3510)</span><span class="sxs-lookup"><span data-stu-id="77658-201">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="77658-202">jmespath クエリを通じてテーブル出力フィールドを選択するサポートを追加しました (#3581)</span><span class="sxs-lookup"><span data-stu-id="77658-202">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="77658-203">解析引数のミュートを改善し、ジェスチャによる履歴を追加しました (#3434)</span><span class="sxs-lookup"><span data-stu-id="77658-203">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="77658-204">正しい SDK プロファイルでサブスクリプション クライアントを作成します</span><span class="sxs-lookup"><span data-stu-id="77658-204">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="77658-205">すべての既存のレコーディング ファイルを最新のフォルダーに移動します</span><span class="sxs-lookup"><span data-stu-id="77658-205">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="77658-206">VM/VMSS 作成のべき等を修正しました (#3586)</span><span class="sxs-lookup"><span data-stu-id="77658-206">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="77658-207">コマンド パスで大文字と小文字が区別されなくなりました</span><span class="sxs-lookup"><span data-stu-id="77658-207">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="77658-208">特定のブール型パラメーターで大文字と小文字が区別されなくなりました</span><span class="sxs-lookup"><span data-stu-id="77658-208">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="77658-209">Azure Stack のような ADFS オンプレミス サーバーへのログインをサポートします</span><span class="sxs-lookup"><span data-stu-id="77658-209">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="77658-210">clouds.config への同時書き込みを修正しました (#3255)</span><span class="sxs-lookup"><span data-stu-id="77658-210">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="77658-211">ACR</span><span class="sxs-lookup"><span data-stu-id="77658-211">ACR</span></span>

* <span data-ttu-id="77658-212">管理対象レジストリ用の `show-usage` コマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-212">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="77658-213">管理対象レジストリの SKU 更新をサポートします</span><span class="sxs-lookup"><span data-stu-id="77658-213">Support SKU update for managed registries</span></span>
* <span data-ttu-id="77658-214">管理対象レジストリと管理 SKU を追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-214">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="77658-215">管理対象レジストリの webhook と acr webhook コマンド モジュールを追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-215">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="77658-216">AAD 認証と acr login コマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-216">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="77658-217">Docker リポジトリ、マニフェスト、タグ用の delete コマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-217">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="77658-218">ACS</span><span class="sxs-lookup"><span data-stu-id="77658-218">ACS</span></span>

* <span data-ttu-id="77658-219">API バージョン 2017-07-01 をサポートします</span><span class="sxs-lookup"><span data-stu-id="77658-219">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="77658-220">Appservice</span><span class="sxs-lookup"><span data-stu-id="77658-220">Appservice</span></span>

* <span data-ttu-id="77658-221">Linux Web アプリの一覧表示で何も返されないバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="77658-221">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="77658-222">acr からの資格情報の取得をサポートします</span><span class="sxs-lookup"><span data-stu-id="77658-222">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="77658-223">`appservice web` のすべてのコマンドを削除します</span><span class="sxs-lookup"><span data-stu-id="77658-223">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="77658-224">コマンド出力で Docker レジストリのパスワードをマスクします (#3656)</span><span class="sxs-lookup"><span data-stu-id="77658-224">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="77658-225">macOS でエラーにならずに既定のブラウザーが使用されます (#3623)</span><span class="sxs-lookup"><span data-stu-id="77658-225">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="77658-226">`webapp log tail` と `webapp log download` のヘルプを改善します (#3624)</span><span class="sxs-lookup"><span data-stu-id="77658-226">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="77658-227">静的ルーティングを構成するための `traffic-routing` コマンドを公開しました (#3566)</span><span class="sxs-lookup"><span data-stu-id="77658-227">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="77658-228">ソース管理の構成で信頼性のための修正が追加されました (#3245)</span><span class="sxs-lookup"><span data-stu-id="77658-228">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="77658-229">Windows Web アプリ用の `webapp config update` から、サポートされていない `--node-version` 引数を削除しました。</span><span class="sxs-lookup"><span data-stu-id="77658-229">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="77658-230">代わりに `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...` を使用してください</span><span class="sxs-lookup"><span data-stu-id="77658-230">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="77658-231">Batch
</span><span class="sxs-lookup"><span data-stu-id="77658-231">Batch</span></span>

* <span data-ttu-id="77658-232">Batch SDK 3.0.0 に更新して、プール内の優先度が低い VM がサポートされるようにしました</span><span class="sxs-lookup"><span data-stu-id="77658-232">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="77658-233">`pool create` のオプション `--target-dedicated` の名前を `--target-dedicated-nodes` に変更しました</span><span class="sxs-lookup"><span data-stu-id="77658-233">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="77658-234">`pool create` のオプションの `--target-low-priority-nodes` と `--application-licenses` を追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-234">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="77658-235">CDN</span><span class="sxs-lookup"><span data-stu-id="77658-235">CDN</span></span>

* <span data-ttu-id="77658-236">`--profile-name` によって指定されたプロファイルが存在しない場合に表示される `cdn endpoint list` のエラー メッセージを、より適切な内容に変更しました。</span><span class="sxs-lookup"><span data-stu-id="77658-236">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="77658-237">クラウド</span><span class="sxs-lookup"><span data-stu-id="77658-237">Cloud</span></span>

* <span data-ttu-id="77658-238">クラウド メタデータ エンドポイントの API バージョンを YYYY-MM-DD 形式に変更しました</span><span class="sxs-lookup"><span data-stu-id="77658-238">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="77658-239">ギャラリー エンドポイントは必須ではありません</span><span class="sxs-lookup"><span data-stu-id="77658-239">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="77658-240">ARM リソース マネージャー エンドポイントだけでのクラウドの登録をサポートします</span><span class="sxs-lookup"><span data-stu-id="77658-240">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="77658-241">`cloud set` で現在のクラウドを選択するときにプロファイルを選択できるオプションを提供しました</span><span class="sxs-lookup"><span data-stu-id="77658-241">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="77658-242">`endpoint_vm_image_alias_doc` を公開しました</span><span class="sxs-lookup"><span data-stu-id="77658-242">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="77658-243">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="77658-243">CosmosDB</span></span>

* <span data-ttu-id="77658-244">カスタム パーティション キーでコレクションを作成できるように修正しました</span><span class="sxs-lookup"><span data-stu-id="77658-244">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="77658-245">既定のコレクション TTL のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77658-245">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="77658-246">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="77658-246">Data Lake Analytics</span></span>

* <span data-ttu-id="77658-247">コンピューティング ポリシー管理用のコマンドを `dla account compute-policy` 見出しの下に追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-247">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="77658-248">`dla job pipeline show` を追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-248">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="77658-249">`dla job recurrence list` を追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-249">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="77658-250">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="77658-250">Data Lake Store</span></span>

* <span data-ttu-id="77658-251">ユーザー管理のキー コンテナーのキー ローテーションのサポートを `dls account update` に追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-251">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="77658-252">基になる Data Lake Store ファイル システム SDK のバージョンを更新して、パフォーマンスの問題に対応しました</span><span class="sxs-lookup"><span data-stu-id="77658-252">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="77658-253">コマンド `dls enable-key-vault` を追加しました。</span><span class="sxs-lookup"><span data-stu-id="77658-253">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="77658-254">このコマンドでは、Data Lake Store アカウント内でデータの暗号化を使用するために、ユーザー指定のキー コンテナーの有効化が試行されます</span><span class="sxs-lookup"><span data-stu-id="77658-254">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="77658-255">対話</span><span class="sxs-lookup"><span data-stu-id="77658-255">Interactive</span></span>

* <span data-ttu-id="77658-256">キャッシュされたコマンドを使用することで、起動時間が向上しました</span><span class="sxs-lookup"><span data-stu-id="77658-256">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="77658-257">テスト カバレッジが増えました</span><span class="sxs-lookup"><span data-stu-id="77658-257">Increased test coverage</span></span>
* <span data-ttu-id="77658-258">"?" ジェスチャが次のコマンドにも挿入されるよう強化しました</span><span class="sxs-lookup"><span data-stu-id="77658-258">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="77658-259">プロファイル 2017-03-09-profile-preview との対話エラーを修正しました (#3587)</span><span class="sxs-lookup"><span data-stu-id="77658-259">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="77658-260">`--version` を対話モードのパラメーターとして使用できるようにしました (#3645)</span><span class="sxs-lookup"><span data-stu-id="77658-260">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="77658-261">対話モードで検証の完了時にエラーがスローされないようにします (#3570)</span><span class="sxs-lookup"><span data-stu-id="77658-261">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="77658-262">テンプレート デプロイの進行状況レポート (#3510)</span><span class="sxs-lookup"><span data-stu-id="77658-262">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="77658-263">`--progress` フラグを追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-263">Added `--progress` flag</span></span>
* <span data-ttu-id="77658-264">入力候補から `--debug` と `--verbose` を削除しました</span><span class="sxs-lookup"><span data-stu-id="77658-264">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="77658-265">入力候補から `interactive` を削除しました (#3324)</span><span class="sxs-lookup"><span data-stu-id="77658-265">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="77658-266">IoT</span><span class="sxs-lookup"><span data-stu-id="77658-266">IoT</span></span>

* <span data-ttu-id="77658-267">ポリシーの作成で既存のポリシーが消去されないように修正しました。</span><span class="sxs-lookup"><span data-stu-id="77658-267">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="77658-268">(#3934)</span><span class="sxs-lookup"><span data-stu-id="77658-268">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="77658-269">Key Vault</span><span class="sxs-lookup"><span data-stu-id="77658-269">Key vault</span></span>

* <span data-ttu-id="77658-270">キー コンテナーの回復機能のために、以下のコマンドを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77658-270">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="77658-271">`keyvault` サブコマンドの `purge`、`recover`、`keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="77658-271">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="77658-272">`keyvault secret` サブコマンドの `backup`、`restore`、`purge`、`recover`、`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="77658-272">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="77658-273">`keyvault certificate` サブコマンドの `purge`、`recover`、`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="77658-273">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="77658-274">`keyvault key` サブコマンドの `purge`、`recover`、`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="77658-274">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="77658-275">サービス プリンシパルのキー コンテナーの統合を追加しました (#3133)</span><span class="sxs-lookup"><span data-stu-id="77658-275">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="77658-276">キー コンテナー データプレーンを 0.3.2 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="77658-276">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="77658-277">(#3307)</span><span class="sxs-lookup"><span data-stu-id="77658-277">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="77658-278">ラボ</span><span class="sxs-lookup"><span data-stu-id="77658-278">Lab</span></span>

* <span data-ttu-id="77658-279">`az lab vm claim` を通じてラボ内の任意の VM を要求するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-279">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="77658-280">`az lab vm list` と `az lab vm show` のテーブル出力フォーマッタを追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-280">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="77658-281">監視</span><span class="sxs-lookup"><span data-stu-id="77658-281">Monitor</span></span>

* <span data-ttu-id="77658-282">`monitor autoscale-settings get-parameters-template` コマンドのテンプレート ファイルを修正しました (#3349)</span><span class="sxs-lookup"><span data-stu-id="77658-282">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="77658-283">`monitor alert-rule-incidents list` の名前を `monitor alert list-incidents` に変更しました</span><span class="sxs-lookup"><span data-stu-id="77658-283">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="77658-284">`monitor alert-rule-incidents show` の名前を `monitor alert show-incident` に変更しました</span><span class="sxs-lookup"><span data-stu-id="77658-284">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="77658-285">`monitor metric-defintions list` の名前を `monitor metrics list-definitions` に変更しました</span><span class="sxs-lookup"><span data-stu-id="77658-285">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="77658-286">`monitor alert-rules` の名前を `monitor alert` に変更しました</span><span class="sxs-lookup"><span data-stu-id="77658-286">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="77658-287">`monitor alert create` を次のように変更しました。</span><span class="sxs-lookup"><span data-stu-id="77658-287">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="77658-288">`condition` および `action` サブコマンドが JSON を受け入れなくなりました</span><span class="sxs-lookup"><span data-stu-id="77658-288">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="77658-289">ルール作成プロセスを簡略化するために多数のパラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="77658-289">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="77658-290">`location` が必須ではなくなりました</span><span class="sxs-lookup"><span data-stu-id="77658-290">`location` no longer required</span></span>
  * <span data-ttu-id="77658-291">ターゲットの名前と ID のサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="77658-291">Add name and ID support for target</span></span>
  * <span data-ttu-id="77658-292">`--alert-rule-resource-name` を削除します</span><span class="sxs-lookup"><span data-stu-id="77658-292">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="77658-293">`is-enabled` の名前を `enabled` に変更し、省略可能にしました</span><span class="sxs-lookup"><span data-stu-id="77658-293">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="77658-294">`description` の既定値が、指定された条件に基づいて設定されるようになりました</span><span class="sxs-lookup"><span data-stu-id="77658-294">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="77658-295">新しい形式をわかりやすく示すための例を追加します</span><span class="sxs-lookup"><span data-stu-id="77658-295">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="77658-296">`monitor metric` コマンドの名前または ID をサポートします</span><span class="sxs-lookup"><span data-stu-id="77658-296">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="77658-297">`monitor alert rule update` に便利な引数と例を追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-297">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="77658-298">ネットワーク</span><span class="sxs-lookup"><span data-stu-id="77658-298">Network</span></span>

* <span data-ttu-id="77658-299">`list-private-access-services` コマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-299">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="77658-300">`--private-access-services` 引数を `vnet subnet create` と `vnet subnet update` に追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-300">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="77658-301">`application-gateway redirect-config create` が失敗する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77658-301">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="77658-302">`application-gateway redirect-config update` で `--no-wait` を指定しても機能しない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77658-302">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="77658-303">`application-gateway address-pool create` と `application-gateway address-pool update` で `--servers` 引数を使用する場合のバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="77658-303">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="77658-304">`application-gateway redirect-config` コマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-304">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="77658-305">`list-options`、`predefined list`、`predefined show` の各コマンドを `application-gateway ssl-policy` に追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-305">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="77658-306">`--name`、`--cipher-suites`、`--min-protocol-version` の各引数を `application-gateway ssl-policy set` に追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-306">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="77658-307">`--host-name-from-backend-pool`、`--affinity-cookie-name`、`--enable-probe`、`--path` の各引数を `application-gateway http-settings create` と `application-gateway http-settings update` に追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-307">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="77658-308">`--default-redirect-config` 引数と `--redirect-config` 引数を `application-gateway url-path-map create` と `application-gateway url-path-map update` に追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-308">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="77658-309">`--redirect-config` 引数を `application-gateway url-path-map rule create` に追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-309">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="77658-310">`--no-wait` のサポートを `application-gateway url-path-map rule delete` に追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-310">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="77658-311">`--host-name-from-http-settings`、`--min-servers`、`--match-body`、`--match-status-codes` の各引数を `application-gateway probe create` と `application-gateway probe update` に追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-311">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="77658-312">`--redirect-config` 引数を `application-gateway rule create` と `application-gateway rule update` に追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-312">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="77658-313">`--accelerated-networking` のサポートを `nic create` と `nic update` に追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-313">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="77658-314">`nic create` から `--internal-dns-name-suffix` 引数を削除しました</span><span class="sxs-lookup"><span data-stu-id="77658-314">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="77658-315">`--dns-servers` のサポートを `nic update` と `nic create` に追加しました: --dns-servers のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-315">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="77658-316">`local-gateway create` で `--local-address-prefixes` が無視されるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="77658-316">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="77658-317">`--dns-servers` のサポートを `vnet update` に追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-317">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="77658-318">`express-route peering create` でルート フィルター処理をせずにピアリングを作成するときのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="77658-318">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="77658-319">`express-route update` で `--provider` および `--bandwidth` 引数が機能しないバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="77658-319">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="77658-320">`network watcher show-topology` の既定値設定ロジックのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="77658-320">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="77658-321">`network list-usages` の出力書式設定を改善しました</span><span class="sxs-lookup"><span data-stu-id="77658-321">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="77658-322">`application-gateway http-listener create` に既定のフロントエンド IP を使用します (1 つしかない場合)</span><span class="sxs-lookup"><span data-stu-id="77658-322">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="77658-323">`application-gateway rule create` に既定のアドレス プール、HTTP 設定、および HTTP リスナーを使用します (1 つしかない場合)</span><span class="sxs-lookup"><span data-stu-id="77658-323">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="77658-324">`lb rule create` に既定のフロントエンド IP およびバックエンド プールを使用します (1 つしかない場合)</span><span class="sxs-lookup"><span data-stu-id="77658-324">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="77658-325">`lb inbound-nat-rule create` に既定のフロントエンド IP を使用します (1 つしかない場合)</span><span class="sxs-lookup"><span data-stu-id="77658-325">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="77658-326">プロファイル</span><span class="sxs-lookup"><span data-stu-id="77658-326">Profile</span></span>

* <span data-ttu-id="77658-327">管理対象 ID での VM 内のログインをサポートします</span><span class="sxs-lookup"><span data-stu-id="77658-327">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="77658-328">`account show` で SDK 認証ファイル形式での出力をサポートします</span><span class="sxs-lookup"><span data-stu-id="77658-328">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="77658-329">"--expanded-view" を使用した場合に非推奨警告を表示します</span><span class="sxs-lookup"><span data-stu-id="77658-329">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="77658-330">生の AAD トークンを提供するための `get-access-token` コマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-330">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="77658-331">サブスクリプションが関連付けられていないユーザー アカウントでのログインをサポートします</span><span class="sxs-lookup"><span data-stu-id="77658-331">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="77658-332">RDBMS</span><span class="sxs-lookup"><span data-stu-id="77658-332">RDBMS</span></span>

* <span data-ttu-id="77658-333">サブスクリプション全体のサーバーの一覧表示をサポートします (#3417)</span><span class="sxs-lookup"><span data-stu-id="77658-333">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="77658-334">`% server_type` が見つからないために `%s` が処理されない問題を修正しました (#3393)</span><span class="sxs-lookup"><span data-stu-id="77658-334">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="77658-335">ドキュメント ソース マップを修正し、検証するための CI タスクを追加しました (#3361)</span><span class="sxs-lookup"><span data-stu-id="77658-335">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="77658-336">MySQL および PostgreSQL のヘルプを修正しました (#3369)</span><span class="sxs-lookup"><span data-stu-id="77658-336">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="77658-337">リソース</span><span class="sxs-lookup"><span data-stu-id="77658-337">Resource</span></span>

* <span data-ttu-id="77658-338">`group deployment create` の不足しているパラメーターの指定を求めるメッセージを改善しました</span><span class="sxs-lookup"><span data-stu-id="77658-338">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="77658-339">`--parameters KEY=VALUE` 構文の解析を改善しました</span><span class="sxs-lookup"><span data-stu-id="77658-339">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="77658-340">`group deployment create` のパラメーター ファイルが `@<file>` 構文で認識されなくなった問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77658-340">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="77658-341">`resource` および `managedapp` コマンドで `--ids` 引数をサポートします</span><span class="sxs-lookup"><span data-stu-id="77658-341">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="77658-342">いくつかの解析およびエラー メッセージを修正しました (#3584)</span><span class="sxs-lookup"><span data-stu-id="77658-342">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="77658-343">`<resource-namespace>` と `<resource-type>` を受け入れるよう、`lock` コマンドの `--resource-type` の解析を修正しました</span><span class="sxs-lookup"><span data-stu-id="77658-343">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="77658-344">テンプレート リンク テンプレートのパラメーター チェックを追加しました (#3629)</span><span class="sxs-lookup"><span data-stu-id="77658-344">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="77658-345">`KEY=VALUE` 構文でデプロイ パラメーターを指定するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-345">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="77658-346">役割</span><span class="sxs-lookup"><span data-stu-id="77658-346">Role</span></span>

* <span data-ttu-id="77658-347">`create-for-rbac` で SDK 認証ファイル形式での出力をサポートします</span><span class="sxs-lookup"><span data-stu-id="77658-347">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="77658-348">サービス プリンシパルを削除するときに、ロールの割り当てと、関連する AAD アプリケーションがクリーンアップされるようになりました (#3610)</span><span class="sxs-lookup"><span data-stu-id="77658-348">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="77658-349">`app create` の引数 `--start-date` および `--end-date` の説明に時刻形式を含めます</span><span class="sxs-lookup"><span data-stu-id="77658-349">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="77658-350">`--expanded-view` を使用した場合に非推奨警告を表示します</span><span class="sxs-lookup"><span data-stu-id="77658-350">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="77658-351">キー コンテナーの統合を `create-for-rbac` および `reset-credentials` コマンドに追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-351">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="77658-352">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="77658-352">Service Fabric</span></span>
* <span data-ttu-id="77658-353">アプリケーション内の大きなファイルがアップロード時に切り詰められる問題を修正しました (#3666)</span><span class="sxs-lookup"><span data-stu-id="77658-353">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="77658-354">Service Fabric コマンドのテストを追加しました (#3424)</span><span class="sxs-lookup"><span data-stu-id="77658-354">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="77658-355">多数の Service Fabric コマンドを修正しました (#3234)</span><span class="sxs-lookup"><span data-stu-id="77658-355">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="77658-356">SQL</span><span class="sxs-lookup"><span data-stu-id="77658-356">SQL</span></span>

* <span data-ttu-id="77658-357">壊れた `sql server create` `--identity` パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="77658-357">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="77658-358">`sql server create` および `sql server update` コマンドの出力からパスワード値を削除しました</span><span class="sxs-lookup"><span data-stu-id="77658-358">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="77658-359">`sql db list-editions` および `sql elastic-pool list-editions` コマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="77658-359">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="77658-360">Storage</span><span class="sxs-lookup"><span data-stu-id="77658-360">Storage</span></span>

* <span data-ttu-id="77658-361">`storage blob list`、`storage container list`、`storage share list` の各コマンドから `--marker` オプションを削除しました (#3745)</span><span class="sxs-lookup"><span data-stu-id="77658-361">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="77658-362">https 専用ストレージ アカウントの作成を有効にしました</span><span class="sxs-lookup"><span data-stu-id="77658-362">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="77658-363">storage metrics、logging、cors の各コマンドを更新しました (#3495)</span><span class="sxs-lookup"><span data-stu-id="77658-363">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="77658-364">CORS add からの例外メッセージを言い換えました (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="77658-364">Rephrased exception message from CORS add (#3638) (#3362)</span></span>  
* <span data-ttu-id="77658-365">ジェネレーターをドライ ラン モードのダウンロード バッチ コマンド内の一覧に変換しました (#3592)</span><span class="sxs-lookup"><span data-stu-id="77658-365">Converted generator to a list in download batch command dry run mode (#3592)</span></span> 
* <span data-ttu-id="77658-366">BLOB ダウンロード バッチのドライ ランの問題を修正しました (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="77658-366">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="77658-367">VM</span><span class="sxs-lookup"><span data-stu-id="77658-367">VM</span></span>

* <span data-ttu-id="77658-368">nsg の構成をサポートします</span><span class="sxs-lookup"><span data-stu-id="77658-368">Support configuring nsg</span></span>
* <span data-ttu-id="77658-369">DNS サーバーが正しく構成されないバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="77658-369">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="77658-370">管理対象のサービス ID をサポートします</span><span class="sxs-lookup"><span data-stu-id="77658-370">Support managed service identities</span></span>
* <span data-ttu-id="77658-371">既存のロード バランサーを使用する `cmss create` で `--backend-pool-name` が必要だった問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="77658-371">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="77658-372">`vm image create` で作成された datadisks の lun を 0 から開始します</span><span class="sxs-lookup"><span data-stu-id="77658-372">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="77658-373">2017 年 5 月 10 日</span><span class="sxs-lookup"><span data-stu-id="77658-373">May 10, 2017</span></span>

<span data-ttu-id="77658-374">バージョン 2.0.6</span><span class="sxs-lookup"><span data-stu-id="77658-374">Version 2.0.6</span></span>

* <span data-ttu-id="77658-375">documentdb から cosmosdb に名前が変更されました</span><span class="sxs-lookup"><span data-stu-id="77658-375">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="77658-376">rdbms (mysql、postgres) が追加されました</span><span class="sxs-lookup"><span data-stu-id="77658-376">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="77658-377">Data Lake Analytics モジュールと Data Lake Store モジュールが追加されました。</span><span class="sxs-lookup"><span data-stu-id="77658-377">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="77658-378">Cognitive Services モジュールが追加されました。</span><span class="sxs-lookup"><span data-stu-id="77658-378">Include Cognitive Services module.</span></span>
* <span data-ttu-id="77658-379">Service Fabric モジュールが追加されました。</span><span class="sxs-lookup"><span data-stu-id="77658-379">Include Service Fabric module.</span></span>
* <span data-ttu-id="77658-380">対話型モジュールが追加されました (az-shell の名前変更)。</span><span class="sxs-lookup"><span data-stu-id="77658-380">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="77658-381">CDN コマンドに対応するようになりました。</span><span class="sxs-lookup"><span data-stu-id="77658-381">Add support for CDN commands.</span></span>
* <span data-ttu-id="77658-382">コンテナー モジュールが削除されました。</span><span class="sxs-lookup"><span data-stu-id="77658-382">Remove Container module.</span></span>
* <span data-ttu-id="77658-383">"az --version" のショートカットとして "az -v" が追加されました ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="77658-383">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="77658-384">パッケージ読み込みとコマンド実行のパフォーマンスが向上しています ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="77658-384">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

```
azure-cli (2.0.6)

acr (2.0.4)
acs (2.0.6)
appservice (0.1.6)
batch (2.0.4)
cdn (0.0.2)
cloud (2.0.2)
cognitiveservices (0.1.2)
command-modules-nspkg (2.0.0)
component (2.0.4)
configure (2.0.6)
core (2.0.6)
cosmosdb (0.1.6)
dla (0.0.6)
dls (0.0.6)
feedback (2.0.2)
find (0.2.2)
interactive (0.3.1)
iot (0.1.5)
keyvault (2.0.4)
lab (0.0.4)
monitor (0.0.4)
network (2.0.6)
nspkg (3.0.0)
profile (2.0.4)
rdbms (0.0.1)
redis (0.2.3)
resource (2.0.6)
role (2.0.4)
sf (1.0.1)
sql (2.0.3)
storage (2.0.6)
vm (2.0.6)
```

### <a name="core"></a><span data-ttu-id="77658-385">コア</span><span class="sxs-lookup"><span data-stu-id="77658-385">Core</span></span>

* <span data-ttu-id="77658-386">コア: 登録されていないプロバイダーによる例外がキャプチャされ、自動登録されます</span><span class="sxs-lookup"><span data-stu-id="77658-386">core: capture exceptions caused by unregistered provider and auto-register it</span></span>   
* <span data-ttu-id="77658-387">パフォーマンス: プロセスが終了するまで ADAL トークン キャッシュがメモリに保持されます ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="77658-387">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="77658-388">16 進フィンガープリント -o tsv から返されるバイトが修正されました ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="77658-388">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="77658-389">Key Vault 証明書ダウンロードの強化と AAD SP 統合 ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="77658-389">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="77658-390">Python の場所が "az —version" に追加されました ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="77658-390">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="77658-391">ログイン: サブスクリプションがないときのログインに対応するようになりました ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="77658-391">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="77658-392">コア: サービス プリンシパルを 2 回使用してログインするときのエラーが修正されました ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="77658-392">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="77658-393">コア: accessTokens.json のファイル パスを環境変数で構成できます ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="77658-393">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="77658-394">コア: 構成済み既定値を省略可能な引数に適用できます ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="77658-394">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="77658-395">コア: パフォーマンスの向上</span><span class="sxs-lookup"><span data-stu-id="77658-395">core: Improved performance</span></span>
* <span data-ttu-id="77658-396">コア: カスタム CA 証明書 - REQUESTS_CA_BUNDLE 環境変数の設定を利用できます</span><span class="sxs-lookup"><span data-stu-id="77658-396">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="77658-397">コア: クラウド構成 - "管理" エンドポイントが設定されていない場合に、"リソース マネージャー" エンドポイントが使用されます</span><span class="sxs-lookup"><span data-stu-id="77658-397">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="77658-398">ACS</span><span class="sxs-lookup"><span data-stu-id="77658-398">ACS</span></span>

* <span data-ttu-id="77658-399">マスター数とエージェント数が文字列から整数に修正されました</span><span class="sxs-lookup"><span data-stu-id="77658-399">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="77658-400">非同期作成用に "az acs create --no-wait" と "az acs wait" が公開されました</span><span class="sxs-lookup"><span data-stu-id="77658-400">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="77658-401">ドライラン検証用に "az acs create --validate" が公開されました</span><span class="sxs-lookup"><span data-stu-id="77658-401">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="77658-402">スケール コマンドの PUT 呼び出しの前の Windows プロファイルが削除されます ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="77658-402">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="77658-403">AppService</span><span class="sxs-lookup"><span data-stu-id="77658-403">AppService</span></span>

* <span data-ttu-id="77658-404">関数アプリ: 作成、表示、リスト、削除、ホスト名、SSL など、関数アプリに完全に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="77658-404">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="77658-405">Team Services (VSTS) が継続的な配信オプションとして "appservice web source-control config" に追加されました</span><span class="sxs-lookup"><span data-stu-id="77658-405">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="77658-406">"az webapp" が作成され "az app service web" が置き換えられています (下位互換性のために "az app service web" は 2 リリースだけ保持されます)</span><span class="sxs-lookup"><span data-stu-id="77658-406">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="77658-407">WebApp 作成時にデプロイと "ランタイム スタック" を構成するための引数が公開されました</span><span class="sxs-lookup"><span data-stu-id="77658-407">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="77658-408">"webapp list-runtimes" が公開されました</span><span class="sxs-lookup"><span data-stu-id="77658-408">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="77658-409">接続文字列の構成がサポートされています ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="77658-409">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="77658-410">プレビューでのスロット スワップがサポートされています</span><span class="sxs-lookup"><span data-stu-id="77658-410">support slot swap with preview</span></span>
* <span data-ttu-id="77658-411">appservice コマンドからのポーランド語のエラー ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="77658-411">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="77658-412">証明書の操作に App Service プランのリソース グループが使用されます ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="77658-412">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="77658-413">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="77658-413">CosmosDB</span></span>

* <span data-ttu-id="77658-414">documentdb モジュールから cosmosdb に名前が変更されました。</span><span class="sxs-lookup"><span data-stu-id="77658-414">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="77658-415">DocumentDB データプレーン API: データベースとコレクション管理に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="77658-415">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="77658-416">データベース アカウントにおける自動フェールオーバーの有効化に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="77658-416">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="77658-417">新しい一貫性ポリシー ConsistentPrefix に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="77658-417">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="77658-418">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="77658-418">Data Lake Analytics</span></span>

* <span data-ttu-id="77658-419">ジョブ リストの結果と状態に対するフィルター処理でエラーがスローされるバグが修正されました。</span><span class="sxs-lookup"><span data-stu-id="77658-419">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="77658-420">新しいカタログ項目の種類: パッケージに対応するようになりました。</span><span class="sxs-lookup"><span data-stu-id="77658-420">Add support for new catalog item type: package.</span></span> <span data-ttu-id="77658-421">`az dla catalog package` を介してアクセスされます</span><span class="sxs-lookup"><span data-stu-id="77658-421">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="77658-422">次のカタログ項目の一覧をデータベース内から表示できます (スキーマ仕様は不要です)。</span><span class="sxs-lookup"><span data-stu-id="77658-422">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="77658-423">テーブル</span><span class="sxs-lookup"><span data-stu-id="77658-423">Table</span></span>
  * <span data-ttu-id="77658-424">テーブル値関数</span><span class="sxs-lookup"><span data-stu-id="77658-424">Table valued function</span></span>
  * <span data-ttu-id="77658-425">表示</span><span class="sxs-lookup"><span data-stu-id="77658-425">View</span></span>
  * <span data-ttu-id="77658-426">テーブルの統計。</span><span class="sxs-lookup"><span data-stu-id="77658-426">Table Statistics.</span></span> <span data-ttu-id="77658-427">スキーマと一緒に表示することもできますが、テーブル名を指定する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="77658-427">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="77658-428">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="77658-428">Data Lake Store</span></span>

* <span data-ttu-id="77658-429">基になるファイルシステム SDK のバージョンが更新され、サーバー側スロットル処理への対応が強化されました。</span><span class="sxs-lookup"><span data-stu-id="77658-429">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="77658-430">パッケージ読み込みとコマンド実行のパフォーマンスが向上しています ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="77658-430">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="77658-431">access show のヘルプがなかったため、</span><span class="sxs-lookup"><span data-stu-id="77658-431">missed help for access show.</span></span> <span data-ttu-id="77658-432">追加しました </span><span class="sxs-lookup"><span data-stu-id="77658-432">adding it.</span></span> <span data-ttu-id="77658-433">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="77658-433">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="77658-434">検索</span><span class="sxs-lookup"><span data-stu-id="77658-434">Find</span></span>

* <span data-ttu-id="77658-435">検索結果を改善し、検索インデックスのバージョン管理を可能にしました</span><span class="sxs-lookup"><span data-stu-id="77658-435">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="77658-436">KeyVault</span><span class="sxs-lookup"><span data-stu-id="77658-436">KeyVault</span></span>

* <span data-ttu-id="77658-437">BC: `az keyvault certificate download` によって -e が文字列またはバイナリから PEM または DER に変更され、オプションの表現が向上しました</span><span class="sxs-lookup"><span data-stu-id="77658-437">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="77658-438">BC: --expires パラメーターと --not-before パラメーターはサービスでサポートされていないため、`keyvault certificate create` から削除されました。</span><span class="sxs-lookup"><span data-stu-id="77658-438">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="77658-439">--validity パラメーターが `keyvault certificate create` に追加され、--policy の値が選択的に上書きされます</span><span class="sxs-lookup"><span data-stu-id="77658-439">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="77658-440">"expires" と "not_before" が公開され、"validity_in_months" が公開されなかった場合に `keyvault certificate get-default-policy` で発生する問題が修正されました。</span><span class="sxs-lookup"><span data-stu-id="77658-440">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="77658-441">KeyVault における pem と pfx のインポートが修正されました ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="77658-441">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="77658-442">ラボ</span><span class="sxs-lookup"><span data-stu-id="77658-442">Lab</span></span>

* <span data-ttu-id="77658-443">ラボ環境用の作成、表示、削除、およびリスト コマンドが追加されました。</span><span class="sxs-lookup"><span data-stu-id="77658-443">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="77658-444">ラボで ARM テンプレートを表示するための表示およびリスト コマンドが追加されました。</span><span class="sxs-lookup"><span data-stu-id="77658-444">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="77658-445">ラボ環境で VM をフィルター処理するための --environment フラグが `az lab vm list` に追加されました。</span><span class="sxs-lookup"><span data-stu-id="77658-445">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="77658-446">ラボの数式内でアーティファクト スキャフォールディングをエクスポートするための便利なコマンド `az lab formula export-artifacts` が追加されました。</span><span class="sxs-lookup"><span data-stu-id="77658-446">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="77658-447">ラボ内でシークレットを管理するためのコマンドが追加されました。</span><span class="sxs-lookup"><span data-stu-id="77658-447">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="77658-448">監視</span><span class="sxs-lookup"><span data-stu-id="77658-448">Monitor</span></span>

* <span data-ttu-id="77658-449">バグの修正: JSON 文字列を使用するため `az alert-rules create` の `--actions` がモデル化されています ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="77658-449">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="77658-450">バグの修正: diagnostic settings create が、表示コマンドからのログ/メトリックを受け付けません ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="77658-450">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="77658-451">ネットワーク</span><span class="sxs-lookup"><span data-stu-id="77658-451">Network</span></span>

* <span data-ttu-id="77658-452">`network watcher test-connectivity` コマンドが追加されました。</span><span class="sxs-lookup"><span data-stu-id="77658-452">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="77658-453">`network watcher packet-capture create` の `--filters` パラメーターに対応するようになりました。</span><span class="sxs-lookup"><span data-stu-id="77658-453">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="77658-454">Application Gateway 接続のドレインに対応するようになりました。</span><span class="sxs-lookup"><span data-stu-id="77658-454">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="77658-455">Application Gateway WAF 規則セットの構成に対応するようになりました。</span><span class="sxs-lookup"><span data-stu-id="77658-455">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="77658-456">ExpressRoute ルート フィルターとルールに対応するようになりました。</span><span class="sxs-lookup"><span data-stu-id="77658-456">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="77658-457">TrafficManager の地理的なルーティングに対応するようになりました。</span><span class="sxs-lookup"><span data-stu-id="77658-457">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="77658-458">VPN 接続ポリシー ベースのトラフィック セレクターに対応するようになりました。</span><span class="sxs-lookup"><span data-stu-id="77658-458">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="77658-459">VPN 接続 IPSec ポリシーに対応するようになりました。</span><span class="sxs-lookup"><span data-stu-id="77658-459">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="77658-460">`--no-wait` パラメーターまたは `--validate` パラメーターを使用するときの `vpn-connection create` のバグが修正されました。</span><span class="sxs-lookup"><span data-stu-id="77658-460">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="77658-461">アクティブ/アクティブ VNet ゲートウェイに対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="77658-461">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="77658-462">`network vpn-connection list/show` コマンドの出力から null 値が削除されました。</span><span class="sxs-lookup"><span data-stu-id="77658-462">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="77658-463">BC: `vpn-connection create` の出力のバグが修正されました</span><span class="sxs-lookup"><span data-stu-id="77658-463">BC: Fix bug in the output of `vpn-connection create`</span></span> 
* <span data-ttu-id="77658-464">"vpn-connection create" の "--key-length" 引数が適切に解析されないバグが修正されました。</span><span class="sxs-lookup"><span data-stu-id="77658-464">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="77658-465">`dns zone import` でレコードが適切にインポートされないバグが修正されました。</span><span class="sxs-lookup"><span data-stu-id="77658-465">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="77658-466">`traffic-manager endpoint update` が動作しないバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="77658-466">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="77658-467">"Network Watcher" プレビューのコマンドが追加されました。</span><span class="sxs-lookup"><span data-stu-id="77658-467">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="77658-468">プロファイル</span><span class="sxs-lookup"><span data-stu-id="77658-468">Profile</span></span>

* <span data-ttu-id="77658-469">サブスクリプションが見つからないときのログインに対応するようになりました ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="77658-469">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="77658-470">az account set --subscription で短いパラメーター名に対応するようになりました ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="77658-470">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="77658-471">Redis</span><span class="sxs-lookup"><span data-stu-id="77658-471">Redis</span></span>

* <span data-ttu-id="77658-472">Redis Cache のスケール機能も追加する更新コマンドが追加されました</span><span class="sxs-lookup"><span data-stu-id="77658-472">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="77658-473">"update-settings" コマンドが廃止されました。</span><span class="sxs-lookup"><span data-stu-id="77658-473">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="77658-474">リソース</span><span class="sxs-lookup"><span data-stu-id="77658-474">Resource</span></span>

* <span data-ttu-id="77658-475">managedapp と managedapp の定義コマンドが追加されました ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="77658-475">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="77658-476">"provider operation" コマンドに対応するようになりました ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="77658-476">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="77658-477">汎用リソースの作成に対応するようになりました ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="77658-477">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="77658-478">リソース解析および API バージョンの検索が修正されました </span><span class="sxs-lookup"><span data-stu-id="77658-478">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="77658-479">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="77658-479">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="77658-480">az lock update のドキュメントが追加されました </span><span class="sxs-lookup"><span data-stu-id="77658-480">Add docs for az lock update.</span></span> <span data-ttu-id="77658-481">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="77658-481">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="77658-482">存在しないグループのリソースの一覧を表示しようとするとエラーが出力されます </span><span class="sxs-lookup"><span data-stu-id="77658-482">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="77658-483">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="77658-483">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="77658-484">[コンピューティング] VMSS と VM の可用性セットの更新に関する問題が修正されました。</span><span class="sxs-lookup"><span data-stu-id="77658-484">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="77658-485">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="77658-485">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="77658-486">parent-resource-path が None の場合のロックの作成と削除が修正されました ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="77658-486">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="77658-487">役割</span><span class="sxs-lookup"><span data-stu-id="77658-487">Role</span></span>

* <span data-ttu-id="77658-488">create-for-rbac: SP の終了日が、確実に証明書の有効期限の前に設定されます ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="77658-488">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="77658-489">RBAC: "ad group" が完全にサポートされるようになりました ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="77658-489">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="77658-490">ロール: ロール定義の更新に関する問題が修正されました ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="77658-490">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="77658-491">create-for-rbac: ユーザーによって指定されたパスワードが確実に取得されます</span><span class="sxs-lookup"><span data-stu-id="77658-491">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="77658-492">SQL</span><span class="sxs-lookup"><span data-stu-id="77658-492">SQL</span></span>

* <span data-ttu-id="77658-493">az sql server list-usages コマンドと az sql db list-usages コマンドが追加されました。</span><span class="sxs-lookup"><span data-stu-id="77658-493">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="77658-494">SQL - リソース プロバイダーに直接接続できます ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="77658-494">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="77658-495">Storage</span><span class="sxs-lookup"><span data-stu-id="77658-495">Storage</span></span>

* <span data-ttu-id="77658-496">`storage account create` のリソース グループの場所に対する既定の場所。</span><span class="sxs-lookup"><span data-stu-id="77658-496">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="77658-497">増分 BLOB コピーに対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="77658-497">Add support for incremental blob copy</span></span>
* <span data-ttu-id="77658-498">大きなブロック BLOB アップロードに対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="77658-498">Add support for large block blob upload</span></span>
* <span data-ttu-id="77658-499">アップロードするファイルが 200 GB を超える場合にブロック サイズが 100 MB に変更されます</span><span class="sxs-lookup"><span data-stu-id="77658-499">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="77658-500">VM</span><span class="sxs-lookup"><span data-stu-id="77658-500">VM</span></span>

* <span data-ttu-id="77658-501">avail-set: UD&FD ドメイン数が省略可能になりました</span><span class="sxs-lookup"><span data-stu-id="77658-501">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="77658-502">注: 独立したクラウドの VM コマンド。次の管理対象ディスク関連機能は避けるようにしてください。</span><span class="sxs-lookup"><span data-stu-id="77658-502">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="77658-503">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="77658-503">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="77658-504">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="77658-504">az vm/vmss disk</span></span>
  3. <span data-ttu-id="77658-505">"az vm/vmss create" 内では、"—use-unmanaged-disk" を使用して管理対象ディスクを回避します。他のコマンドは機能します</span><span class="sxs-lookup"><span data-stu-id="77658-505">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="77658-506">vm/vmss: SSH キー ペアを生成するときの警告テキストが向上します</span><span class="sxs-lookup"><span data-stu-id="77658-506">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="77658-507">vm/vmss: プラン情報を必要とするマーケットプレイス イメージからの作成をサポートします ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="77658-507">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="77658-508">2017 年 4 月 3 日</span><span class="sxs-lookup"><span data-stu-id="77658-508">April 3, 2017</span></span>

<span data-ttu-id="77658-509">バージョン 2.0.2</span><span class="sxs-lookup"><span data-stu-id="77658-509">Version 2.0.2</span></span>

<span data-ttu-id="77658-510">このリリースでは、ACR、Batch、KeyVault、SQL コンポーネントをリリースしました。</span><span class="sxs-lookup"><span data-stu-id="77658-510">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

```
azure-cli (2.0.2)
 
acr (2.0.0)
acs (2.0.2)
appservice (0.1.2)
batch (2.0.0)
cloud (2.0.0)
component (2.0.0)
configure (2.0.2)
container (0.1.2)
core (2.0.2)
documentdb (0.1.2)
feedback (2.0.0)
find (0.0.1b1)
iot (0.1.2)
keyvault (2.0.0)
lab (0.0.1)
monitor (0.0.1)
network (2.0.2)
nspkg (2.0.0)
profile (2.0.2)
redis (0.1.1b3)
resource (2.0.2)
role (2.0.1)
sql (2.0.0)
storage (2.0.2)
vm (2.0.2)
```

### <a name="core"></a><span data-ttu-id="77658-511">コア</span><span class="sxs-lookup"><span data-stu-id="77658-511">Core</span></span>

* <span data-ttu-id="77658-512">既定の一覧に acr、lab、monitor、find モジュールを追加。</span><span class="sxs-lookup"><span data-stu-id="77658-512">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="77658-513">ログイン: 誤ったテナントをスキップ ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="77658-513">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="77658-514">ログイン: 既定のサブスクリプションを "Enabled" の状態のサブスクリプションに設定 ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="77658-514">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="77658-515">wait コマンドと --no-wait のサポートをより多くのコマンドに追加 ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="77658-515">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="77658-516">コア: 証明書を持つサービス プリンシパルを使用したログインをサポート ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="77658-516">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="77658-517">不足しているテンプレート パラメーターの指定を求めるメッセージを追加 </span><span class="sxs-lookup"><span data-stu-id="77658-517">Add prompting for missing template parameters.</span></span> <span data-ttu-id="77658-518">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="77658-518">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="77658-519">既定のリソース グループ、既定の Web、既定の VM など、一般的な引数の既定値の設定をサポート</span><span class="sxs-lookup"><span data-stu-id="77658-519">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="77658-520">特定のテナントへのログインをサポート</span><span class="sxs-lookup"><span data-stu-id="77658-520">Support login to specific tenant</span></span>
 
### <a name="acs"></a><span data-ttu-id="77658-521">ACS</span><span class="sxs-lookup"><span data-stu-id="77658-521">ACS</span></span>

* <span data-ttu-id="77658-522">[ACS] 既定の ACS クラスターを構成するためのサポートを追加 ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="77658-522">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="77658-523">ssh キー パスワードの入力要求のサポートを追加 </span><span class="sxs-lookup"><span data-stu-id="77658-523">Add support for ssh key password prompting.</span></span> <span data-ttu-id="77658-524">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="77658-524">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="77658-525">Windows クラスターのためのサポートを追加 </span><span class="sxs-lookup"><span data-stu-id="77658-525">Add support for windows clusters.</span></span> <span data-ttu-id="77658-526">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="77658-526">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="77658-527">所有者から共同作成者へのロールの切り替え </span><span class="sxs-lookup"><span data-stu-id="77658-527">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="77658-528">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="77658-528">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>
 
### <a name="appservice"></a><span data-ttu-id="77658-529">AppService</span><span class="sxs-lookup"><span data-stu-id="77658-529">AppService</span></span>

* <span data-ttu-id="77658-530">appservice: DNS A レコードで使用される外部 IP アドレスの取得をサポート ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="77658-530">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="77658-531">appservice: ワイルドカード証明書のバインドをサポート ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="77658-531">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="77658-532">appservice: 発行プロファイルの一覧表示をサポート ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="77658-532">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="77658-533">AppService - 構成後にソース管理の同期をトリガー ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="77658-533">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>
 
### <a name="datalake"></a><span data-ttu-id="77658-534">DataLake</span><span class="sxs-lookup"><span data-stu-id="77658-534">DataLake</span></span>

* <span data-ttu-id="77658-535">Data Lake Analytics モジュールの最初のリリース。</span><span class="sxs-lookup"><span data-stu-id="77658-535">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="77658-536">Data Lake Store モジュールの最初のリリース。</span><span class="sxs-lookup"><span data-stu-id="77658-536">Initial release of Data Lake Store module.</span></span>
 
### <a name="docuemntdb"></a><span data-ttu-id="77658-537">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="77658-537">DocuemntDB</span></span>

* <span data-ttu-id="77658-538">DocumentDB: 接続文字列を一覧表示するためのサポートを追加 ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="77658-538">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="77658-539">VM</span><span class="sxs-lookup"><span data-stu-id="77658-539">VM</span></span>

* <span data-ttu-id="77658-540">[コンピューティング] 仮想マシン スケール セットを作成するための AppGateway サポートを追加 ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="77658-540">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="77658-541">[VM/VMSS] ディスク キャッシュのサポートを改善しました ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="77658-541">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="77658-542">VM/VMSS: ポータルで使用される資格情報検証ロジックを組み込む ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="77658-542">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="77658-543">wait コマンドと --no-wait のサポートを追加 ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="77658-543">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="77658-544">仮想マシン スケール セット: VM 間にわたるインスタンス ビューの一覧表示をサポート * ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="77658-544">Virtual machine scale set: support * to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="77658-545">VM と仮想マシン スケール セット用の --secrets を追加 ([#2212](https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="77658-545">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="77658-546">特殊化した VHD による VM 作成を許可 ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="77658-546">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="77658-547">2017 年 2 月 27 日</span><span class="sxs-lookup"><span data-stu-id="77658-547">February 27, 2017</span></span>

<span data-ttu-id="77658-548">バージョン 2.0.0</span><span class="sxs-lookup"><span data-stu-id="77658-548">Version 2.0.0</span></span>

<span data-ttu-id="77658-549">Azure CLI 2.0 のこのリリースは、最初の "一般公開" リリースです。</span><span class="sxs-lookup"><span data-stu-id="77658-549">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="77658-550">一般公開に該当するのは、以下のコマンド モジュールです。</span><span class="sxs-lookup"><span data-stu-id="77658-550">General availability applies to these command modules:</span></span>
- <span data-ttu-id="77658-551">コンテナー サービス (acs)</span><span class="sxs-lookup"><span data-stu-id="77658-551">Container Service (acs)</span></span>
- <span data-ttu-id="77658-552">コンピューティング (Resource Manager、VM、仮想マシン スケール セット、Managed Disks など)</span><span class="sxs-lookup"><span data-stu-id="77658-552">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="77658-553">ネットワーク</span><span class="sxs-lookup"><span data-stu-id="77658-553">Networking</span></span>
- <span data-ttu-id="77658-554">Storage</span><span class="sxs-lookup"><span data-stu-id="77658-554">Storage</span></span>

<span data-ttu-id="77658-555">これらのコマンド モジュールは、運用環境で使用することができ、標準の Microsoft SLA でサポートされています。</span><span class="sxs-lookup"><span data-stu-id="77658-555">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="77658-556">問題は、Microsoft サポートで直接開くことも、[github の問題一覧](https://github.com/azure/azure-cli/issues/)で開くこともできます。</span><span class="sxs-lookup"><span data-stu-id="77658-556">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="77658-557">[azure-cli タグを使用して StackOverflow](http://stackoverflow.com/questions/tagged/azure-cli) で質問したり、製品チーム ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)) に問い合わせたりすることもできます。`az feedback` コマンドを使用すると、コマンド ラインからフィードバックを送ることができます。</span><span class="sxs-lookup"><span data-stu-id="77658-557">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="77658-558">これらのモジュールのコマンドは安定しており、Azure CLI のこのバージョンの今後のリリースで構文が変更されることは想定されていません。</span><span class="sxs-lookup"><span data-stu-id="77658-558">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="77658-559">CLI のバージョンを確認するには、`az --version` を使用します。</span><span class="sxs-lookup"><span data-stu-id="77658-559">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="77658-560">出力では、CLI 自体のバージョン (このリリースでは 2.0.0)、個々のコマンド モジュール、および使用している Python と GCC のバージョンが示されます。</span><span class="sxs-lookup"><span data-stu-id="77658-560">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

```
azure-cli (2.0.0)

acs (2.0.0)
appservice (0.1.1b5)
batch (0.1.1b4)
cloud (2.0.0)
component (2.0.0)
configure (2.0.0)
container (0.1.1b4)
core (2.0.0)
documentdb (0.1.1b2)
feedback (2.0.0)
iot (0.1.1b3)
keyvault (0.1.1b5)
network (2.0.0)
nspkg (2.0.0)
profile (2.0.0)
redis (0.1.1b3)
resource (2.0.0)
role (2.0.0)
sql (0.1.1b5)
storage (2.0.0)
vm (2.0.0)
 
Python (Darwin) 2.7.10 (default, Jul 30 2016, 19:40:32) 
[GCC 4.2.1 Compatible Apple LLVM 8.0.0 (clang-800.0.34)]
```

> [!Note]
> <span data-ttu-id="77658-561">コマンド モジュールには、"b*n*" または "rc*n*" という接尾辞が付いているものがあります。</span><span class="sxs-lookup"><span data-stu-id="77658-561">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="77658-562">これらのコマンド モジュールはまだプレビュー段階であり、今後一般公開される予定です。</span><span class="sxs-lookup"><span data-stu-id="77658-562">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="77658-563">CLI のナイトリー プレビュー ビルドもあります。</span><span class="sxs-lookup"><span data-stu-id="77658-563">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="77658-564">詳細については、[ナイトリー ビルドの入手](https://github.com/Azure/azure-cli#nightly-builds)に関する手順と、[開発者向けセットアップおよび共同作成コード](https://github.com/Azure/azure-cli#developer-setup)に関する手順を参照してください。</span><span class="sxs-lookup"><span data-stu-id="77658-564">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="77658-565">ナイトリー プレビュー ビルドの問題は、次の方法で報告することができます。</span><span class="sxs-lookup"><span data-stu-id="77658-565">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="77658-566">[github の問題一覧](https://github.com/azure/azure-cli/issues/)で問題を報告する。</span><span class="sxs-lookup"><span data-stu-id="77658-566">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="77658-567">製品チーム ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)) に問い合わせる。</span><span class="sxs-lookup"><span data-stu-id="77658-567">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="77658-568">`az feedback` コマンドを使用してコマンド ラインからフィードバックを送る。</span><span class="sxs-lookup"><span data-stu-id="77658-568">Provide feedback from the command line with the `az feedback` command.</span></span>
