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
description: ConversationAction 要素には、単一の会話に適用される1つのアクションが含まれています。
ms.openlocfilehash: cb7d874f787b105d5185749dfaf1e940d2411d89
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529253"
---
# <a name="conversationaction"></a>ConversationAction

**ConversationAction**要素には、単一の会話に適用される1つのアクションが含まれています。 
  
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
|[アクション (ConversationActionTypeType)](action-conversationactiontypetype.md) <br/> |[ConversationId](conversationid.md)要素によって指定された会話に対して実行するアクションが含まれています。 この要素が存在している必要があります。  <br/> |
|[ConversationId](conversationid.md) <br/> |スレッドのアイテムに適用される[action (ConversationActionTypeType)](action-conversationactiontypetype.md)要素によって指定されたアクションを実行する会話の識別子が含まれます。 この要素が存在している必要があります。  <br/> |
|[ContextFolderId](contextfolderid.md) <br/> |フォルダーを使用する操作を対象とするフォルダーを示します。 この要素は、ターゲットフォルダー内の会話アイテムのコピー、削除、移動、および読み取り状態の設定時に存在する必要があります。  <br/> |
|[ConversationLastSyncTime](conversationlastsynctime.md) <br/> |会話が最後に同期された日付と時刻が含まれます。 この要素は、指定された時刻までに受信した会話内のすべてのアイテムを削除しようとするときに存在する必要があります。  <br/> |
|[ProcessRightAway](processrightaway.md) <br/> |アクションがサーバー上での処理を開始するとすぐに応答が送信されるか、またはアクションの完了後に応答が送信されるかを示します。 この要素は、要求されたアクションに応答を非同期送信するために存在する必要があります。  <br/> |
|[DestinationFolderId](destinationfolderid.md) <br/> |コピー操作と移動操作の宛先フォルダーを指定します。  <br/> |
|[Categories](categories-ex15websvcsotherref.md) <br/> |会話内のアイテムが属するカテゴリを識別する文字列のコレクションが含まれています。  <br/> |
|[Enablealways Delete](enablealwaysdelete.md) <br/> |スレッド内のすべての新規アイテムの削除を有効にするフラグを指定します。  <br/> |
|[IsRead](isread.md) <br/> |メッセージが開封されたかどうかを示します。  <br/> |
|[DeleteType](deletetype.md) <br/> |スレッド内のアイテムが削除される方法を示します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ConversationActions](conversationactions.md) <br/> |会話のコレクションと、それらに適用するアクションが含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

**ConversationAction 要素のテキスト値**

|**値**|**説明**|
|:-----|:-----|
|AlwaysCategorize  <br/> |常に会話を分類します。  <br/> |
|常に削除  <br/> |常に会話を削除します。  <br/> |
|常に移動  <br/> |常に会話を移動します。  <br/> |
|削除  <br/> |会話を削除します。  <br/> |
|Move  <br/> |会話を移動します。  <br/> |
|Copy  <br/> |会話をコピーします。  <br/> |
|SetReadState  <br/> |会話の読み取り状態を設定します。  <br/> |
|SetRetentionPolicy  <br/> |会話のアイテム保持ポリシーを設定します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[ApplyConversationAction 操作](applyconversationaction-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

