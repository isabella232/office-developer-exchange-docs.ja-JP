---
title: StatusFrequency
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StatusFrequency
api_type:
- schema
ms.assetid: 917474e2-a426-4166-b825-53783a41dad4
description: StatusFrequency 要素は、サーバーによって再試行が試行される最大タイムアウト時間 (分単位) を表します。
ms.openlocfilehash: db14ecfd54584188b3da16bb369db6c8089c70f4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468244"
---
# <a name="statusfrequency"></a>StatusFrequency

**Statusfrequency**要素は、サーバーによって再試行が試行される最大タイムアウト時間 (分単位) を表します。 
  
[登録](subscribe.md)
  
[PushSubscriptionRequest](pushsubscriptionrequest.md)
  
[StatusFrequency](statusfrequency.md)
  
```XML
<StatusFrequency/>
```

 **SubscriptionStatusFrequencyType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[PushSubscriptionRequest](pushsubscriptionrequest.md) <br/> |プッシュベースのイベント通知サブスクリプションのサブスクリプションを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素を使用する場合は、整数を表すテキスト値が必要です。 この要素で使用できる値は、1 ~ 1440 の範囲です。 この要素は省略できます。 既定値は 30 分です。
  
## <a name="remarks"></a>注釈

**Statusfrequency**値は、プッシュ通知またはクライアントからのステータス ping に対する応答が受信されない場合に、プッシュ通知を再試行するためにサーバーによって使用されます。 サーバーが応答を受信しない場合は、通知の送信を停止する前に、何度か通知の送信を再試行します。 EWS では、既定の再試行間隔は30秒で、その後の再試行は常に最後の再試行間隔の2倍の時間になります。 サーバー上の他の負荷が原因で遅延が発生する可能性があるので、再試行時間は正確ではありません。 次の表に、既定の**Statusfrequency**値 (サーバーで遅延が発生しなかった場合) によって割り当てられた30分間の再試行間隔を示します。 
  
|**再試行**|**秒**|**Time**|
|:-----|:-----|:-----|
|.0  <br/> |.0  <br/> |初期同期  <br/> |
|1   <br/> |31  <br/> |00:30  <br/> |
|pbm-2  <br/> |60  <br/> |01:00  <br/> |
|1/3  <br/> |120  <br/> |02:00  <br/> |
|4   <br/> |240  <br/> |04:00  <br/> |
|5   <br/> |480  <br/> |08:00  <br/> |
|6   <br/> |960  <br/> |16:00  <br/> |
|7   <br/> |1920  <br/> |32:00- **Statusfrequency**の既定値である30を超えたため、再試行を送信しない  <br/> |
   
**Statusfrequency**で指定された時間を超える期間、クライアントがサーバーからの通知メッセージを受信しない場合、クライアントはサブスクリプションの再作成などの操作を実行する必要があります。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
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
  
[Watermark](watermark.md)

