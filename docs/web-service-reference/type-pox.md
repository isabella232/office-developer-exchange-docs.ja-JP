---
title: Type (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 9a627244-554f-4223-b9d8-a601b81a4a1a
description: Type 要素は、構成済みのメール アカウントの種類を識別します。
ms.openlocfilehash: bb92913071509fec46736341bce56b1a00730f6b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517526"
---
# <a name="type-pox"></a>Type (POX)

**Type 要素は**、構成済みのメール アカウントの種類を識別します。 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[Type (POX)](type-pox.md)
  
```XML
<Type>WEB or EXCH or EXPR or EXHTTP</Type>
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
|[Protocol (POX)](protocol-pox.md) <br/> |クライアントをサーバーに接続するための仕様Exchangeします。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、メール アカウントの種類を表します。 次の表に、使用可能な値を示します。
  
|**値**|**説明**|
|:-----|:-----|
|EXCH  <br/> |サーバーへの接続に使用されるプロトコルは、RPC Exchangeされます。  <br/> |
|EXHTTP  <br/> |サーバー RPC/HTTP 接続への接続に使用されるプロトコル。  <br/> |
|EXPR  <br/> |サーバーへの接続に使用されるプロトコルは、RPC Exchangeを使用して RPC over HTTP に対して実行されます。  <br/> これは [、AccountType (POX)](accounttype-pox.md) 要素が電子メールに設定されている場合にのみ適用されます。  <br/> |
|WEB  <br/> |サーバー [(POX)](server-pox.md) 要素で指定された URL を使用して、Web ブラウザーから電子メールにアクセスします。  <br/> これは [、AccountType (POX)](accounttype-pox.md) 要素が電子メールに設定されている場合にのみ適用されます。  <br/> |
   
### <a name="version-differences"></a>バージョンの相違点

Office 365、Exchange Online、およびビルド 15.00.0995.014 から始まる Exchange のオンプレミス バージョンは、サーバーが RPC/HTTP 接続を受け入れ、クライアントに "ExHttpInfo" を含む[X-ClientCanHandle](pox-autodiscover-request-for-exchange.md)ヘッダーが含まれている場合にのみ、"EXHTTP" の値を返します。 
  
## <a name="see-also"></a>関連項目



[POX 自動検出 XML 要素のExchange](pox-autodiscover-xml-elements-for-exchange.md)

