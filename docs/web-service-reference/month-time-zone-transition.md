---
title: 月 (タイム ゾーンの切り替え)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Month
api_type:
- schema
ms.assetid: 5e6aac75-366d-43d0-8ccb-956285474662
description: 月要素では、タイム ゾーンの切り替えが発生する月を表します。
ms.openlocfilehash: 887bd750b9cad1e28e6f7603c7b3289da8f8dc07
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832483"
---
# <a name="month-time-zone-transition"></a>月 (タイム ゾーンの切り替え)

**月**要素では、タイム ゾーンの切り替えが発生する月を表します。 
  
```xml
<Month/>
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
|[RecurringDateTransition](recurringdatetransition.md) <br/> |毎年特定の日に発生するタイム ゾーンの移行を表します。  <br/> |
|[RecurringDayTransition](recurringdaytransition.md) <br/> |毎年同じ日に発生するタイム ゾーンの移行を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、タイム ゾーンの切り替えが発生する月を表す整数です。
  
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

