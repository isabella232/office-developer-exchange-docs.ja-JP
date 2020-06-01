---
title: EcpUrl-sms (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: f5e5e589-ee16-42a8-9cd4-ae3909fc869b
description: EcpUrl 要素は、EcpUrl (POX) 要素の値と組み合わせて、メールが有効なユーザーのショートメッセージサービス (SMS) の設定にアクセスするために使用できる URL を生成できる url の一部を指定します。
ms.openlocfilehash: 24f475e7f2d54fa565cc90796a983c0bd842e4da
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458685"
---
# <a name="ecpurl-sms-pox"></a>EcpUrl-sms (POX)

**EcpUrl**要素は、 [EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、メールが有効なユーザーのショートメッセージサービス (sms) の設定にアクセスするために使用できる url を生成できる url の一部を指定します。 
  
[自動検出 (POX)](autodiscover-pox.md)
  
[応答 (POX)](response-pox.md)
  
[アカウント (POX)](account-pox.md)
  
[プロトコル (POX)](protocol-pox.md)
  
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
|[プロトコル (POX)](protocol-pox.md) <br/> |クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、 [EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、ユーザーの SMS 設定にアクセスするために使用できる url を生成できる url の部分を表します。 
  
## <a name="remarks"></a>注釈

**EcpUrl**要素は、 **Protocol**要素のオプションの子要素です。 
  
## <a name="see-also"></a>関連項目



[Exchange の POX 自動検出 XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

