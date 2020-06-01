---
title: Name (メッセージ追跡)
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
description: Name 要素は、メッセージ追跡レポートのプロパティ名を表します。
ms.openlocfilehash: 86f049c0a90dbeb55418a5eee58079adf17e5ded
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/01/2020
ms.locfileid: "44466900"
---
# <a name="name-message-tracking"></a>Name (メッセージ追跡)

**Name**要素は、メッセージ追跡レポートのプロパティ名を表します。 
  
```xml
<Name/>
```

**String**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[TrackingPropertyType](trackingpropertytype.md) <br/> |メッセージ追跡レポートのプロパティを作成するために使用される文字列の名前と値のペアを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素を使用する場合は、テキスト値が必要です。
  
## <a name="remarks"></a>注釈

この要素は、 [TrackingPropertyType](trackingpropertytype.md)要素で最大で1回発生する可能性があります。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

