---
title: 種類 (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 9a627244-554f-4223-b9d8-a601b81a4a1a
description: Type 要素は、構成されたメールアカウントの種類を識別します。
ms.openlocfilehash: ad3570094ebe28498dfdc375cf7fc255434ba20d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465101"
---
# <a name="type-pox"></a>種類 (POX)

**Type**要素は、構成されたメールアカウントの種類を識別します。 
  
[自動検出 (POX)](autodiscover-pox.md)
  
[応答 (POX)](response-pox.md)
  
[アカウント (POX)](account-pox.md)
  
[プロトコル (POX)](protocol-pox.md)
  
[種類 (POX)](type-pox.md)
  
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
|[プロトコル (POX)](protocol-pox.md) <br/> |クライアントを Exchange サーバーに接続するための仕様が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

Text 値は、メールアカウントの種類を表します。 次の表に、使用可能な値を示します。
  
|**値**|**説明**|
|:-----|:-----|
|EXCH  <br/> |サーバーへの接続に使用されるプロトコルは、Exchange RPC です。  <br/> |
|EXHTTP  <br/> |サーバーの RPC/HTTP 接続に接続するために使用されるプロトコル。  <br/> |
|引数  <br/> |サーバーへの接続に使用されるプロトコルは、RPC プロキシサーバーを使用する Exchange RPC over HTTP です。  <br/> これは、 [AccountType (POX)](accounttype-pox.md)要素が電子メールに設定されている場合にのみ適用されます。  <br/> |
|WEB  <br/> |Web ブラウザーから電子メールにアクセスするには、[サーバー (POX)](server-pox.md)要素で指定されている URL を使用します。  <br/> これは、 [AccountType (POX)](accounttype-pox.md)要素が電子メールに設定されている場合にのみ適用されます。  <br/> |
   
### <a name="version-differences"></a>バージョンの相違点

Office 365、Exchange Online、およびオンプレミスバージョンの Exchange は、サーバーが RPC/HTTP 接続を受け付けるように構成されており、クライアントに "ExHttpInfo" が含まれている[X ClientCanHandle](pox-autodiscover-request-for-exchange.md)ヘッダーが含まれている場合にのみ、build 15.00.0995.014 からの値を返します。 
  
## <a name="see-also"></a>関連項目



[Exchange の POX 自動検出 XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

