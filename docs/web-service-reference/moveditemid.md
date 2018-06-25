---
title: MovedItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7d5425ab-1e75-43d1-b801-802ff5139df6
description: MovedItemId 要素は、MarkAsJunk 操作によって移動されたアイテムの識別子を指定します。
ms.openlocfilehash: 17e20e8ca81f97b419fc4a2b413e21322e828ec9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832484"
---
# <a name="moveditemid"></a>MovedItemId

**MovedItemId**要素は、 **MarkAsJunk**操作によって移動されたアイテムの識別子を指定します。 
  
```XML
<MovedItemId Id="" ChangeKey=""/>
```

 **ItemIdType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|ID  <br/> |**Id**属性の値は、 **MarkAsJunk**操作によって移動された項目の項目の識別子です。 アイテム識別子は変わりません、移動した後です。  <br/> |
|ChangeKey  <br/> |**変更キー**属性の値は、移動された項目のキーの変更です。 キーの変更は、 **MarkAsJunk**操作でアイテムを移動した後に変更します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[MarkAsJunkResponseMessage](markasjunkresponsemessage.md)
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |messages.xsd  <br/> |
|空にすることができます。  <br/> ||
   

