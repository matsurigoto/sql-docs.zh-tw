---
title: "若要監視伺服器和 SQL Operations Studio （預覽） 中的資料庫使用深入解析小工具 |Microsoft 文件"
description: "深入了解 SQL Operations Studio （預覽） 中深入解析小工具。"
ms.custom: tools|sos
ms.date: 11/15/2017
ms.prod: sql-non-specified
ms.reviewer: alayu; erickang; sstein
ms.suite: sql
ms.prod_service: sql-tools
ms.component: sos
ms.tgt_pltfrm: 
ms.topic: article"
author: stevestein
ms.author: sstein
manager: craigg
ms.workload: Inactive
ms.openlocfilehash: d810e0b5ed89b93ac3d56a12758285fbd297092b
ms.sourcegitcommit: cc71f1027884462c359effb898390c8d97eaa414
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/21/2017
---
# <a name="manage-servers-and-databases-with-insight-widgets-in-includename-sosincludesname-sos-shortmd"></a>在 [!INCLUDE[name-sos] 中管理伺服器和資料庫的深入解析小工具 (../includes/name-sos-short.md)]

深入解析小工具需要您使用監視伺服器和資料庫 TRANSACT-SQL (T-SQL) 查詢並將它們轉換成具洞察力的視覺效果。 

Insights 是可自訂圖表和圖形加入至伺服器和資料庫監視儀表板。 檢視在摘要深入資訊，您的伺服器和資料庫，然後向下鑽研到詳細資訊，並啟動您所定義的管理動作。 

您可以透過下列類似範例建立實用伺服器和資料庫管理儀表板：

![資料庫儀表板](media/insight-widgets/database-dashboard.png)


若要進入並開始建立不同類型的深入解析小工具，請參閱下列教學課程：

- [建置自訂的深入解析小工具](tutorial-build-custom-insight-sql-server.md)
- *啟用內建的深入解析小工具*
   - [啟用效能監視 insight](tutorial-qds-sql-server.md)
   - [啟用資料表空間使用量深入資訊](tutorial-table-space-sql-server.md)


## <a name="sql-queries"></a>SQL 查詢 

[!INCLUDE[name-sos](../includes/name-sos-short.md)]若要避免引進其他語言或大量的使用者介面，因此它會嘗試使用 T-SQL 盡可能以最小的 JSON 組態尚未嘗試。 使用 T-SQL 深入解析小工具會利用無數的有用可以轉換成具洞察力的小工具的 T-SQL 查詢現有來源的數目。

深入解析小工具是由一個或兩個 T-SQL 查詢所組成：
* *深入解析小工具查詢*是必要的且查詢會傳回小工具中出現的資料。
* *深入解析詳細資料查詢*是如果您建立深入解析詳細資料頁面，才需要。

深入解析小工具查詢定義轉譯計數、 圖表或圖形的資料集。 深入解析詳細資料的查詢用來列出相關的 Insight 詳細資訊，深入解析詳細資料窗格中以表格格式。 

[!INCLUDE[name-sos](../includes/name-sos-short.md)]執行深入解析小工具查詢並將查詢結果集對應至圖表的資料集，然後會將其轉譯。 當使用者開啟深入解析的詳細資料時，它會執行深入了解詳細資料查詢，並會列印出方格檢視 對話方塊中的結果。

基本概念是寫入 T-SQL 查詢的方式，因此它可用來當做資料集的計數、 圖表和圖形小工具。 

## <a name="summary"></a>摘要

T-SQL 查詢和它的結果集決定深入解析小工具行為。 撰寫查詢的圖表類型，或對應現有查詢的正確的圖表類型是關鍵考量來建置有效的深入解析小工具。



## <a name="additional-resources"></a>其他資源
- [查詢編輯器](tutorial-sql-editor.md)

