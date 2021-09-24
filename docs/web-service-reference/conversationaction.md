---
title: ConversationAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ConversationAction
api_type:
- schema
ms.assetid: 9ecea41a-3860-4569-8e9b-284b451fc4e0
description: ConversationAction 要素には、1 つのスレッドに適用する 1 つのアクションが含まれる。
ms.openlocfilehash: 04af68b4ad8442160792fd3aa9f3259058a0f3a4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531107"
---
# <a name="conversationaction"></a>ConversationAction

**ConversationAction 要素には**、1 つのスレッドに適用する 1 つのアクションが含まれる。 
  
[ApplyConversationAction](applyconversationaction.md)
  
[ConversationActions](conversationactions.md)
  
[ConversationAction](conversationaction.md)
  
```XML
<ConversationAction>
   <Action/>
   <ConversationId/>
   <ContextFolderId/>
   <ConversationLastSyncTime/>
   <ProcessRightAway/>
   <DestinationFolderId/>
   <Categories/>
   <EnableAlwaysDelete/>
   <IsRead/>
   <DeleteType/>
</ConversationAction>
```

 **ConversationActionType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Action (ConversationActionTypeType)](action-conversationactiontypetype.md) <br/> |ConversationId 要素で指定された会話に対して実行するアクション [を格納](conversationid.md) します。 この要素が存在する必要があります。  <br/> |
|[ConversationId](conversationid.md) <br/> |Action [(ConversationActionTypeType)](action-conversationactiontypetype.md) 要素で指定されたアクションをスレッド内のアイテムに適用する会話の識別子を格納します。 この要素が存在する必要があります。  <br/> |
|[ContextFolderId](contextfolderid.md) <br/> |フォルダーを使用するアクションの対象となるフォルダーを示します。 この要素は、ターゲット フォルダー内の会話アイテムの読み取り状態をコピー、削除、移動、および設定するときに存在する必要があります。  <br/> |
|[ConversationLastSyncTime](conversationlastsynctime.md) <br/> |会話が最後に同期された日時を格納します。 この要素は、指定した時間まで受信した会話内のすべてのアイテムを削除しようとするときに存在する必要があります。  <br/> |
|[ProcessRightAway](processrightaway.md) <br/> |アクションがサーバーで処理を開始した直後に応答が送信されるかどうか、またはアクションが完了した後に応答が送信されるかどうかを示します。 要求されたアクションに非同期で送信される応答には、この要素が存在する必要があります。  <br/> |
|[DestinationFolderId](destinationfolderid.md) <br/> |コピーおよび移動アクションの移動先フォルダーを示します。  <br/> |
|[Categories](categories-ex15websvcsotherref.md) <br/> |会話内のアイテムが属するカテゴリを識別する文字列のコレクションを格納します。  <br/> |
|[EnableAlwaysDelete](enablealwaysdelete.md) <br/> |会話内のすべての新しいアイテムの削除を有効にするフラグを指定します。  <br/> |
|[IsRead](isread.md) <br/> |メッセージが読み取りされているかどうかを示します。  <br/> |
|[DeleteType](deletetype.md) <br/> |会話内のアイテムを削除する方法を示します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ConversationActions](conversationactions.md) <br/> |会話のコレクションと、会話に適用するアクションが含まれる。  <br/> |
   
## <a name="text-value"></a>テキスト値

**ConversationAction 要素のテキスト値**

|**値**|**説明**|
|:-----|:-----|
|AlwaysCategorize  <br/> |常に会話を分類します。  <br/> |
|AlwaysDelete  <br/> |常に会話を削除します。  <br/> |
|AlwaysMove  <br/> |常に会話を移動します。  <br/> |
|削除  <br/> |会話を削除します。  <br/> |
|Move  <br/> |会話を移動します。  <br/> |
|Copy  <br/> |会話をコピーします。  <br/> |
|SetReadState  <br/> |会話の読み取り状態を設定します。  <br/> |
|SetRetentionPolicy  <br/> |会話の保持ポリシーを設定します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web Services をホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[ApplyConversationAction 操作](applyconversationaction-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

