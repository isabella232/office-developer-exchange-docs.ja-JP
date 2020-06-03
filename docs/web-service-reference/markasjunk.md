---
title: MarkAsJunk
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f06bafc6-7ee3-4b2b-9fd1-7c51328f4729
description: MarkAsJunk 要素は、アイテムを迷惑メールフォルダーに移動し、送信者を受信拒否リストに追加する要求を指定します。
ms.openlocfilehash: 99adc423864f3096772394ef290df20e158e457d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467082"
---
# <a name="markasjunk"></a>MarkAsJunk

**Markasjunk**要素は、アイテムを迷惑メールフォルダーに移動し、送信者を受信拒否リストに追加する要求を指定します。 
  
```XML
<MarkAsJunk IsJunk="true | false" MoveItem="true | false">
   <ItemIds/>
</MarkAsJunk>
```

 **MarkAsJunkType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|IsJunk  <br/> |**Isjunk**属性のテキスト値が**true の場合**は、電子メール送信者がブロックされた送信者の一覧に追加されていることを示します。 値が**false**の場合、電子メール送信者が既にリストに含まれている場合は、受信拒否リストから電子メール送信者が削除されることを示します。  <br/> |
|MoveItem  <br/> |**Moveitem**属性のテキスト値が**true の場合**は、アイテムが既定の迷惑メールフォルダーに移動されることを示します。 値が**false**の場合は、アイテムが既定の迷惑メールフォルダーに移動されないことを示します。  <br/> |
   
### <a name="child-elements"></a>子要素

[ItemIds](itemids.md)
  
### <a name="parent-elements"></a>親要素

なし。
  
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
   

