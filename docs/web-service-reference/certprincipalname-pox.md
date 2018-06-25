---
title: CertPrincipalName (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a24092c9-58be-4008-92c4-68ec5c6c0fa6
description: CertPrincipalName 要素は、SSL を使用して Microsoft Exchange Server 2007 組織に接続するために必要な Secure Sockets Layer (SSL) 証明書のプリンシパル名を指定します。
ms.openlocfilehash: d2766b16a3e8a1bcd013de332d9c07f709fcf949
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759618"
---
# <a name="certprincipalname-pox"></a>CertPrincipalName (POX)

**CertPrincipalName**要素は、SSL を使用して Microsoft Exchange Server 2007 組織に接続するために必要な Secure Sockets Layer (SSL) 証明書のプリンシパル名を指定します。 
  
[(POX) を自動検出](autodiscover-pox.md)
  
[応答 (POX)](response-pox.md)
  
[アカウント (POX)](account-pox.md)
  
[プロトコル (POX)](protocol-pox.md)
  
[CertPrincipalName (POX)](certprincipalname-pox.md)
  
```xml
<CertPrincipalName>none or servername</CertPrinicpalName>
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
|[プロトコル (POX)](protocol-pox.md) <br/> |クライアント アクセス サーバーの役割がインストールされている Exchange 2007 を実行しているコンピューターにクライアントを接続するための仕様が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、SSL を使用して Microsoft Exchange 組織に接続するために必要な SSL 証明書のプリンシパル名を指定します。
  
## <a name="remarks"></a>備考

**CertPrincipalName**要素が指定されていない場合、デフォルトは msstd:SERVER に設定されてサーバーと[サーバー (POX)](server-pox.md)要素で指定されている値があります。 たとえば、example.com としてサーバーを指定すると、 **CertPrincipalName**は空白のままに[SSL (POX)](ssl-pox.md)がオンに、 **CertPrincipalName**の既定値になります msstd:example.com。 
  
何も指定されて**いない**場合、Windows は MSDN で、[プリンシパル名](http://go.microsoft.com/fwlink/?LinkId=93417)」のトピックに含まれる情報に基づいて証明書のプリンシパル名を検証します。 
  
## <a name="see-also"></a>関連項目



[交換の POX の自動検出の XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

