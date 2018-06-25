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
ms.openlocfilehash: 990e15f468f836d51977329c524acb439014da95
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760497"
---
# <a name="findconversation"></a>FindConversation

**FindConversation**要素は、メールボックス内の会話を検索するための要求を定義します。 
  
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
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

****

|**属性**|**説明**|
|:-----|:-----|
|トラバーサル  <br/> |サブツリーの走査の種類を識別します。 この属性は、省略可能です。  <br/> |
|ビューワ  <br/> |型ビューのフィルターを識別します。 この属性は、省略可能です。  <br/> |
   
#### <a name="traversal-attribute-values"></a>検査の属性値

****

|**値**|**説明**|
|:-----|:-----|
|浅い  <br/> |Shallow トラバースを示します。  <br/> |
|深い  <br/> |Deep traversal 検索を示します。  <br/> |
   
#### <a name="viewfilter-attribute-values"></a>ビューワの属性値

****

|**値**|**説明**|
|:-----|:-----|
|All  <br/> |すべての会話を検索します。  <br/> |
|Flagged  <br/> |フラグが設定された会話を検索します。  <br/> |
|添付ファイルあり  <br/> |添付ファイルとの会話を検索します。  <br/> |
|ToOrCcMe  <br/> |会話の宛先または cc のように自分の名前を検索します。  <br/> |
|Unread  <br/> |未読の会話を検索します。  <br/> |
|TaskActive  <br/> |アクティブなタスクを検索します。  <br/> |
|TaskOverdue  <br/> |期限過ぎのタスクを検索します。  <br/> |
|TaskCompleted  <br/> |完了したタスクを検索します。  <br/> |
|NoClutter  <br/> |内部使用のために用意されています。  <br/> |
|散乱  <br/> |内部使用のために用意されています。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[IndexedPageItemView](indexedpageitemview.md) <br/> |ページがどのように会話を説明する情報が返されます。  <br/> |
|[SeekToConditionPageItemView](seektoconditionpageitemview.md) <br/> |検索の終了、検索、戻るには、最大のエントリと**FindItem**または**FindConversation**の検索に検索方向の開始インデックスを識別するために使用される条件を指定します。  <br/> |
|[並べ替え順序](sortorder.md) <br/> |[FindConversation 操作](findconversation-operation.md)の要求の項目の並べ替え方法を定義します。 **会話: LastDeliveryTime**プロパティは、 **FindConversation**操作を使用する場合の並べ替えはサポートされている唯一のプロパティです。  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> |会話を検索するフォルダーを識別します。  <br/> |
|[MailboxScope](mailboxscope.md) <br/> |かどうか、検索、または会話をフェッチする必要があります、プライマリ メールボックス、アーカイブ メールボックス、または両方のプライマリ、メールボックスのアーカイブを指定します。  <br/> |
|[クエリ文字列 (QueryStringType)](querystring-querystringtype.md) <br/> |ベースの高度なクエリ構文 (AQS) のメールボックスのクエリ文字列を指定します。  <br/> |
|[ConversationShape](conversationshape.md) <br/> |[FindConversation 操作](findconversation-operation.md)の応答を返すにプロパティ セットを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目




  [FindConversation 操作](findconversation-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)


[EWS での会話](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

