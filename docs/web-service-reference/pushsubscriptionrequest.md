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
description: PushSubscriptionRequest 要素は、プッシュベースのイベント通知サブスクリプションへのサブスクリプションを表します。
ms.openlocfilehash: dcdb767ed175468aa4ec940f3147c164e4707e40
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465514"
---
# <a name="pushsubscriptionrequest"></a>PushSubscriptionRequest

**Pushsubscriptionrequest**要素は、プッシュベースのイベント通知サブスクリプションへのサブスクリプションを表します。 
  
[登録](subscribe.md)
  
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
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**SubscribeToAllFolders** <br/> |利用可能なすべてのフォルダーを購読するかどうかを示します。 この属性は省略可能です。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[FolderIds](folderids.md) <br/> |イベント通知を監視するフォルダーを識別するために使用されるフォルダー識別子の配列を格納します。  <br/> |
|[EventTypes](eventtypes.md) <br/> |サブスクリプションの作成に使用されるイベント通知のコレクションが含まれています。  <br/> |
|[Watermark](watermark.md) <br/> |メールボックスイベントテーブル内のイベントブックマークを表します。 これは、ウォーターマークで表されるイベントから開始するサブスクリプションを作成するために使用されます。 Subscribe 要求のウォーターマークが見つからない場合は、クライアントにエラー応答が返されます。 これは、ウォーターマークが30日よりも古い場合、またはウォーターマークがメールボックスに存在しない場合に発生することがあります。  <br/> |
|[StatusFrequency](statusfrequency.md) <br/> |イベントが発生していない場合に通知メッセージがクライアントに送信される頻度 (分単位) を表します。  <br/> |
|[.Url](url-ex15websvcsotherref.md) <br/> |プッシュ通知用のクライアント Web サービスの場所を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[登録](subscribe.md) <br/> |サブスクリプションの作成に使用されるプロパティが含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[サブスクライブ操作](subscribe-operation.md)
  
[GetEvents 操作](getevents-operation.md)
  
[Unsubscribe 操作](unsubscribe-operation.md)

