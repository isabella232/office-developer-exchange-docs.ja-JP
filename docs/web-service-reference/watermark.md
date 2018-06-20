---
title: ウォーターマーク
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Watermark
api_type:
- schema
ms.assetid: e1545046-94f9-4ac7-af1c-ea81dfb6822c
description: 透かしの要素は、メールボックス イベント キュー内のイベント ブックマークを表します。
ms.openlocfilehash: 1867aa781bc24f5eb3bdb4648fa494a2a7ea396a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839999"
---
# <a name="watermark"></a>ウォーターマーク

**透かし**の要素は、メールボックス イベント キュー内のイベント ブックマークを表します。 
  
```xml
<Watermark/>
```

 **WatermarkType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[PullSubscriptionRequest](pullsubscriptionrequest.md) <br/> |プル ベースのイベント通知サブスクリプションをサブスクリプションを表します。  <br/> |
|[PushSubscriptionRequest](pushsubscriptionrequest.md) <br/> |プッシュ ベースのイベント通知サブスクリプションをサブスクリプションを表します。  <br/> |
|[GetEvents](getevents.md) <br/> |プル クライアントがサーバーからの通知を要求に使用する操作を表します。  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |アイテムまたはフォルダーがコピーされるイベントを表します。  <br/> |
|[CreatedEvent](createdevent.md) <br/> |アイテムまたはフォルダーが作成されるイベントを表します。  <br/> |
|[DeletedEvent](deletedevent.md) <br/> |アイテムまたはフォルダーが削除されたイベントを表します。  <br/> |
|[ModifiedEvent](modifiedevent.md) <br/> |アイテムまたはフォルダーが変更されたイベントを表します。  <br/> |
|[MovedEvent](movedevent.md) <br/> |アイテムまたはフォルダーの移動先フォルダーの 1 つの親から別の親フォルダー イベントを表します。  <br/> |
|[NewMailEvent](newmailevent.md) <br/> |メールボックス内の新しいメール アイテムによって発生したイベントを表します。  <br/> |
|[StatusEvent](statusevent.md) <br/> |通知メールボックスに新しいアクティビティが発生していないことを表します。  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |Subscribe 要求の結果ステータスを格納します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値には、必須またはオプションによっては、この要素を使用する方法があります。
  
## <a name="remarks"></a>備考

Subscribe 要求にウォーターマークが含まれている場合、サブスクリプションはウォーターマークから先作成されます。 Subscribe 要求にウォーターマークがメールボックス イベント テーブル内に見つからないことが含まれている場合、`ErrorInvalidWatermark`エラーがクライアント アプリケーションに返されます。 ウォーターマークが古すぎるので、30 日間のウィンドウ イベント テーブルから削除された場合に発生することも透かしがかつてない場合は、イベント テーブルに表示します。 これは、たとえば、ウォーターマークが別のデータベース内のメールボックスの別のサブスクリプションから取得した場合に発生します。 
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[サブスクライブ操作](subscribe-operation.md)
  
[GetEvents 操作](getevents-operation.md)
  
[Unsubscribe 操作](unsubscribe-operation.md)

