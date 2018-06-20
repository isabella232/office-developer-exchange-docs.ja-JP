---
title: イベント
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
description: イベント要素は、クライアントに配信するキューにその他のイベントがあるかどうかを示します。
ms.openlocfilehash: cc3f7ed3b4b5f5ce27a9d45d508506bfa62e5086
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832489"
---
# <a name="moreevents"></a>イベント

**イベント**要素は、クライアントに配信するキューにその他のイベントがあるかどうかを示します。 
  
```xml
<MoreEvents/>
```

 **ブール型 (Boolean)**
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

テキスト値は、ブール値を表します。 **True**の場合より多くのイベントがキューにあることを示します。 **False**の値は、これ以上イベントがキューにあることを示します。 このプロパティは値の取得のみ可能です。 
  
## <a name="remarks"></a>備考

プルの通知の場合はこの要素の値が**true**を示しますクライアントに残りのイベントを取得する別の GetEvents 要求を発行すること。 仮定するとクライアントの仕様では、イベント通知の最小待機時間を必要とする、GetEvents 要求する必要がありますまで続行する継続的な連続、 **false** **イベント**の値が返されます。 
  
場合は、プッシュ通知**イベント**の**真**の値を示しますクライアントに別の通知要求が残りのイベントを提供するクライアントに送信されること。 プル通知と同様に、これらのフォロー アップの要求は引き続き継続的な連続してクライアント アクセス サーバー上のイベント キューが空になるまでです。 
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
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

