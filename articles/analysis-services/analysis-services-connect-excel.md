---
title: Excel で Azure Analysis Services に接続する | Microsoft Docs
description: Azure Analysis Services サーバーに Excel を使って接続する方法を説明します。 接続されたら、ユーザーはピボットテーブルを作成してデータを調査できます。
author: minewiskan
ms.service: azure-analysis-services
ms.topic: conceptual
ms.date: 10/30/2019
ms.author: owend
ms.reviewer: minewiskan
ms.openlocfilehash: bb76accfef94327386d0ff58d003782a9fe3b0d2
ms.sourcegitcommit: f4d8f4e48c49bd3bc15ee7e5a77bee3164a5ae1b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/04/2019
ms.locfileid: "73573148"
---
# <a name="connect-with-excel"></a>Excel を使用した接続

サーバーを作成し、それに表形式モデルをデプロイしたら、クライアントは接続してデータの調査を開始できます。 

## <a name="before-you-begin"></a>開始する前に

サインインに使用するアカウントは、少なくとも、読み取り許可を持つ model データベースのロールに属していなければなりません。 詳細については、「[認証とユーザーのアクセス許可](analysis-services-manage-users.md)」を参照してください。 

## <a name="connect-in-excel"></a>Excel での接続

Excel でのサーバーへの接続は、Excel 2016 以降のデータの取得を使用してサポートされます。 Power Pivot での [テーブルのインポート] ウィザードを使用した接続はサポートされません。 

1. Excel では、 **[データ]** リボンで **[外部データの取り込み]**  >  **[その他のデータ ソース]**  >  **[Analysis Services]** の順にクリックします。

2. データ接続ウィザードで、 **[サーバー名]** にプロトコルや URI などのサーバー名を入力します。 たとえば、「asazure://westcentralus.asazure.windows.net/advworks」のように入力します。 そして **[ログオン資格情報]** で **[以下のユーザー名とパスワードを使用する]** を選択し、組織でのユーザー名 (たとえば nancy@adventureworks.com) とパスワードを入力します。

    > [!IMPORTANT]
    > Microsoft アカウント、Live ID、Yahoo、Gmail などでサインインする場合や、多要素認証を使用してサインインする必要がある場合は、パスワード フィールドを空白のままにしておきます。 [次へ] をクリックすると、パスワードの入力を求められます。 

    ![Excel ログオンから接続する](./media/analysis-services-connect-excel/aas-connect-excel-logon.png)

3. **[データベースとテーブルの選択]** で、データベースとモデルまたはパースペクティブを選択し、 **[完了]** をクリックします。
   
    ![Excel 選択モデルから接続する](./media/analysis-services-connect-excel/aas-connect-excel-select.png)


## <a name="see-also"></a>関連項目

[クライアント ライブラリ](analysis-services-data-providers.md)   
[サーバーの管理](analysis-services-manage.md)     


