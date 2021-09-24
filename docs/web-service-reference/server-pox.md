---
title: Server (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 0ce51644-7f3a-408c-a398-814439b658dc
description: Server 要素は、メール サーバーの名前を指定します。
ms.openlocfilehash: 13673364aff111e1f330121283738119bc6041a2
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517792"
---
# <a name="server-pox"></a>Server (POX)

**Server 要素** は、メール サーバーの名前を指定します。 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[Server (POX)](server-pox.md)
  
```xml
<Server/>
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

テキスト値は、サーバーを識別します。 POP3、SMTP、IMAP、NNTP などのプロトコルの場合、この値はホスト名または IP アドレスになります。 DAV や WEB などのプロトコルの場合、これは URL です。
  
## <a name="see-also"></a>関連項目



[POX 自動検出 XML 要素のExchange](pox-autodiscover-xml-elements-for-exchange.md)

