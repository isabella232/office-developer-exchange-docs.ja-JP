---
title: 宛先
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- To
api_type:
- schema
ms.assetid: d14e46da-14bd-4a33-a78e-8ee314d9c1d8
description: To 要素は、タイムゾーン遷移のターゲットを指定します。 目標は、タイムゾーンの期間またはタイムゾーンの移行のグループのいずれかです。
ms.openlocfilehash: 8cce700eedd64035f2e21be4db6b517f3f85d98d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468797"
---
# <a name="to"></a>宛先

**To**要素は、タイムゾーン遷移のターゲットを指定します。 目標は、タイムゾーンの期間またはタイムゾーンの移行のグループのいずれかです。 
  
```xml
<To Kind=""/>
```

 **遷移 Tiontargettype**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|Kind  <br/> |タイムゾーンの移行対象がタイムゾーンの期間であるか、またはタイムゾーンの切り替えのグループであるかを示します。  <br/> |
   
#### <a name="kind-attribute-values"></a>Kind 属性値

|**値**|**説明**|
|:-----|:-----|
|ピリオド  <br/> |タイムゾーンの移行ターゲットがタイムゾーンの期間であることを指定します。  <br/> |
|Group  <br/> |タイムゾーンの移行ターゲットが、タイムゾーン遷移のグループであることを指定します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AbsoluteDateTransition](absolutedatetransition.md) <br/> |特定の日付および特定の時刻に発生するタイムゾーンの切り替えを表します。  <br/> |
|[RecurringDayTransition](recurringdaytransition.md) <br/> |毎年同じ日に発生するタイムゾーンの切り替えを表します。  <br/> |
|[RecurringDateTransition](recurringdatetransition.md) <br/> |指定した日に発生するタイムゾーンの切り替えを表します。  <br/> |
|[Transition](transition.md) <br/> |タイムゾーンの切り替えを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、期間または時間帯遷移のターゲットである[期間](period.md)または[推移 tionsgroup](transitionsgroup.md)の一意の識別子を指定する文字列です。 
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|名前空間  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

