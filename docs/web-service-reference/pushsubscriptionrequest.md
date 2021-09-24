---
title: PushSubscriptionRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PushSubscriptionRequest
api_type:
- schema
ms.assetid: 70caa0ca-40a1-421f-b4e6-0658f22d0b8e
description: PushSubscriptionRequest 要素は、プッシュ ベースのイベント通知サブスクリプションのサブスクリプションを表します。
ms.openlocfilehash: 6eb76bba92e78e048ae97dbec5fc6c4d698a815f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523728"
---
# <a name="pushsubscriptionrequest"></a>PushSubscriptionRequest

**PushSubscriptionRequest** 要素は、プッシュ ベースのイベント通知サブスクリプションのサブスクリプションを表します。 
  
[Subscribe](subscribe.md)
  
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
|**SubscribeToAllFolders** <br/> |使用可能なすべてのフォルダーをサブスクライブするかどうかを示します。 この属性は省略可能です。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[FolderIds](folderids.md) <br/> |イベント通知を監視するフォルダーを識別するために使用されるフォルダー識別子の配列を格納します。  <br/> |
|[EventTypes](eventtypes.md) <br/> |サブスクリプションの作成に使用されるイベント通知のコレクションを含む。  <br/> |
|[Watermark](watermark.md) <br/> |メールボックス イベント テーブルのイベント ブックマークを表します。 これは、透かしで表されるイベントから始まるサブスクリプションを作成するために使用されます。 Subscribe 要求の透かしが見つからない場合は、エラー応答がクライアントに返されます。 これは、透かしが 30 日を超える場合、またはメールボックスに透かしが存在しない場合に発生することがあります。  <br/> |
|[StatusFrequency](statusfrequency.md) <br/> |イベントが発生しない場合にクライアントに通知メッセージを送信する頻度 (分) を表します。  <br/> |
|[Url ](url-ex15websvcsotherref.md) <br/> |プッシュ通知のクライアント Web サービスの場所を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Subscribe](subscribe.md) <br/> |サブスクリプションの作成に使用するプロパティを格納します。  <br/> |
   
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



[サブスクライブ操作](subscribe-operation.md)
  
[GetEvents 操作](getevents-operation.md)
  
[Unsubscribe 操作](unsubscribe-operation.md)

