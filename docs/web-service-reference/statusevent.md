---
title: StatusEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StatusEvent
api_type:
- schema
ms.assetid: d3901818-2640-4bed-aad8-21a61aee62a1
description: StatusEvent 要素は、メールボックスに新しいアクティビティが発生していないことの通知を表します。
ms.openlocfilehash: e214918f9795e9e29061d4aac72ab144d2b24267
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833592"
---
# <a name="statusevent"></a>StatusEvent

**StatusEvent**要素は、メールボックスに新しいアクティビティが発生していないことの通知を表します。 
  
```xml
<StatusEvent>
   <Watermark/>
</StatusEvent>
```

 **BaseNotificationEventType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[透かし](watermark.md) <br/> |サブスクリプションの有効な最新のウォーターマークを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[通知](notification-ex15websvcsotherref.md) <br/> |サブスクリプションおよび最後の通知以降に発生したイベントに関する情報が含まれています。  <br/> |
   
## <a name="remarks"></a>備考

**StatusEvent**要素は次の理由の 1 つの通知で返されます。 
  
- プル クライアントでは、アクティビティがサブスクリプションの GetEvents 要求を発行しません。
    
- プッシュ クライアント イベントがありません。 キュー内の[StatusFrequency](statusfrequency.md)に到達したとき。 
    
**StatusEvent**[ウォーターマーク](watermark.md)は、他のイベントの種類のウォーターマークと同じ方法でクライアント アプリケーションによって使用されます。 ただし、 **StatusEvent**のウォーターマークは他のイベントに使用されるウォーターマークと同じです。 などの透かし 1 を使用してイベントをサブスクリプションには、2 と 3 とこれらのイベント通知されていること正常に通知します。 一定の期間が発生し、 **GetEvents**要求が送信されます。 クライアント アクセス サーバー (CAS) は、状態イベントを返し、 [PreviousWatermark](previouswatermark.md)と現在の[透かし](watermark.md)の両方として、3、最新のウォーターマークが含まれています。
  
透かしのすべてのケースで同じままになりません。 イベント エントリは、30 日間保持されます。 アクティブなサブスクリプションを維持するために、CA は、サブスクリプションのキューの透かしを定期的に更新します。 最新のウォーターマークは、アクティブなサブスクリプションを維持するために、クライアントに送信されます。
  
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

