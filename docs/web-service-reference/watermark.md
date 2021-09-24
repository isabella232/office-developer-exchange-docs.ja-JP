---
title: Watermark
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Watermark
api_type:
- schema
ms.assetid: e1545046-94f9-4ac7-af1c-ea81dfb6822c
description: Watermark 要素は、メールボックス イベント キュー内のイベント ブックマークを表します。
ms.openlocfilehash: 959ae7369195a164d257b8805a8c985f1fdca53b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524400"
---
# <a name="watermark"></a>Watermark

**Watermark 要素** は、メールボックス イベント キュー内のイベント ブックマークを表します。 
  
```xml
<Watermark/>
```

 **透かしの種類**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[PullSubscriptionRequest](pullsubscriptionrequest.md) <br/> |プル ベースのイベント通知サブスクリプションのサブスクリプションを表します。  <br/> |
|[PushSubscriptionRequest](pushsubscriptionrequest.md) <br/> |プッシュ ベースのイベント通知サブスクリプションのサブスクリプションを表します。  <br/> |
|[GetEvents](getevents.md) <br/> |プル クライアントがサーバーから通知を要求するために使用する操作を表します。  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |アイテムまたはフォルダーがコピーされるイベントを表します。  <br/> |
|[CreatedEvent](createdevent.md) <br/> |アイテムまたはフォルダーが作成されるイベントを表します。  <br/> |
|[DeletedEvent](deletedevent.md) <br/> |アイテムまたはフォルダーが削除されるイベントを表します。  <br/> |
|[ModifiedEvent](modifiedevent.md) <br/> |アイテムまたはフォルダーが変更されたイベントを表します。  <br/> |
|[MovedEvent](movedevent.md) <br/> |ある親フォルダーから別の親フォルダーにアイテムまたはフォルダーを移動するイベントを表します。  <br/> |
|[NewMailEvent](newmailevent.md) <br/> |メールボックス内の新しいメール アイテムによってトリガーされるイベントを表します。  <br/> |
|[StatusEvent](statusevent.md) <br/> |メールボックスで新しいアクティビティが発生したという通知を表します。  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |サブスクライブ要求の状態と結果を格納します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、この要素の使用方法に応じて必須または省略可能です。
  
## <a name="remarks"></a>注釈

サブスクライブ要求に透かしが含まれている場合、サブスクリプションは透かしの転送から作成されます。 サブスクライブ要求に、メールボックス イベント テーブルに見つからない透かしが含まれている場合は、クライアント アプリケーション  `ErrorInvalidWatermark` にエラーが返されます。 これは、透かしが古すぎてイベント テーブルの 30 日ウィンドウから削除された場合、または透かしがイベント テーブルに存在しない場合に発生することがあります。 これは、たとえば、別のデータベース内のメールボックスの別のサブスクリプションから透かしが取得された場合に発生する可能性があります。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[サブスクライブ操作](subscribe-operation.md)
  
[GetEvents 操作](getevents-operation.md)
  
[Unsubscribe 操作](unsubscribe-operation.md)

