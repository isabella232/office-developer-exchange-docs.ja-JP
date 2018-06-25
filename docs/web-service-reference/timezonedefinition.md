---
title: タイム
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
description: タイムの要素では、期間およびタイム ゾーンを定義するための遷移を指定します。
ms.openlocfilehash: ffd5ed0c862af794e4aff2387f508849b1d5fd5d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839712"
---
# <a name="timezonedefinition"></a>タイム

**タイム**の要素では、期間およびタイム ゾーンを定義するための遷移を指定します。 
  
```XML
<TimeZoneDefinition Id="" Name="">
   <Periods/>
   <TransitionsGroups/>
   <Transitions/>
</TimeZoneDefinition>

```

 **TimeZoneDefinitionType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|ID  <br/> |タイム ゾーンの一意の識別子を表します。  <br/> |
|名前  <br/> |タイム ゾーンのわかりやすい名前を表します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[Periods](periods.md) <br/> |タイム ゾーンのさまざまな段階での時刻のオフセットを定義する[期間](period.md)の要素の配列を表します。  <br/> |
|[TransitionsGroups](transitionsgroups.md) <br/> |タイムゾーンの遷移を指定する[TransitionsGroup](transitionsgroup.md)要素の配列を表します。  <br/> |
|[遷移](transitions.md) <br/> |タイム ゾーンの移行の配列を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[TimeZoneDefinitions](timezonedefinitions.md) <br/> |タイム ゾーン定義の配列を表します。  <br/> |
|[TimeZoneContext](timezonecontext.md) <br/> |スコープの作成、更新、および Exchange Web サービス (EWS) を使用して取得するオブジェクトの DateTime プロパティを使用する既定のタイム ゾーンの定義を表します。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

