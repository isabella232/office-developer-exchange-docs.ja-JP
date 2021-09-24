---
title: TimeZoneDefinition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- TimeZoneDefinition
api_type:
- schema
ms.assetid: b005a80c-addb-4409-beff-e5162076752c
description: TimeZoneDefinition 要素は、タイム ゾーンを定義する期間と遷移を指定します。
ms.openlocfilehash: 6f2b580d2c3e31826ca74034cfda938cff71ee53
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538815"
---
# <a name="timezonedefinition"></a>TimeZoneDefinition

**TimeZoneDefinition 要素は**、タイム ゾーンを定義する期間と遷移を指定します。 
  
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
|ID  <br/> |タイム ゾーンの一意の識別子を表します。  <br/> |
|名前  <br/> |タイム ゾーンのわかりやすい名前を表します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Periods](periods.md) <br/> |タイム ゾーンの異なるステージでのタイム オフセットを定義する [Period](period.md) 要素の配列を表します。  <br/> |
|[TransitionsGroups](transitionsgroups.md) <br/> |タイム ゾーンの遷移を [指定する TransitionsGroup](transitionsgroup.md) 要素の配列を表します。  <br/> |
|[Transitions](transitions.md) <br/> |タイム ゾーン遷移の配列を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[TimeZoneDefinitions](timezonedefinitions.md) <br/> |タイム ゾーン定義の配列を表します。  <br/> |
|[TimeZoneContext](timezonecontext.md) <br/> |Exchange Web Services (EWS) を使用して作成、更新、および取得されるオブジェクトの DateTime プロパティをスコープ化するために使用される既定のタイム ゾーン定義を表します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

