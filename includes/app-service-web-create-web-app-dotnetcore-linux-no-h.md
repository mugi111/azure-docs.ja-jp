---
title: インクルード ファイル
description: インクルード ファイル
services: app-service
author: cephalin
ms.service: app-service
ms.topic: include
ms.date: 08/06/2019
ms.author: cephalin
ms.custom: include file
ms.openlocfilehash: 2dc35727a82459750b4414b6e3eeddf28b31b718
ms.sourcegitcommit: 3073581d81253558f89ef560ffdf71db7e0b592b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/06/2019
ms.locfileid: "68824723"
---
`myAppServicePlan` App Service プランで [Web アプリ](../articles/app-service/containers/app-service-linux-intro.md)を作成します。 

Cloud Shell で、[`az webapp create`](/cli/azure/webapp?view=azure-cli-latest) コマンドを使用することができます。 次の例では、`<app-name>` をグローバルに一意のアプリ名に置き換えてください (有効な文字は `a-z`、`0-9`、`-`)。 ランタイムは `DOTNETCORE|2.2` に設定されています。 サポートされているすべてのランタイムを確認するには、[`az webapp list-runtimes --linux`](/cli/azure/webapp?view=azure-cli-latest) を実行します。 

```azurecli-interactive
# Bash
az webapp create --resource-group myResourceGroup --plan myAppServicePlan --name <app-name> --runtime "DOTNETCORE|2.2" --deployment-local-git
# PowerShell
az --% webapp create --resource-group myResourceGroup --plan myAppServicePlan --name <app-name> --runtime "DOTNETCORE|2.2" --deployment-local-git
```

Web アプリが作成されると、Azure CLI によって次の例のような出力が表示されます。

```json
Local git is configured with url of 'https://<username>@<app-name>.scm.azurewebsites.net/<app-name>.git'
{
  "availabilityState": "Normal",
  "clientAffinityEnabled": true,
  "clientCertEnabled": false,
  "cloningInfo": null,
  "containerSize": 0,
  "dailyMemoryTimeQuota": 0,
  "defaultHostName": "<app-name>.azurewebsites.net",
  "deploymentLocalGitUrl": "https://<username>@<app-name>.scm.azurewebsites.net/<app-name>.git",
  "enabled": true,
  < JSON data removed for brevity. >
}
```

Git デプロイを有効にして、空の Web アプリを Linux コンテナーに作成しました。

> [!NOTE]
> Git リモートの URL は `deploymentLocalGitUrl` プロパティに `https://<username>@<app-name>.scm.azurewebsites.net/<app-name>.git` 形式で出力されます。 この URL は後で必要になるので保存しておいてください。
>
