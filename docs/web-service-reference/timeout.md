---
title: Timeout
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Timeout
api_type:
- schema
ms.assetid: c2e1ca5a-6667-4f6f-aac4-89de33bddc54
description: タイムアウト要素は、サブスクリプションがクライアントからの GetEvents 要求なしアイドルを分単位で、期間を表します。
ms.openlocfilehash: 0a26002689e131959f09318b01d97ffb73b605f9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839698"
---
# <a name="timeout"></a>Timeout

**タイムアウト**要素は、サブスクリプションがクライアントからの GetEvents 要求なしアイドルを分単位で、期間を表します。 
  
```xml
<Timeout/>
```

 **int**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[PullSubscriptionRequest](pullsubscriptionrequest.md) <br/> |プル ベースのイベント通知サブスクリプションをサブスクリプションを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

整数値を表すテキスト値は、この要素を使用する場合に必要です。 この要素の値は、1 から 1440 の範囲です。 この要素は必須です。
  
## <a name="remarks"></a>備考

GetEvents 要求が成功して、サブスクリプションのタイムアウト タイマーがリセットされます。
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。 
  
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

