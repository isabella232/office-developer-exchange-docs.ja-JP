---
title: その他のイベント
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoreEvents
api_type:
- schema
ms.assetid: 76a7ea58-a44f-49b8-baba-d21302d742ad
description: More Events 要素は、キュー内にクライアントに配信されるイベントが他にもあるかどうかを示します。
ms.openlocfilehash: fd12dd2e2e64ce1711e553ba5eb29bd0eb64c892
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462732"
---
# <a name="moreevents"></a>その他のイベント

More **events**要素は、キュー内にクライアントに配信されるイベントが他にもあるかどうかを示します。 
  
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
|[通知](notification-ex15websvcsotherref.md) <br/> |サブスクリプションに関する情報、および前回の通知以降に発生したイベントに関する情報が含まれます。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、ブール値を表します。 値が**true の場合**は、キューに追加されたイベントがあることを示します。 値が**false**の場合は、キューにこれ以上イベントがないことを示します。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。 
  
## <a name="remarks"></a>注釈

プル通知の場合、この要素の**true**値は、残りのイベントを取得するために別の GetEvents 要求を発行する必要があることをクライアントに示します。 クライアント仕様でイベント通知の最小待機時間が要求されていると仮定すると、GetEvents 要求**は、それ**よりも長い**イベント**値が返されるまで連続した連続で続行する必要があります。 
  
プッシュ通知の場合、[その他のイベントの**true**値] は、他の通知要求がクライアントに送信され、残りのイベントが配信されること**を示します**。 プル通知と同様に、これらのフォローアップ要求は、クライアントアクセスサーバーのイベントキューが空になるまで連続して継続して続行されます。 
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
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

