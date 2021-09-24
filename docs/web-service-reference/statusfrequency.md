---
title: StatusFrequency
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- StatusFrequency
api_type:
- schema
ms.assetid: 917474e2-a426-4166-b825-53783a41dad4
description: StatusFrequency 要素は、サーバーが再試行する最大タイムアウト値を分で表します。
ms.openlocfilehash: f0359bab58167bbe7be5cce8c250240bebc7cc08
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525534"
---
# <a name="statusfrequency"></a>StatusFrequency

**StatusFrequency** 要素は、サーバーが再試行する最大タイムアウト値を分で表します。 
  
[Subscribe](subscribe.md)
  
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
|[PushSubscriptionRequest](pushsubscriptionrequest.md) <br/> |プッシュ ベースのイベント通知サブスクリプションのサブスクリプションを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素を使用する場合は、整数を表すテキスト値が必要です。 この要素に使用できる値は、1 ~ 1440 です。含まれます。 この要素は省略できます。 既定値は 30 分です。
  
## <a name="remarks"></a>注釈

**StatusFrequency 値** は、クライアントからプッシュ通知または状態 ping への応答を受信しない場合に、プッシュ通知を再試行するためにサーバーによって使用されます。 サーバーが応答を受信しない場合、通知の送信を何度も再試行してから、通知の送信を停止します。 EWS では、既定の再試行間隔は 30 秒で、それ以降の再試行は常に最後の再試行間隔の 2 倍になります。 再試行時間は、サーバー上の他の負荷のために遅延する可能性がある正確ではありません。 次の表は、既定の **StatusFrequency** 値によって割り当てられた 30 分で再試行間隔が発生する方法を示しています (サーバーに遅延が発生しなかった場合)。 
  
|**再試行**|**秒**|**Time**|
|:-----|:-----|:-----|
|0  <br/> |0  <br/> |初期同期  <br/> |
|1  <br/> |30  <br/> |00:30  <br/> |
|2  <br/> |60  <br/> |01:00  <br/> |
|3  <br/> |120  <br/> |02:00  <br/> |
|4   <br/> |240  <br/> |04:00  <br/> |
|5  <br/> |480  <br/> |08:00  <br/> |
|6   <br/> |960  <br/> |16:00  <br/> |
|7   <br/> |1920  <br/> |32:00 - **StatusFrequency** の既定値 30 を超え、再試行は送信されません  <br/> |
   
**StatusFrequency** で指定された時間の 2 倍を超える期間、クライアントがサーバーから通知メッセージを受信しない場合、クライアントはサブスクリプションの再作成などのアクションを実行する必要があります。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
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
  
[Watermark](watermark.md)

