---
title: コマーシャル マーケットプレース分析でのパートナー センターの [注文] ダッシュボード
description: マーケットプレース オファーの注文に関するグラフィカルでダウンロード可能な形式の分析レポートにアクセスする方法について説明します。
author: ChJenk
manager: evansma
ms.author: v-chjen
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
ms.date: 12/11/2019
ms.openlocfilehash: bf4b48fafa5b877053abe653b569cf27eb50d57b
ms.sourcegitcommit: f4f626d6e92174086c530ed9bf3ccbe058639081
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/25/2019
ms.locfileid: "75475317"
---
# <a name="orders-dashboard-in-commercial-marketplace-analytics"></a>コマーシャル マーケットプレース分析での [注文] ダッシュボード

この記事では、パートナー センターの **[注文] ダッシュボード**について説明します。 このダッシュボードには、注文に関するグラフィカルでダウンロード可能な形式の情報が表示されます。

パートナー センター分析ツールの **[注文] ダッシュボード**にアクセスするには、コマーシャル マーケットプレースの **[[分析] ダッシュボード](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/summary)** を開きます。

>[!NOTE]
> 分析の用語の詳細な定義については、「[コマーシャル マーケットプレース分析に関するよく寄せられる質問と用語](./faq-terminology.md)」を参照してください。

## <a name="orders-dashboard"></a>[注文] ダッシュボード

**[分析]** メニューの **[注文]** ダッシュボードには、すべての SaaS オファーの現在の注文が表示されます。 次の項目のグラフィカル表示を見ることができます。

- [注文の概要](#order-summary)
- [地域別注文数](#orders-by-geography)
- [オファーごとの注文数](#orders-by-offers)
- [サイトごとおよびシートごとの注文数の傾向](#orders-trend-per-site-versus-per-seat)
- [SKU 別の注文](#orders-by-skus)
- [注文およびシートの傾向](#orders-and-seats-trend)
- [注文詳細テーブル](#order-details-table)

> [!NOTE]
> Cloud パートナー ポータル (CPP) と、パートナー センターの新しい [Commercial Marketplace]\(商用マーケットプレース\) プログラムでは、分析レポートの表示方法に違いがあります。 具体的な違いの 1 つとして、CPP の **[Seller Insights]\(販売者分析情報\)** には **[Orders & Usage]\(注文と使用量\)** タブがあり、ここには、使用量ベースのオファーと使用量ベースでないオファーに関するデータが表示されます。 パートナー センターの **[注文]** ページには、SaaS 注文の独立したタブがあります。

## <a name="order-dashboard-details"></a>[注文] ダッシュボードの詳細

このセクションでは、分析レポートについて詳しく説明します。

### <a name="order-summary"></a>注文の概要

[注文の概要] セクションには、すべての購入された注文 (キャンセルされた注文を除く)、キャンセルされた注文、およびシートの数が表示されます。

[注文合計] の横のパーセント値は、選択した日付範囲での増加量を表します。

![パートナー センター分析での注文概要](./media/order-summary.png)

- 上向きの緑の三角形はプラスの増加傾向を示します。
- 下向きの赤い三角形は前月比のマイナスの増加傾向を示します。
- 増加傾向は、小さい棒グラフで表されます。 各月の値を表示するには、グラフ内の棒にマウス ポインターを合わせます。
- キャンセルされた注文数は、以前に購入された後、選択した日付範囲内にキャンセルされた注文の数です。
- シート数は、選択した日付範囲内に作成されたシートの数です。

### <a name="orders-by-geography"></a>地域別注文数

**[地域ごとの注文]** ヒートマップでは、注文数が世界地図上に表示され、顧客の国に基づいてマップされたシート数が示されます。 このヒートマップは、 **[[地域別の顧客] ヒートマップ](./customer-dashboard.md#customer-by-geography)** と同じ機能です。

![パートナー センター分析の地域ごとの注文](./media/orders-by-geography.png)

### <a name="orders-by-offers"></a>オファーごとの注文

**[オファーごとの注文]** ドーナツ グラフには、オファー名に従って注文数 (キャンセルされた注文を含む) がまとめられます。

- 上位のオファーがグラフに表示され、残りのオファーは [Rest All]\(残りすべて\) としてグループ化されます。
- 凡例で特定のオファーを選択し、それらのオファーのみをグラフに表示することができます。
- グラフのスライスにポインターを合わせると、注文数とそのオファーの割合が、すべてのオファーの合計注文数と比較して表示されます。
- **オファーごとの注文の傾向**には、月単位での増加傾向が表示されます。 月の列はオファー名別の注文数を表します。 折れ線グラフでは、増加率の傾向を Z 軸にプロットして表示します。
- グラフの上部にあるスライダーを使用して、X 軸に沿って左右にスクロールし、特定のデータ ポイントにフォーカスすることができます。
- 凡例の特定の項目を選択すると、傾向グラフを表示できます。
- **キャンセルされた注文**の傾向とデータを表示する選択もできます。 グラフの機能は、**オファーごとの注文数**のグラフと同じです。

### <a name="orders-trend-per-site-versus-per-seat"></a>サイトごとおよびシートごとの注文数の傾向

**サイトごととシートごとの対比**のドーナツ グラフには、顧客によって購入されたサイトごとの SaaS 注文数とシートごとの SaaS 注文数の内訳が表示されます (このグラフには、キャンセルされた注文が含まれます)。 棒グラフには、顧客によって購入されたサイトごとの SaaS 注文数とシートごとの SaaS 注文数の傾向が表示されます (このグラフには、キャンセルされた注文が含まれます)。

### <a name="orders-by-skus"></a>SKU 別の注文

**[SKU 別の注文]** グラフには、すべてのオファーの Stock Keeping Unit (SKU) レベルでの注文数の傾向が表されます (これには、キャンセルされた注文が含まれます)。 ドーナツ グラフには上位 5 つの SKU の注文数の内訳が表され、棒グラフには上位 5 つの SKU の注文数の傾向が表示されます。

### <a name="orders-and-seats-trend"></a>注文およびシートの傾向

**[注文およびシートの傾向]** グラフには、注文数が最も多い上位 50 のオファーが表示されます。 これらはランキングに表示され、最大注文数と注文率で並べ替えられます。

- **[SKU 別の注文]** : グラフ内の上位 5 SKU の注文数の内訳を表示するには、オファーを選択します。
- **[SKU 別のシート]** : 上位 5 SKU のシート数の月ごとの傾向です。 選択したオファーがシートごとのオファーではない場合、この面グラフにデータは表示されません。

### <a name="canceled-orders-by-offers"></a>オファーごとのキャンセルされた注文

**[オファーごとのキャンセルされた注文]** 円グラフには、オファー名に従ってすべてのキャンセルされた注文がまとめられます。 上位のオファーがグラフに表示され、残りのオファーは [Rest All]\(残りすべて\) としてグループ化されます。 凡例で特定のオファーを選択して、それをグラフに表示することができます。

- グラフのスライスをポイントすると、選択したオファーの注文数と割合が、すべてのオファーの合計注文数と比較して表示されます。
- 棒グラフには、月ごとの傾向が表示されます。 棒は、オファー名ごとのキャンセルされた注文の数を表します。 グラフの上部にあるスライダーを使用して、X 軸に沿って左右にスクロールし、特定のデータ ポイントにフォーカスすることができます。 凡例の特定の項目を選択すると、傾向グラフを表示できます。

### <a name="order-details-table"></a>注文詳細テーブル

注文詳細テーブルには、購入日で並べ替えた上位 1000 注文の番号付きリストが表示されます。

- グリッドの各列で並べ替えることができます。
- レコード数が 1000 未満の場合、TSV ファイルにデータを抽出できます。
- レコード数が 1000 を超える場合、エクスポートされたデータは今後 30 日間、ダウンロード ページに非同期で配置されます。
- **注文詳細テーブル**にフィルターを適用して、関心のあるデータのみを表示できます。 データに適用できるフィルターは、国、Azure ライセンスの種類、Marketplace ライセンスの種類、オファーの種類、注文の状態、無料評価版、マーケットプレース サブスクリプション ID、顧客 ID、および会社名です。

#### <a name="orders-page-filters"></a>注文ページ フィルター

これらのフィルターは、ページ レベルで適用されます。

複数のフィルターを選択して、表示するよう選択した基準に合ったグラフや、 **[Detailed Order Data]\(詳細な注文データ\)** グリッドおよびエクスポートに表示したいデータを表示できます。 フィルターは、注文ページの右上隅で選択したデータ範囲に対して抽出されたデータに適用されます。

- オファーの種類とオファー名は、選択した日付範囲内に注文があるオファーに対してのみ表示されます。 一覧で選択したオファーの種類について、一覧にオファー名が表示されます。
- 適用したフィルターでは、選択した各フィルターについて、各選択内の合計メトリックが表示されます。 既定の選択では、適用したフィルターは表示されません。
- いずれかのドロップダウン リストで **[すべて]** を選択すると、選択したページ内のすべてのメトリックが集計されます。 次に例を示します。オファーの種類フィルター オプションの [すべて] は、すべてのオファーの種類が選択されていることを意味します。 これは、ドロップダウン リストの既定の選択です。 **[すべて]** を選択すると、適用したフィルターでは何も表示されません。
- **複数の値の選択**: ドロップダウン リストで行ったすべての選択に対し、ページ内のすべてのメトリックが集計されます。 複数の選択を行った場合、適用したフィルターでは、選択したすべての項目の数が表示されます。 次の画像を参照してください。

    ![パートナー センター分析で、フィルターに複数の値が適用された注文](./media/filters-applied.png)

- **1 つの値の選択**: 1 つの値を選択した場合、適用したフィルターでは、選択した 1 つのフィルターの数が表示されます。 以下の画像を参照してください。

     ![パートナー センター分析で、フィルターに 1 つの値が適用された注文](./media/filters-applied-single.png)

## <a name="next-steps"></a>次のステップ

- パートナー センターのコマーシャル マーケットプレースで利用可能な分析レポートの概要については、「[パートナー センターでの商用マーケットプレース向け分析](./analytics.md)」を参照してください。
- オファーのマーケットプレース アクティビティを要約した集計データのグラフ、傾向、値については、「[コマーシャル マーケットプレース分析の概要ダッシュボード](./summary-dashboard.md)」を参照してください。
- 仮想マシン (VM) オファーの使用量と従量制課金メトリックについては、「[コマーシャル マーケットプレース分析の使用量ダッシュボード](./usage-dashboard.md)」を参照してください。
- 成長傾向など、顧客の詳細については、「[コマーシャル マーケットプレース分析の顧客ダッシュボード](./customer-dashboard.md)」を参照してください。
- 過去 30 日間のダウンロード要求の一覧については、「[コマーシャル マーケットプレース分析のダウンロード ダッシュボード](./downloads-dashboard.md)」を参照してください。
- Azure Marketplace と AppSource でのオファーに関する顧客からのフィードバックを統合して表示する方法については、「[コマーシャル マーケットプレース分析の評価とレビューのダッシュボード](./ratings-reviews.md)」を参照してください。
- コマーシャル マーケットプレース分析についてよく寄せられる質問と、データ用語の包括的な辞書については、「[コマーシャル マーケットプレース分析に関するよく寄せられる質問と用語](./faq-terminology.md)」を参照してください。
