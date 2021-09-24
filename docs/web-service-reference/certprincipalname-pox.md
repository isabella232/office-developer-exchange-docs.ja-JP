---
title: CertPrincipalName (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: a24092c9-58be-4008-92c4-68ec5c6c0fa6
description: CertPrincipalName 要素は、SSL を使用して Microsoft Exchange Server 2007 組織に接続するために必要な Secure Sockets Layer (SSL) 証明書プリンシパル名を指定します。
ms.openlocfilehash: 69ee49cdad09032c269ffbbcc918044daf61cb9b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523252"
---
# <a name="certprincipalname-pox"></a>CertPrincipalName (POX)

**CertPrincipalName** 要素は、SSL を使用して Microsoft Exchange Server 2007 組織に接続するために必要な Secure Sockets Layer (SSL) 証明書プリンシパル名を指定します。 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[CertPrincipalName (POX)](certprincipalname-pox.md)
  
```xml
<CertPrincipalName>none or servername</CertPrinicpalName>
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
|[Protocol (POX)](protocol-pox.md) <br/> |クライアント アクセス サーバーの役割がインストールされている 2007 年Exchangeコンピューターにクライアントを接続するための仕様が含まれている。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、SSL を使用して Microsoft 組織に接続するために必要Exchange SSL 証明書プリンシパル名を指定します。
  
## <a name="remarks"></a>注釈

**CertPrincipalName** 要素を指定しない場合、既定値は msstd:SERVER に設定されます。ここで、SERVER は Server [(POX)](server-pox.md)要素で指定された値です。 たとえば、SERVER が example.com として指定され **、CertPrincipalName** が SSL [(POX)](ssl-pox.md) をオンにした状態で空白の場合 **、CertPrincipalName** の既定値は msstd:example.com になります。 
  
何 **も** 指定しない場合Windows MSDN の 「プリンシパル名」のトピックに記載されている情報に従って証明書プリンシパル [名を検証](https://go.microsoft.com/fwlink/?LinkId=93417)します。 
  
## <a name="see-also"></a>関連項目



[POX 自動検出 XML 要素のExchange](pox-autodiscover-xml-elements-for-exchange.md)

