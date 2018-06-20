---
title: GetConversationItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4f7bcd0f-140c-4cbc-a5ed-daeffded1df1
description: GetConversationItems 要素は、同じスレッドであることによって関連付けられている項目のセットを取得する要求を定義します。
ms.openlocfilehash: 9be300318a07173e4a8e11e5a6ca78b885de1199
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760664"
---
# <a name="getconversationitems"></a>GetConversationItems

**GetConversationItems**要素は、同じスレッドであることによって関連付けられている項目のセットを取得する要求を定義します。 
  
```XML
<GetConversationItems>
   <ItemShape/>
   <FoldersToIgnore/>
   <MaxItemsToReturn/>
   <SortOrder/>
   <MailboxScope/>
   <Conversations/>
</GetConversationItems>
```

 **GetConversationItemsType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[ItemShape](itemshape.md) | [FoldersToIgnore](folderstoignore.md) | [MaxItemsToReturn](maxitemstoreturn.md) | [ソート順序 (ConversationNodeSortOrder)](sortorder-conversationnodesortorder.md) | [MailboxScope](mailboxscope.md) | [会話](conversations-ex15websvcsotherref.md)
  
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
|空にすることができます。  <br/> |false  <br/> |
   

