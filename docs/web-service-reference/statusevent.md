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
description: StatusEvent 要素は、メールボックス内で新しいアクティビティが発生していないことを示す通知を表します。
ms.openlocfilehash: 8158a47937a810be2ea22346384b4e61da56ac48
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468258"
---
# <a name="statusevent"></a>StatusEvent

**Statusevent**要素は、メールボックス内で新しいアクティビティが発生していないことを示す通知を表します。 
  
```xml
<StatusEvent>
   <Watermark/>
</StatusEvent>
```

 **BaseNotificationEventType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Watermark](watermark.md) <br/> |サブスクリプションの最後の有効なウォーターマークを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[通知](notification-ex15websvcsotherref.md) <br/> |サブスクリプションに関する情報、および前回の通知以降に発生したイベントに関する情報が含まれます。  <br/> |
   
## <a name="remarks"></a>注釈

**Statusevent**要素は、次のいずれかの理由で通知で返されます。 
  
- プルクライアントが、アクティビティのないサブスクリプションに対して GetEvents 要求を発行します。
    
- [Statusfrequency](statusfrequency.md)に達した場合、プッシュクライアントにはキューにイベントがありません。 
    
**Statusevent**[ウォーターマーク](watermark.md)は、クライアントアプリケーションによって、他のイベントの種類のウォーターマークと同じ方法で使用されます。 ただし、 **Statusevent**のウォーターマークは、他のイベントで使用されるウォーターマークとは異なります。 たとえば、サブスクリプションにはウォーターマーク1、2、および3のイベントがあり、それらのイベントは通知で正常に伝達されています。 非アクティブな期間が発生し、 **GetEvents**要求が送信されます。 クライアントアクセスサーバー (CAS) は状態イベントを返し、最後のウォーターマーク3を[PreviousWatermark](previouswatermark.md)と現在の[ウォーターマーク](watermark.md)の両方として含みます。
  
ウォーターマークは、すべての場合に変わりません。 イベントエントリは、30日間保持されます。 アクティブなサブスクリプションを維持するために、CAS はサブスクリプションキューのウォーターマークを定期的に更新します。 更新されたウォーターマークは、アクティブなサブスクリプションを維持するためにクライアントに送信されます。
  
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

