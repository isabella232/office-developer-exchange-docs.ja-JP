---
title: PreviousWatermark
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PreviousWatermark
api_type:
- schema
ms.assetid: 474f4f7c-47da-47d4-8126-230012172fb5
description: PreviousWatermark 要素は、サブスクリプションのクライアントに正常に通信された最新のイベントの透かしを表します。
ms.openlocfilehash: c46e18c7a58405fe2149666531cb2af773110816
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543024"
---
# <a name="previouswatermark"></a>PreviousWatermark

**PreviousWatermark** 要素は、サブスクリプションのクライアントに正常に通信された最新のイベントの透かしを表します。 
  
```xml
<PreviousWatermark/>
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
|[通知](notification-ex15websvcsotherref.md) <br/> |サブスクリプションと、前回の通知以降に発生したイベントに関する情報が格納されます。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 テキスト値は、最新の透かしを表します。 テキスト値を空の文字列にすることはできません。
  
## <a name="remarks"></a>注釈

**PreviousWatermark プロパティ** は、クライアントが最後に成功した通知を決定する際に役立ちます。 たとえば、サブスクリプションに透かし 1、2、3 の 3 つのイベントが含まれる場合、次の通知が **PreviousWatermark** 値 3 で送信された場合、クライアントは、この値を最後に受信した通知の透かし値と比較できます。 これにより、クライアントはイベントの継続性を確保できます。 
  
プッシュ クライアントの場合 **、PreviousWatermark** はローカルのクライアント側の最後の既知の透かしと比較されます。 値が異なる場合、クライアントはイベント通知を見逃し、最新のローカル透かしを使用してサブスクリプションを再確立する必要があります。 たとえば、プッシュ クライアントが透かし 1、2、および 3 のサブスクリプションの 3 つのイベントを受信し、次の通知に **PreviousWatermark** 値 5 が付属している場合、クライアントは少なくとも 1 つの通知を見逃し、3 を透かしとして渡す新しいサブスクリプションを作成する必要があります。 
  
プル クライアントの場合 **、PreviousWatermark の値は、GetEvents** 呼び [](watermark.md)出しに含まれるクライアントによって含まれる透かしと同じです。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[サブスクライブ操作](subscribe-operation.md)
  
[GetEvents 操作](getevents-operation.md)
  
[Unsubscribe 操作](unsubscribe-operation.md)

