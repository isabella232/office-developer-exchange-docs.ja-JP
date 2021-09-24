---
title: Occurrence (タイム ゾーン切り替え)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Occurrence
api_type:
- schema
ms.assetid: 5c1142b1-c51f-42e1-bbb2-57e00cad0fdb
description: Occurrence 要素は、タイム ゾーンの切り替えが発生した月の日の発生を表します。
ms.openlocfilehash: 9790b0e9541da0c22f2eac59850b8a361645c7b4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539278"
---
# <a name="occurrence-time-zone-transition"></a>Occurrence (タイム ゾーン切り替え)

**Occurrence 要素** は、タイム ゾーンの切り替えが発生した月の日の発生を表します。 
  
```xml
<Occurrence/>
```

**int**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[RecurringDayTransition](recurringdaytransition.md) <br/> |毎年同じ日に発生するタイム ゾーン遷移を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、タイム ゾーンの切り替えが発生した月の日の発生を表す整数です。 次の表に、使用可能な値を示します。
  
|**値**|**説明**|
|:-----|:-----|
|1  <br/> |月の初めから指定した週の最初の出現日。  <br/> |
|2  <br/> |月の初めから指定した週の 2 番目の出現日。  <br/> |
|3  <br/> |月の初めから指定した日の 3 番目に出現します。  <br/> |
|4   <br/> |月の初めから指定した週の 4 番目の出現日。  <br/> |
|-1  <br/> |指定した週の最初の出現日が、その月の終わりから発生します。  <br/> |
|-2  <br/> |指定した週の 2 番目の出現日が、その月の終わりから発生します。  <br/> |
|-3  <br/> |指定した日の 3 番目に、その月の終わりから発生します。  <br/> |
|-4  <br/> |指定した週の 4 番目に、その月の終わりから発生します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされているコンピューター Microsoft Exchange Server EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

