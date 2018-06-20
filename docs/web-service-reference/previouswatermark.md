---
title: PreviousWatermark
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PreviousWatermark
api_type:
- schema
ms.assetid: 474f4f7c-47da-47d4-8126-230012172fb5
description: PreviousWatermark 要素は、サブスクリプションのためにクライアントに正常に通信された最新イベントのウォーターマークを表します。
ms.openlocfilehash: 93c6f90d0866ae13618391b8544ab593fe33922b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832886"
---
# <a name="previouswatermark"></a>PreviousWatermark

**PreviousWatermark**要素は、サブスクリプションのためにクライアントに正常に通信された最新イベントのウォーターマークを表します。 
  
```xml
<PreviousWatermark/>
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
|[通知](notification-ex15websvcsotherref.md) <br/> |サブスクリプションおよび最後の通知以降に発生したイベントに関する情報が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 テキスト値は、最新のウォーターマークを表します。 テキスト値は、空の文字列にすることはできません。
  
## <a name="remarks"></a>備考

**PreviousWatermark**プロパティは、最後の成功の通知を決定するときにクライアントに便利です。 たとえば、サブスクリプションには 1、2、および 3 の透かしを使用して次の 3 つのイベント、3 の**PreviousWatermark**値を持つ次の通知が送信される場合は、クライアントは受信した最後の通知のウォーターマークの値にこの値を比較できます。 これにより、クライアントのイベントの継続性を確保します。 
  
プッシュ クライアントは、 **PreviousWatermark**は、クライアント側のローカル最新既知のウォーターマークと比較されます。 値が異なる場合は、クライアントがイベント通知を見逃しているし、ローカルの最新のウォーターマークを使用してサブスクリプションを再確立する必要があります。 たとえば、プッシュ クライアントは、1、2、および 3 の透かしを使用してサブスクリプションの 3 つのイベントを受け取るし、次の通知は、5 の**PreviousWatermark**値が付属しています、クライアントが少なくとも 1 つの通知が失われた、新しいサブスクリプションを作成する必要があります。透かしとして 3 を渡しています。 
  
クライアントの場合、プル、 **PreviousWatermark**の値になります GetEvents 呼び出しのクライアントが含まれている[ウォーターマーク](watermark.md)と同じです。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[サブスクライブ操作](subscribe-operation.md)
  
[GetEvents 操作](getevents-operation.md)
  
[Unsubscribe 操作](unsubscribe-operation.md)

