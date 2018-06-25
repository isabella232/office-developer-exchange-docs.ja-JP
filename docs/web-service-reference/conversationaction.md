---
title: ConversationAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConversationAction
api_type:
- schema
ms.assetid: 9ecea41a-3860-4569-8e9b-284b451fc4e0
description: ConversationAction 要素には、1 つのテーマを適用する 1 つのアクションが含まれています。
ms.openlocfilehash: 45cd6df3aba94062bd5aa0ddf9367e8cf118dc6b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759753"
---
# <a name="conversationaction"></a>ConversationAction

**ConversationAction**要素には、1 つのテーマを適用する 1 つのアクションが含まれています。 
  
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
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[アクション (ConversationActionTypeType)](action-conversationactiontypetype.md) <br/> |[ConversationId](conversationid.md)要素で指定されたスレッド上で実行するアクションが含まれています。 この要素が存在する必要があります。  <br/> |
|[ConversationId](conversationid.md) <br/> |会話内のアイテムに適用される[アクション (ConversationActionTypeType)](action-conversationactiontypetype.md)の要素によって指定されたアクションがある会話スレッドの識別子が含まれています。 この要素が存在する必要があります。  <br/> |
|[ContextFolderId](contextfolderid.md) <br/> |フォルダーを使用する操作を対象としているフォルダーを示します。 この要素は、コピー、削除、移動、およびターゲット フォルダー内のアイテムの会話の読み取り状態を設定するときに存在する必要があります。  <br/> |
|[ConversationLastSyncTime](conversationlastsynctime.md) <br/> |会話が最後に同期された日時が含まれています。 この要素は、会話で指定した時刻までに受信したすべてのアイテムを削除しようとするときに存在する必要があります。  <br/> |
|[ProcessRightAway](processrightaway.md) <br/> |アクションがサーバーまたはアクションが完了した後に応答を送信するかどうかで処理を開始すると、すぐに応答を送信するかどうかを示します。 この要素は、要求された操作を非同期に送信する応答のために存在する必要があります。  <br/> |
|[DestinationFolderId](destinationfolderid.md) <br/> |コピー先のフォルダーを指定し、アクションを移動します。  <br/> |
|[Categories](categories-ex15websvcsotherref.md) <br/> |会話内の項目が所属するカテゴリを識別する文字列のコレクションが含まれています。  <br/> |
|[EnableAlwaysDelete](enablealwaysdelete.md) <br/> |会話内のすべての新しいアイテムの削除を有効にするフラグを指定します。  <br/> |
|[IsRead](isread.md) <br/> |メッセージが読み取られたかどうかを示します。  <br/> |
|[削除の種類](deletetype.md) <br/> |会話内の項目を削除する方法を示します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ConversationActions](conversationactions.md) <br/> |会話およびそれらに適用するアクションのコレクションが含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

**ConversationAction 要素のテキスト値**

|**値**|**説明**|
|:-----|:-----|
|AlwaysCategorize  <br/> |会話を常に分類します。  <br/> |
|AlwaysDelete  <br/> |会話を常に削除します。  <br/> |
|AlwaysMove  <br/> |会話を常に移動します。  <br/> |
|削除  <br/> |会話を削除します。  <br/> |
|移動  <br/> |会話に移動します。  <br/> |
|Copy  <br/> |会話をコピーします。  <br/> |
|SetReadState  <br/> |会話の読み取り状態を設定します。  <br/> |
|SetRetentionPolicy  <br/> |会話のリテンション ・ ポリシーを設定します。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[ApplyConversationAction 操作](applyconversationaction-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

