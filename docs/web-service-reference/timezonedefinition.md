---
title: TimeZoneDefinition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeZoneDefinition
api_type:
- schema
ms.assetid: b005a80c-addb-4409-beff-e5162076752c
description: TimeZoneDefinition 要素は、タイムゾーンを定義する期間と遷移を指定します。
ms.openlocfilehash: 58d34556686bfc77244b5829798eada51a1df843
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466067"
---
# <a name="timezonedefinition"></a>TimeZoneDefinition

**TimeZoneDefinition**要素は、タイムゾーンを定義する期間と遷移を指定します。 
  
```XML
<TimeZoneDefinition Id="" Name="">
   <Periods/>
   <TransitionsGroups/>
   <Transitions/>
</TimeZoneDefinition>

```

 **TimeZoneDefinitionType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|ID  <br/> |タイムゾーンの一意の識別子を表します。  <br/> |
|名前  <br/> |タイムゾーンのわかりやすい名前を表します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Periods](periods.md) <br/> |タイムゾーンのさまざまな段階での時間のオフセットを定義する[Period](period.md)要素の配列を表します。  <br/> |
|[遷移のグループ](transitionsgroups.md) <br/> |タイムゾーンの遷移を指定する、[推移 Tionsgroup](transitionsgroup.md)要素の配列を表します。  <br/> |
|[切り替わる](transitions.md) <br/> |タイムゾーンの切り替えの配列を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[TimeZoneDefinitions](timezonedefinitions.md) <br/> |タイムゾーン定義の配列を表します。  <br/> |
|[TimeZoneContext](timezonecontext.md) <br/> |Exchange Web サービス (EWS) を使用して作成、更新、および取得されるオブジェクトの DateTime プロパティのスコープ設定に使用される既定のタイムゾーン定義を表します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

