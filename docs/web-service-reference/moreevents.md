---
title: MoreEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MoreEvents
api_type:
- schema
ms.assetid: 76a7ea58-a44f-49b8-baba-d21302d742ad
description: MoreEvents 要素は、キュー内にクライアントに配信されるイベントが多いかどうかを示します。
ms.openlocfilehash: 7a19349e406a7e55e52c8a8cf0c3febba0a7301b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521810"
---
# <a name="moreevents"></a>MoreEvents

**MoreEvents 要素** は、キュー内にクライアントに配信されるイベントが多いかどうかを示します。 
  
```xml
<MoreEvents/>
```

 **Boolean**
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

テキスト値はブール値を表します。 true の値 **は** 、キュー内のイベントが多く含むかどうかを示します。 false の **値は** 、キュー内にこれ以上イベントが発生しなかっているかどうかを示します。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。 
  
## <a name="remarks"></a>注釈

プル通知の場合、この要素のtrue 値は、残りのイベントを取得するために別の GetEvents 要求を発行する必要があるクライアントに示します。 クライアント仕様でイベント通知の最小待機時間が必要な場合、GetEvents 要求は、false **の MoreEvents** 値が返されるまで、継続的に続行する必要があります。 
  
プッシュ通知の場合 **、MoreEvents** の true 値は、残りのイベントを配信するために別の通知要求がクライアントに送信されるというメッセージをクライアントに示します。  プル通知と同様に、これらのフォローアップ要求は、クライアント アクセス サーバー上のイベント キューが空になるまで連続して続行されます。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
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

