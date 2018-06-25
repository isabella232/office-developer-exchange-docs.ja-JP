---
title: 発生 (タイム ゾーンの切り替え)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Occurrence
api_type:
- schema
ms.assetid: 5c1142b1-c51f-42e1-bbb2-57e00cad0fdb
description: 見つかった要素では、タイム ゾーンの切り替えが発生する月の週の日の発生を表します。
ms.openlocfilehash: bc5160480cc6881bb9d724aa61323f5717d1f2fa
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832636"
---
# <a name="occurrence-time-zone-transition"></a>発生 (タイム ゾーンの切り替え)

**見つかった**要素では、タイム ゾーンの切り替えが発生する月の週の日の発生を表します。 
  
```xml
<Occurrence/>
```

**int**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[RecurringDayTransition](recurringdaytransition.md) <br/> |毎年同じ日に発生するタイム ゾーンの移行を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、タイム ゾーンの切り替えが発生する月の週の日の発生を表す整数です。 次の表は、可能な値を一覧します。
  
|**値**|**説明**|
|:-----|:-----|
|1  <br/> |指定した曜日、月の最初から最初に出現します。  <br/> |
|2  <br/> |指定した曜日、月の最初からの 2 つ目の発生。  <br/> |
|3  <br/> |指定した曜日、月の最初からの 3 つ目の発生。  <br/> |
|4  <br/> |指定した曜日、月の最初からの 4 番目の発生。  <br/> |
|-1  <br/> |指定した曜日、月の最後から最初に出現します。  <br/> |
|-2  <br/> |指定した曜日、月の最後からの 2 つ目の発生。  <br/> |
|-3  <br/> |指定した曜日、月の最後からの 3 つ目の発生。  <br/> |
|-4  <br/> |指定した曜日、月の最後からの 4 番目の発生。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

