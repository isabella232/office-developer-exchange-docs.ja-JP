---
title: 発生 (タイムゾーンの切り替え)
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
description: オカレンスリンク要素は、タイムゾーンの切り替えが行われる月の曜日の発生を表します。
ms.openlocfilehash: 846f6b22f43bcda07b9408d768d0845a5acfe668
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467978"
---
# <a name="occurrence-time-zone-transition"></a>発生 (タイムゾーンの切り替え)

**オカレンスリンク**要素は、タイムゾーンの切り替えが行われる月の曜日の発生を表します。 
  
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
|[RecurringDayTransition](recurringdaytransition.md) <br/> |毎年同じ日に発生するタイムゾーンの切り替えを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

Text 値は、タイムゾーンの切り替えが行われる月の曜日の発生を表す整数です。 次の表に、使用可能な値を示します。
  
|**値**|**説明**|
|:-----|:-----|
|1-d  <br/> |月の最初から指定された曜日の最初の出現。  <br/> |
|pbm-2  <br/> |月の最初から指定された曜日の2回目の出現。  <br/> |
|1/3  <br/> |月の最初から指定された曜日の3番目の出現。  <br/> |
|4   <br/> |月の最初の曜日の、指定された曜日の4番目の出現。  <br/> |
|-1  <br/> |月の終わりから、指定された曜日の最初の出現。  <br/> |
|-2  <br/> |月の終わりから、指定された曜日の2回目の出現。  <br/> |
|-3  <br/> |月の終わりから、指定された曜日の3番目の出現。  <br/> |
|-4  <br/> |月の終わりから、指定された曜日の4番目の出現。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

