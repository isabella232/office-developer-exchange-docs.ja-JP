---
title: (POX) の種類
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 9a627244-554f-4223-b9d8-a601b81a4a1a
description: 型要素は、構成済みのメール アカウントの種類を識別します。
ms.openlocfilehash: 6e1349769c6a5349304f576419e0c609d3edd9a0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839759"
---
# <a name="type-pox"></a>(POX) の種類

**型**要素は、構成済みのメール アカウントの種類を識別します。 
  
[(POX) を自動検出](autodiscover-pox.md)
  
[応答 (POX)](response-pox.md)
  
[アカウント (POX)](account-pox.md)
  
[プロトコル (POX)](protocol-pox.md)
  
[(POX) の種類](type-pox.md)
  
```XML
<Type>WEB or EXCH or EXPR or EXHTTP</Type>
```

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[プロトコル (POX)](protocol-pox.md) <br/> |クライアントを Exchange サーバーに接続するための仕様が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、メール アカウントの種類を表します。 次の表は、可能な値を一覧します。
  
|**値**|**説明**|
|:-----|:-----|
|EXCH  <br/> |サーバーへの接続に使用されるプロトコルは、Exchange RPC です。  <br/> |
|EXHTTP  <br/> |サーバーの RPC/HTTP 接続への接続に使用されるプロトコルです。  <br/> |
|EXPR  <br/> |サーバーへの接続に使用されるプロトコルでは、Exchange RPC over HTTP を RPC プロキシ サーバーを使用しています。  <br/> これは、 [AccountType (POX)](accounttype-pox.md)要素は、電子メールに設定されている場合にのみ適用されます。  <br/> |
|WEB  <br/> |電子メールは、[サーバー (POX)](server-pox.md)要素で指定されている URL を使用して Web ブラウザーからアクセスします。  <br/> これは、 [AccountType (POX)](accounttype-pox.md)要素は、電子メールに設定されている場合にのみ適用されます。  <br/> |
   
### <a name="version-differences"></a>バージョンの相違点

Office 365、Exchange Online では、および設置型バージョンの Exchange が始まるビルド 15.00.0995.014 の戻り値が"EXHTTP"のサーバーが RPC または HTTP 接続を受け付けるように構成し、クライアントには、 [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md)ヘッダーが含まれて 場合にのみです"ExHttpInfo"が含まれています。 
  
## <a name="see-also"></a>関連項目



[交換の POX の自動検出の XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

