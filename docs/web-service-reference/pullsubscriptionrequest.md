---
title: PullSubscriptionRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PullSubscriptionRequest
api_type:
- schema
ms.assetid: 145c5cc7-a894-4f0b-a6ea-358cddfb5c33
description: PullSubscriptionRequest 要素は、プル ベースのイベント通知サブスクリプションをサブスクリプションを表します。
ms.openlocfilehash: 5f757bf1f79f7e2a00fb886db50e6ea0eaed1a4a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832932"
---
# <a name="pullsubscriptionrequest"></a>PullSubscriptionRequest

**PullSubscriptionRequest**要素は、プル ベースのイベント通知サブスクリプションをサブスクリプションを表します。 
  
[購読](subscribe.md)
  
[PullSubscriptionRequest](pullsubscriptionrequest.md)
  
```XML
<PullSubscriptionRequest SubscribeToAllFolders="">
   <FolderIds/>
   <EventTypes/>
   <Watermark/>
   <Timeout/>
</PullSubscriptionRequest>
```

 **PullSubscriptionRequestType**
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
|[透かし](watermark.md) <br/> |メールボックス イベント テーブル内のイベント ブックマークを表します。 ウォーターマークが表すイベントで開始されるサブスクリプションを作成するために使用されます。 Subscribe 要求からのウォーターマークが見つからない場合、エラー応答がクライアントに返されます。 ウォーターマークは、30 日間またはウォーターマークがメールボックス内に存在しなかったかどうかよりも古い場合、このエラーが発生する可能性があります。  <br/> |
|[Timeout](timeout.md) <br/> |サブスクリプションがクライアントからの GetEvents 要求なしアイドルを分単位で、期間を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[購読](subscribe.md) <br/> |サブスクリプションの作成に使用するプロパティが含まれています。  <br/> |
   
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



[PushSubscriptionRequest](pushsubscriptionrequest.md)
  
[サブスクライブ操作](subscribe-operation.md)
  
[GetEvents 操作](getevents-operation.md)
  
[Unsubscribe 操作](unsubscribe-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

