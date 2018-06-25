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
description: StatusFrequency 要素は、分単位、サーバーの再試行が行わ、タイムアウトの最大値を表します。
ms.openlocfilehash: 402f8978c0ec6b377dfa020f23595c8954509a07
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833589"
---
# <a name="statusfrequency"></a>StatusFrequency

**StatusFrequency**要素は、分単位、サーバーの再試行が行わ、タイムアウトの最大値を表します。 
  
[購読](subscribe.md)
  
[PushSubscriptionRequest](pushsubscriptionrequest.md)
  
[StatusFrequency](statusfrequency.md)
  
```XML
<StatusFrequency/>
```

 **SubscriptionStatusFrequencyType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[PushSubscriptionRequest](pushsubscriptionrequest.md) <br/> |プッシュ ベースのイベント通知サブスクリプションをサブスクリプションを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

整数値を表すテキスト値は、この要素を使用する場合に必要です。 この要素の値は、1 から 1440 の範囲です。 この要素はオプションです。 既定値は、30 分です。
  
## <a name="remarks"></a>備考

**StatusFrequency**値は、クライアントからのプッシュ通知やステータスの ping に応答を受信しません、プッシュ通知を再試行するのには、サーバーによって使用されます。 サーバーが応答を受信しない場合は、通知の送信を停止する前に、何回か、通知の送信を再試行します。 EWS、既定の再試行間隔は、30 秒でそれ以降の再試行は、常に最後の再試行間隔の時間が 2 倍。 サーバー上の他の負荷のための遅延と、再試行の回数は正確ではないです。 (サーバーは、任意の遅延を検出しなかったと仮定した場合)、デフォルトの**StatusFrequency**値に割り当てられている 30 分以内に再試行の間隔が発生する方法を次の表に示します。 
  
|**再試行**|**秒**|**時間**|
|:-----|:-----|:-----|
|0  <br/> |0  <br/> |初期同期  <br/> |
|1  <br/> |30  <br/> |00:30  <br/> |
|2  <br/> |60  <br/> |01:00  <br/> |
|3  <br/> |120  <br/> |02:00  <br/> |
|4  <br/> |240  <br/> |04:00  <br/> |
|5  <br/> |480  <br/> |08:00  <br/> |
|6  <br/> |960  <br/> |16:00  <br/> |
|7  <br/> |1920  <br/> |32:00 - **StatusFrequency**の既定値の 30 を超えると、再試行が送信されません。  <br/> |
   
クライアントを受信しない場合の通知メッセージ、サーバーから**StatusFrequency**で指定されたタイムの 2 倍を超える時間の期間、クライアントはサブスクリプションを再作成するなどアクションを実行する必要があります。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
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
  
[透かし](watermark.md)

