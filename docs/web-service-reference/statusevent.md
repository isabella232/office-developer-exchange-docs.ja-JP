---
title: StatusEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- StatusEvent
api_type:
- schema
ms.assetid: d3901818-2640-4bed-aad8-21a61aee62a1
description: StatusEvent 要素は、メールボックスで新しいアクティビティが発生したという通知を表します。
ms.openlocfilehash: 777d5cd22e47fea6e7bf7432e58e5d58d1ef67a4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543976"
---
# <a name="statusevent"></a>StatusEvent

**StatusEvent 要素** は、メールボックスで新しいアクティビティが発生したという通知を表します。 
  
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
|[Watermark](watermark.md) <br/> |サブスクリプションの最後の有効な透かしを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[通知](notification-ex15websvcsotherref.md) <br/> |サブスクリプションと、前回の通知以降に発生したイベントに関する情報が格納されます。  <br/> |
   
## <a name="remarks"></a>注釈

**StatusEvent 要素** は、次のいずれかの理由で通知で返されます。 
  
- プル クライアントは、アクティビティがないサブスクリプションに対して GetEvents 要求を発行します。
    
- [StatusFrequency](statusfrequency.md)に達した場合、プッシュ クライアントにはキューにイベントはありません。 
    
**StatusEvent**[透かし](watermark.md)は、他のイベントの種類の透かしと同じ方法でクライアント アプリケーションによって使用されます。 ただし **、StatusEvent** の透かしは、他のイベントで使用される透かしと同じではありません。 たとえば、サブスクリプションには透かし 1、2、3 のイベントが含まれます。これらのイベントは通知で正常に伝達されています。 非アクティブの期間が発生し **、GetEvents 要求が** 送信されます。 クライアント アクセス サーバー (CAS) は、状態イベントを返し [、PreviousWatermark](previouswatermark.md) と現在の透かしの両方として最後の透かし 3 を含 [む](watermark.md)。
  
透かしは、すべてのケースで同じままではありません。 イベント エントリは 30 日間保持されます。 アクティブなサブスクリプションを維持するために、CAS はサブスクリプション キューの透かしを定期的に更新します。 更新された透かしは、アクティブなサブスクリプションを維持するためにクライアントに送信されます。
  
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

