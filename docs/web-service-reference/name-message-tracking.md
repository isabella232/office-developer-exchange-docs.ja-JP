---
title: 名前 (メッセージの追跡)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Name
api_type:
- schema
ms.assetid: a1669f6d-53f3-4849-9b30-56909aaeac82
description: Name 要素は、メッセージ ・ トラッキング ・ レポートのプロパティ名を表します。
ms.openlocfilehash: c905df03842de47b2bcbd62897aa9a8cf464cc6d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832501"
---
# <a name="name-message-tracking"></a>名前 (メッセージの追跡)

**Name**要素は、メッセージ ・ トラッキング ・ レポートのプロパティ名を表します。 
  
```xml
<Name/>
```

**文字列型 (String)**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[TrackingPropertyType](trackingpropertytype.md) <br/> |名前と値文字列のペアを使用してレポートを追跡するメッセージのプロパティを作成するを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、この要素が使用される場合に必要です。
  
## <a name="remarks"></a>備考

この要素に最大で 1 回、 [TrackingPropertyType](trackingpropertytype.md)の要素で発生します。 
  
この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

