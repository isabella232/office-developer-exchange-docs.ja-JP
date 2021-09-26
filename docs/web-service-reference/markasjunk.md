---
title: MarkAsJunk
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f06bafc6-7ee3-4b2b-9fd1-7c51328f4729
description: MarkAsJunk 要素は、アイテムを迷惑メール フォルダーに移動し、送信者をブロックされた送信者リストに追加する要求を指定します。
ms.openlocfilehash: 252c36b8bb3662ffd6c0fe470a81b6f0b55acb69
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544088"
---
# <a name="markasjunk"></a>MarkAsJunk

**MarkAsJunk** 要素は、アイテムを迷惑メール フォルダーに移動し、送信者をブロックされた送信者リストに追加する要求を指定します。 
  
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
|IsJunk  <br/> |**IsJunk** 属性 **のテキスト値が true** の場合、電子メール送信者がブロックされた送信者リストに追加されます。 false の **値は** 、電子メール送信者が既にリストに存在する場合に、電子メール送信者がブロックされた送信者リストから削除されるかどうかを示します。  <br/> |
|MoveItem  <br/> |**MoveItem** 属性の **テキスト値が true** の場合は、アイテムが既定の迷惑メール フォルダーに移動されます。 false の **値は** 、アイテムが既定の迷惑メール フォルダーに移動されないかどうかを示します。  <br/> |
   
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
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |messages.xsd  <br/> |
|空の場合  <br/> ||
   

