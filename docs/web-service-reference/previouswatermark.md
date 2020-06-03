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
description: PreviousWatermark 要素は、サブスクリプションのためにクライアントに正常に伝達された最新のイベントのウォーターマークを表します。
ms.openlocfilehash: 1b26a645a5ec6dbbd2874b118f968866aadc32af
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461654"
---
# <a name="previouswatermark"></a>PreviousWatermark

**PreviousWatermark**要素は、サブスクリプションのためにクライアントに正常に伝達された最新のイベントのウォーターマークを表します。 
  
```xml
<PreviousWatermark/>
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
|[通知](notification-ex15websvcsotherref.md) <br/> |サブスクリプションに関する情報、および前回の通知以降に発生したイベントに関する情報が含まれます。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 Text 値は、最新のウォーターマークを表します。 テキスト値を空の文字列にすることはできません。
  
## <a name="remarks"></a>注釈

**PreviousWatermark**プロパティは、最後に成功した通知を判断するためにクライアントに役立ちます。 たとえば、サブスクリプションにウォーターマーク1、2、3の3つのイベントがあり、次の通知が**PreviousWatermark**値3で送信される場合、クライアントはこの値を、最後に受信した通知のウォーターマーク値と比較できます。 これにより、クライアントはイベントの連続性を確保できます。 
  
プッシュクライアントの場合、 **PreviousWatermark**は、ローカルのクライアント側の最後の既知のウォーターマークと比較されます。 値が異なる場合、クライアントはイベント通知を失ったため、最新のローカルウォーターマークを使用してサブスクリプションを再確立する必要があります。 たとえば、プッシュクライアントがウォーターマーク1、2、3を含むサブスクリプションに対して3つのイベントを受信し、次の通知の**PreviousWatermark**値が5である場合、クライアントは少なくとも1つの通知を失ったため、新しいサブスクリプションを作成して3をウォーターマークとして渡す必要があります。 
  
プルクライアントの場合、 **PreviousWatermark**の値は、GetEvents 呼び出しのクライアントによって含まれる[ウォーターマーク](watermark.md)と同じになります。 
  
この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[サブスクライブ操作](subscribe-operation.md)
  
[GetEvents 操作](getevents-operation.md)
  
[Unsubscribe 操作](unsubscribe-operation.md)

