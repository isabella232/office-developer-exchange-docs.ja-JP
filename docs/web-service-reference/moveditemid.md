---
title: MovedItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7d5425ab-1e75-43d1-b801-802ff5139df6
description: MovedItemId 要素は、MarkAsJunk 操作によって移動されたアイテムの id を指定します。
ms.openlocfilehash: 5cf8800ec672278691348bbcd8c6c8cc7a12905b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468615"
---
# <a name="moveditemid"></a>MovedItemId

**Moveditemid**要素は、 **markasjunk**操作によって移動されたアイテムの id を指定します。 
  
```XML
<MovedItemId Id="" ChangeKey=""/>
```

 **ItemIdType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|ID  <br/> |**Id**属性の値は、 **markasjunk**操作によって移動されるアイテムのアイテム識別子です。 移動後も、アイテムの識別子は変わりません。  <br/> |
|ChangeKey  <br/> |**Changekey**属性の値は、移動されたアイテムの変更キーです。 **Markasjunk**操作によってアイテムが移動された後に、change キーが変更されます。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[MarkAsJunkResponseMessage](markasjunkresponsemessage.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空にすることができます。  <br/> ||
   

