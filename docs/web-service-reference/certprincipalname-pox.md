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
description: CertPrincipalName 要素は、SSL を使用して Microsoft Exchange Server 2007 組織に接続するために必要な SSL (Secure Sockets Layer) 証明書プリンシパル名を指定します。
ms.openlocfilehash: fb2a1c8577bce41945b669be56f2a94a2c4dca26
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463343"
---
# <a name="certprincipalname-pox"></a>CertPrincipalName (POX)

**CertPrincipalName**要素は、ssl を使用して Microsoft Exchange Server 2007 組織に接続するために必要な Ssl (Secure Sockets layer) 証明書プリンシパル名を指定します。 
  
[自動検出 (POX)](autodiscover-pox.md)
  
[応答 (POX)](response-pox.md)
  
[アカウント (POX)](account-pox.md)
  
[プロトコル (POX)](protocol-pox.md)
  
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
|[プロトコル (POX)](protocol-pox.md) <br/> |クライアントアクセスサーバーの役割がインストールされている Exchange 2007 を実行しているコンピューターにクライアントを接続するための仕様が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、SSL を使用して Microsoft Exchange 組織に接続するために必要な SSL 証明書のプリンシパル名を指定します。
  
## <a name="remarks"></a>注釈

**CertPrincipalName**要素が指定されていない場合、既定で msstd: server が設定されます。ここで、Server は[server (POX)](server-pox.md)要素で指定された値です。 たとえば、SERVER が example.com として指定されていて、 [SSL (POX)](ssl-pox.md)が有効になっている場合、 **CertPrincipalName**を空白のままにすると、既定値の**CertPrincipalName**は msstd: example .com になります。 
  
**何も**指定されていない場合、WINDOWS は MSDN の[プリンシパル名](https://go.microsoft.com/fwlink/?LinkId=93417)のトピックに記載されている情報に従って、証明書のプリンシパル名を検証します。 
  
## <a name="see-also"></a>関連項目



[Exchange の POX 自動検出 XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

