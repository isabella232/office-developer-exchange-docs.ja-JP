---
title: PushSubscriptionRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PushSubscriptionRequest
api_type:
- schema
ms.assetid: 70caa0ca-40a1-421f-b4e6-0658f22d0b8e
description: PushSubscriptionRequest 要素は、プッシュ ベースのイベント通知サブスクリプションをサブスクリプションを表します。
ms.openlocfilehash: 34717d37b8e5bb50c927e57088299fbcb18a2514
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832929"
---
# <a name="pushsubscriptionrequest"></a>PushSubscriptionRequest

**PushSubscriptionRequest**要素は、プッシュ ベースのイベント通知サブスクリプションをサブスクリプションを表します。 
  
[購読](subscribe.md)
  
[PushSubscriptionRequest](pushsubscriptionrequest.md)
  
```XML
<PushSubscriptionRequest SubscribeToAllFolders="">
   <FolderIds/>
   <EventTypes/>
   <Watermark/>
   <StatusFrequency/>
   <URL/>
</PushSubscriptionRequest>
```

 **PushSubscriptionRequestType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**SubscribeToAllFolders** <br/> |使用可能なすべてのフォルダーを購読するかどうかを示します。 この属性は、省略可能です。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[FolderIds](folderids.md) <br/> |イベント通知を監視するフォルダーを識別するために使用されるフォルダー識別子の配列が含まれています。  <br/> |
|[EventTypes](eventtypes.md) <br/> |サブスクリプションを作成するために使用されるイベント通知のコレクションが含まれています。  <br/> |
|[透かし](watermark.md) <br/> |メールボックス イベント テーブル内のイベント ブックマークを表します。 透かしによって表されるイベントからサブスクリプションの作成に使用されます。 Subscribe 要求からのウォーターマークが見つからない場合、エラー応答がクライアントに返されます。 これは、透かしは、30 日間またはウォーターマークがメールボックス内に存在しなかったかどうかよりも古い場合に発生します。  <br/> |
|[StatusFrequency](statusfrequency.md) <br/> |(分)、通知のメッセージがクライアントに送信、イベントが発生していない場合、頻度を表します。  <br/> |
|[Url](url-ex15websvcsotherref.md) <br/> |クライアント プッシュ通知のための Web サービスの場所を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[購読](subscribe.md) <br/> |サブスクリプションを作成するためのプロパティが含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[サブスクライブ操作](subscribe-operation.md)
  
[GetEvents 操作](getevents-operation.md)
  
[Unsubscribe 操作](unsubscribe-operation.md)

