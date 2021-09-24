---
title: FindConversation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FindConversation
api_type:
- schema
ms.assetid: 94b7083c-60cf-478b-a9af-a88f7acb30fb
description: FindConversation 要素は、メールボックス内の会話を検索する要求を定義します。
ms.openlocfilehash: e48e0d9fd71dac12fe6848031b2c056ea9a913ce
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59535171"
---
# <a name="findconversation"></a>FindConversation

**FindConversation 要素は**、メールボックス内の会話を検索する要求を定義します。 
  
[FindConversation](findconversation.md)
  
```XML
<FindConversation Traversal="" ViewFilter="">
   <IndexedPageItemView/>
   <SeekToConditionPageItemView/>
   <SortOrder/>
   <ParentFolderId/>
   <MailboxScope/>
   <QueryString/>
   <ConversationShape/>
</FindConversation>
```

 **FindConversationType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

****

|**属性**|**説明**|
|:-----|:-----|
|Traversal  <br/> |サブツリー トラバーサルの種類を識別します。 この属性は省略可能です。  <br/> |
|ViewFilter  <br/> |種類のビュー フィルターを識別します。 この属性は省略可能です。  <br/> |
   
#### <a name="traversal-attribute-values"></a>Traversal 属性値

****

|**値**|**説明**|
|:-----|:-----|
|浅い  <br/> |浅いトラバーサルを示します。  <br/> |
|深い  <br/> |深いトラバーサルを示します。  <br/> |
   
#### <a name="viewfilter-attribute-values"></a>ViewFilter 属性値

****

|**値**|**説明**|
|:-----|:-----|
|すべて  <br/> |すべての会話を検索します。  <br/> |
|Flagged  <br/> |フラグが設定された会話を検索します。  <br/> |
|HasAttachment  <br/> |添付ファイルを含む会話を検索します。  <br/> |
|ToOrCcMe  <br/> |自分に対してアドレス指定または cc'd の会話を見つける。  <br/> |
|Unread  <br/> |未読の会話を見つける。  <br/> |
|TaskActive  <br/> |アクティブなタスクを検索します。  <br/> |
|TaskOverdue  <br/> |時間が過ぎたタスクを検索します。  <br/> |
|TaskCompleted  <br/> |完了したタスクを検索します。  <br/> |
|NoClutter  <br/> |内部使用のみ。  <br/> |
|クラッター機能  <br/> |内部使用のみ。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[IndexedPageItemView](indexedpageitemview.md) <br/> |ページ会話情報が返される方法について説明します。  <br/> |
|[SeekToConditionPageItemView](seektoconditionpageitemview.md) <br/> |検索の終了、検索の開始インデックス、返す最大エントリ、 **および FindItem** または **FindConversation** 検索の検索方向を識別するために使用する条件を指定します。  <br/> |
|[SortOrder](sortorder.md) <br/> |[FindConversation](findconversation-operation.md)操作要求でアイテムを並べ替える方法を定義します。 **conversation:LastDeliveryTime** プロパティは **、FindConversation** 操作を使用するときに並べ替えでサポートされる唯一のプロパティです。  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> |会話を検索するフォルダーを識別します。  <br/> |
|[MailboxScope](mailboxscope.md) <br/> |会話の検索またはフェッチをプライマリ メールボックス、アーカイブ メールボックス、またはプライマリ メールボックスとアーカイブ メールボックスの両方にまたがるかどうかを指定します。  <br/> |
|[QueryString (QueryStringType)](querystring-querystringtype.md) <br/> |高度なクエリ構文 (AQS) に基づくメールボックス クエリ文字列を指定します。  <br/> |
|[ConversationShape](conversationshape.md) <br/> |[FindConversation](findconversation-operation.md)操作応答で返すプロパティ セットを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web Services をホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[FindConversation 操作](findconversation-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)


[EWS での会話](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

