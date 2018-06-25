---
title: MarkAsJunk
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f06bafc6-7ee3-4b2b-9fd1-7c51328f4729
description: MarkAsJunk 要素は、[迷惑メール] フォルダーにアイテムを移動して、送信者を受信拒否リストに追加する要求を指定します。
ms.openlocfilehash: fbb3eee7ce350954888931ca55b27f596656b161
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832350"
---
# <a name="markasjunk"></a>MarkAsJunk

**MarkAsJunk**要素は、[迷惑メール] フォルダーにアイテムを移動して、送信者を受信拒否リストに追加する要求を指定します。 
  
```XML
<MarkAsJunk IsJunk="true | false" MoveItem="true | false">
   <ItemIds/>
</MarkAsJunk>
```

 **MarkAsJunkType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|引数 IsJunk  <br/> |**True** **引数 IsJunk**属性のテキスト値は、電子メールの送信者は、受信拒否リストに追加されていることを示します。 **False**の値は、電子メール送信者の一覧に既に場合に、電子メールの送信者がブロックされる送信者の一覧から削除されているを示します。  <br/> |
|MoveItem  <br/> |の**場合は true** 、 **MoveItem**属性のテキスト値は、既定の迷惑メール フォルダーにアイテムを移動することを示します。 **False**の値は、項目が既定の迷惑メール フォルダーに移動していないことを示します。  <br/> |
   
### <a name="child-elements"></a>子要素

[Itemid](itemids.md)
  
### <a name="parent-elements"></a>親要素

なし。
  
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
   

