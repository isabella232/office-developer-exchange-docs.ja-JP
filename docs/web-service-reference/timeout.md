---
title: Timeout
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Timeout
api_type:
- schema
ms.assetid: c2e1ca5a-6667-4f6f-aac4-89de33bddc54
description: Timeout 要素は、サブスクリプションがクライアントからの GetEvents 要求なしでアイドル状態を維持できる期間を分単位で表します。
ms.openlocfilehash: d0b5945f5d116e0ebb7a24a23970e785761fb0c9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59534168"
---
# <a name="timeout"></a>Timeout

**Timeout 要素** は、サブスクリプションがクライアントからの GetEvents 要求なしでアイドル状態を維持できる期間を分単位で表します。 
  
```xml
<Timeout/>
```

 **int**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[PullSubscriptionRequest](pullsubscriptionrequest.md) <br/> |プル ベースのイベント通知サブスクリプションのサブスクリプションを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素を使用する場合は、整数を表すテキスト値が必要です。 この要素に使用できる値は、1 ~ 1440 です。含まれます。 この要素は必須です。
  
## <a name="remarks"></a>注釈

サブスクリプションのタイムアウト タイマーは、成功した GetEvents 要求によってリセットされます。
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。 
  
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

