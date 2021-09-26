---
title: SMTPLast (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: f1aa8bd9-c6ac-41ac-8d2d-56fb20006005
description: SMTPLast 要素は、簡易メール転送プロトコル (SMTP) サーバーが SMTP サーバーを使用して電子メールを送信する前に電子メールをダウンロードする必要があるかどうかを指定します。
ms.openlocfilehash: ff1e47fa1e3ebd0267879cd596a3a559f2702943
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544683"
---
# <a name="smtplast-pox"></a>SMTPLast (POX)

**SMTPLast 要素** は、簡易メール転送プロトコル (SMTP) サーバーが SMTP サーバーを使用して電子メールを送信する前に電子メールをダウンロードする必要があるかどうかを指定します。 
  
- [AutoDiscover (POX)](autodiscover-pox.md)
  
- [Response (POX)](response-pox.md)
  
- [Account (POX)](account-pox.md)
  
- [Protocol (POX)](protocol-pox.md)
  
- [SMTPLast (POX)](smtplast-pox.md)
  
```xml
<SMTPLast>on or off</SMTPLast>
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
|[Protocol (POX)](protocol-pox.md) <br/> |クライアント アクセス サーバーの役割がインストールされている 2007 年Microsoft Exchange Serverコンピューターにクライアントを接続するための仕様が含まれている。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、SMTP サーバーを使用して電子メールを送信する前に、SMTP サーバーが電子メールをダウンロードする必要があるかどうかを指定します。 指定できる値は **オンと** オフ **です**。 既定値はオフ **です**。
  
## <a name="see-also"></a>関連項目

- [POX 自動検出 XML 要素のExchange](pox-autodiscover-xml-elements-for-exchange.md)

