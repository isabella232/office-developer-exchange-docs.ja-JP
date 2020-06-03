---
title: FindConversation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindConversation
api_type:
- schema
ms.assetid: 94b7083c-60cf-478b-a9af-a88f7acb30fb
description: FindConversation 要素は、メールボックス内の会話を検索するための要求を定義します。
ms.openlocfilehash: 98d692132ed9375d981c95d24600b0e2c4b1d8c1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462648"
---
# <a name="findconversation"></a>FindConversation

**Findconversation**要素は、メールボックス内の会話を検索するための要求を定義します。 
  
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
|走査  <br/> |サブツリーの走査の種類を識別します。 この属性は省略可能です。  <br/> |
|ViewFilter  <br/> |種類ビューのフィルターを識別します。 この属性は省略可能です。  <br/> |
   
#### <a name="traversal-attribute-values"></a>トラバース属性値

****

|**値**|**説明**|
|:-----|:-----|
|浅い  <br/> |浅い走査を示します。  <br/> |
|深い  <br/> |Deep トラバースを示します。  <br/> |
   
#### <a name="viewfilter-attribute-values"></a>ViewFilter 属性値

****

|**値**|**説明**|
|:-----|:-----|
|すべて  <br/> |すべての会話を検索します。  <br/> |
|Flagged  <br/> |フラグ付きの会話を検索します。  <br/> |
|HasAttachment  <br/> |添付ファイル付きの会話を検索します。  <br/> |
|ToOrCcMe  <br/> |[宛先] または [cc] の会話を検索します。  <br/> |
|Unread  <br/> |未読の会話を検索します。  <br/> |
|TaskActive  <br/> |アクティブなタスクを検索します。  <br/> |
|TaskOverdue  <br/> |期限の過ぎたタスクを検索します。  <br/> |
|TaskCompleted  <br/> |完了したタスクを検索します。  <br/> |
|低優先メール  <br/> |内部使用のみ。  <br/> |
|クラッター機能  <br/> |内部使用のみ。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[IndexedPageItemView](indexedpageitemview.md) <br/> |ページングされた会話情報が返される方法について説明します。  <br/> |
|[SeekToConditionPageItemView](seektoconditionpageitemview.md) <br/> |検索の終了を識別するために使用される条件、検索の開始インデックス、返される最大エントリ、および**FindItem**または**findconversation**検索の検索方向を指定します。  <br/> |
|[SortOrder](sortorder.md) <br/> |[Findconversation 操作](findconversation-operation.md)要求でのアイテムの並べ替え方法を定義します。 **会話: LastDeliveryTime**プロパティは、 **findconversation**操作が使用されるときに並べ替えに対してサポートされている唯一のプロパティです。  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> |会話を検索するフォルダーを指定します。  <br/> |
|[MailboxScope](mailboxscope.md) <br/> |会話の検索またはフェッチがプライマリメールボックス、アーカイブメールボックス、またはプライマリメールボックスとアーカイブメールボックスのいずれかにスパンするかどうかを指定します。  <br/> |
|[QueryString (QueryStringType)](querystring-querystringtype.md) <br/> |高度なクエリ構文 (AQS) に基づくメールボックスクエリ文字列を指定します。  <br/> |
|[ConversationShape](conversationshape.md) <br/> |[Findconversation 操作](findconversation-operation.md)応答で返されるプロパティセットを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[FindConversation 操作](findconversation-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)


[EWS での会話](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

