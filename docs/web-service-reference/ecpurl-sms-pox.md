---
title: EcpUrl-sms (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: f5e5e589-ee16-42a8-9cd4-ae3909fc869b
description: EcpUrl-sms 要素は、メールが有効なユーザーのショート メッセージ サービス (SMS) 設定にアクセスするために使用できる URL を生成するために、EcpUrl (POX) 要素の値と組み合わせ可能な部分 URL を指定します。
ms.openlocfilehash: b3926e1d8b4e15e72827e9cf0458bd64a02bd793
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538255"
---
# <a name="ecpurl-sms-pox"></a>EcpUrl-sms (POX)

**EcpUrl-sms** 要素は、メールが有効なユーザーのショート メッセージ サービス (SMS) 設定にアクセスするために使用できる URL を生成するために [、EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせ可能な部分 URL を指定します。 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[EcpUrl-sms (POX)](ecpurl-sms-pox.md)
  
```XML
<EcpUrl-sms/>
```

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Protocol (POX)](protocol-pox.md) <br/> |クライアント アクセス サーバーの役割がインストールされているクライアントを実行しているコンピューター Microsoft Exchange Server接続するための仕様が含まれている。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は [、EcpUrl (POX)](ecpurl-pox.md) 要素の値と組み合わせて、ユーザーの SMS 設定にアクセスするために使用できる URL を生成できる部分的な URL を表します。 
  
## <a name="remarks"></a>注釈

**EcpUrl-sms** 要素は **、Protocol** 要素の省略可能な子要素です。 
  
## <a name="see-also"></a>関連項目



[POX 自動検出 XML 要素のExchange](pox-autodiscover-xml-elements-for-exchange.md)

