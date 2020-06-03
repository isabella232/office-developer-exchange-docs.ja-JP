---
title: Watermark
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
description: ウォーターマーク要素は、メールボックスイベントキュー内のイベントブックマークを表します。
ms.openlocfilehash: a717196101fea698b0b8c66f92a3d420fda9a421
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459764"
---
# <a name="watermark"></a>Watermark

**ウォーターマーク**要素は、メールボックスイベントキュー内のイベントブックマークを表します。 
  
```xml
<Watermark/>
```

 **WatermarkType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[PullSubscriptionRequest](pullsubscriptionrequest.md) <br/> |プルベースのイベント通知サブスクリプションに対するサブスクリプションを表します。  <br/> |
|[PushSubscriptionRequest](pushsubscriptionrequest.md) <br/> |プッシュベースのイベント通知サブスクリプションのサブスクリプションを表します。  <br/> |
|[GetEvents](getevents.md) <br/> |プルクライアントがサーバーからの通知を要求するために使用する操作を表します。  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |アイテムまたはフォルダーがコピーされるイベントを表します。  <br/> |
|[対する createdevent](createdevent.md) <br/> |アイテムまたはフォルダーが作成されるイベントを表します。  <br/> |
|[DeletedEvent](deletedevent.md) <br/> |アイテムまたはフォルダーが削除されるイベントを表します。  <br/> |
|[対する modifiedevent](modifiedevent.md) <br/> |アイテムまたはフォルダーが変更されるイベントを表します。  <br/> |
|[MovedEvent](movedevent.md) <br/> |ある親フォルダーから別の親フォルダーにアイテムまたはフォルダーを移動するイベントを表します。  <br/> |
|[NewMailEvent](newmailevent.md) <br/> |メールボックス内の新しいメールアイテムによってトリガーされるイベントを表します。  <br/> |
|[StatusEvent](statusevent.md) <br/> |メールボックス内で新しいアクティビティが発生していないことを示す通知を表します。  <br/> |
|[メッセージの表示](subscriberesponsemessage.md) <br/> |サブスクライブ要求の状態と結果を格納します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素の使用方法によっては、テキスト値が必須または省略可能である場合があります。
  
## <a name="remarks"></a>注釈

Subscribe 要求にウォーターマークが含まれている場合、サブスクリプションはウォーターマークの前から作成されます。 Subscribe 要求に、メールボックスの events テーブルにないウォーターマークが含まれる場合、 `ErrorInvalidWatermark` クライアントアプリケーションにエラーが返されます。 これは、ウォーターマークが古すぎ、[イベント] テーブルの30日間のウィンドウから削除されている場合、またはウォーターマークが events テーブルに存在しない場合に発生することがあります。 これは、たとえば、別のデータベースにあるメールボックスの別のサブスクリプションからウォーターマークが取得された場合などに発生します。 
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[サブスクライブ操作](subscribe-operation.md)
  
[GetEvents 操作](getevents-operation.md)
  
[Unsubscribe 操作](unsubscribe-operation.md)

