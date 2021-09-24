---
title: MovedItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 7d5425ab-1e75-43d1-b801-802ff5139df6
description: MovedItemId 要素は、MarkAsJunk 操作によって移動されたアイテムの識別子を指定します。
ms.openlocfilehash: 0775aaed119242fc2a2057fb20807d5be30692e5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509596"
---
# <a name="moveditemid"></a>MovedItemId

**MovedItemId** 要素は **、MarkAsJunk** 操作によって移動されたアイテムの識別子を指定します。 
  
```XML
<MovedItemId Id="" ChangeKey=""/>
```

 **ItemIdType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|ID  <br/> |Id 属性の値は **、MarkAsJunk** 操作によって移動されるアイテムのアイテム識別子です。  アイテム識別子は、移動後も同じままです。  <br/> |
|ChangeKey  <br/> |**ChangeKey** 属性の値は、移動したアイテムの変更キーです。 **MarkAsJunk** 操作によってアイテムを移動すると、変更キーが変更されます。  <br/> |
   
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
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |messages.xsd  <br/> |
|空の場合  <br/> ||
   

