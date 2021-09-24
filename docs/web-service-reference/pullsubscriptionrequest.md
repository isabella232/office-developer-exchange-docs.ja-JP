---
title: PullSubscriptionRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PullSubscriptionRequest
api_type:
- schema
ms.assetid: 145c5cc7-a894-4f0b-a6ea-358cddfb5c33
description: PullSubscriptionRequest 要素は、プルベースのイベント通知サブスクリプションのサブスクリプションを表します。
ms.openlocfilehash: f1a527dff0c81262cac01a905293af1155acbf1c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540602"
---
# <a name="pullsubscriptionrequest"></a>PullSubscriptionRequest

**PullSubscriptionRequest** 要素は、プルベースのイベント通知サブスクリプションのサブスクリプションを表します。 
  
[Subscribe](subscribe.md)
  
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
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**SubscribeToAllFolders** <br/> |使用可能なすべてのフォルダーをサブスクライブするかどうかを示します。 この属性は省略可能です。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[FolderIds](folderids.md) <br/> |イベント通知を監視するフォルダーを識別するために使用されるフォルダー識別子の配列を格納します。  <br/> |
|[EventTypes](eventtypes.md) <br/> |サブスクリプションの作成に使用されるイベント通知のコレクションを含む。  <br/> |
|[Watermark](watermark.md) <br/> |メールボックス イベント テーブルのイベント ブックマークを表します。 これは、透かしで表されるイベントから始まるサブスクリプションを作成するために使用されます。 Subscribe 要求の透かしが見つからない場合は、エラー応答がクライアントに返されます。 このエラーは、透かしが 30 日より古い場合、または透かしがメールボックスに存在しない場合に発生する可能性があります。  <br/> |
|[Timeout](timeout.md) <br/> |クライアントからの GetEvents 要求なしでサブスクリプションがアイドル状態を維持できる期間を分単位で表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Subscribe](subscribe.md) <br/> |サブスクリプションの作成に使用されるプロパティを格納します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[PushSubscriptionRequest](pushsubscriptionrequest.md)
  
[サブスクライブ操作](subscribe-operation.md)
  
[GetEvents 操作](getevents-operation.md)
  
[Unsubscribe 操作](unsubscribe-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

