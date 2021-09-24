---
title: POX 自動検出要求のExchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 75671b1d-f35b-497b-8d8c-706f3f2535fd
description: 自動検出要求には、ユーザーのクライアント アクセス構成のクエリが含まれる。
ms.openlocfilehash: 8a0960dcff21276baf723512befacc4eca35950f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523867"
---
# <a name="pox-autodiscover-request-for-exchange"></a>POX 自動検出要求のExchange

自動検出要求には、ユーザーのクライアント アクセス構成のクエリが含まれる。
  
## <a name="autodiscover-request-example"></a>自動検出要求の例

### <a name="description"></a>説明

次の XML 例は、自動検出要求本文を示しています。
  
### <a name="code"></a>コード

```XML
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
   <Request>
     <EMailAddress>user@contoso.com</EMailAddress>
     <AcceptableResponseSchema>https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
   </Request>
 </Autodiscover>
```

### <a name="request-headers"></a>要求ヘッダー

自動検出要求を送信する場合、次の HTTP ヘッダーは省略可能です。
  
**表 1.HTTP 要求ヘッダー**

|**ヘッダー**|**説明**|
|:-----|:-----|
|X-MapiHttpCapability  <br/> |存在し、"1" に設定されている場合は、クライアントが MAPI/HTTP プロトコルを使用してサーバーへの接続に使用できる情報を要求しています。 このヘッダーは、MAPI/HTTP プロトコルを実装するクライアントに適用できます。  <br/> |
|X-ClientCanHandle  <br/> |このヘッダーには、クライアントがサポートする機能のコンマ区切りリストが含まれています。 使用できる値は表 2 で指定します。  <br/> |
   
**表 2.X-ClientCanHandle ヘッダー値**

|**X-ClientCanHandle 値 (大文字と小文字を区別しない)**|**サーバーの最小バージョン**|**説明**|
|:-----|:-----|:-----|
|ネゴシエート  <br/> |15.00.0995.014  <br/> |この値が存在する場合、サーバーがネゴシエート認証を受け入れる構成の場合、サーバーは [AuthPackage (POX)](authpackage-pox.md) 要素の "Negotiate" の値を返します。 この値が存在しない場合、サーバーは **AuthPackage** 要素の "Negotiate" の値を返しません。  <br/> |
|ExHttpInfo  <br/> |15.00.0995.014  <br/> |この値が存在する場合、サーバーが RPC/HTTP 接続を受け入れするように構成されている場合、サーバーは Type [(POX)](protocol-pox.md) 要素が "EXHTTP" に設定されたプロトコル [(POX)](type-pox.md) 要素を返します。 この値が存在しない場合、サーバーは **Type** 要素が "EXHTTP" に設定された **Protocol** 要素を返しません。  <br/> |
   
### <a name="request-elements"></a>要求要素

要求本文では、次の要素が使用されます。
  
- [AutoDiscover (POX)](autodiscover-pox.md)
    
- [Request (POX)](request-pox.md)
    
- [AcceptableResponseSchema (POX)](acceptableresponseschema-pox.md)
    
- [EMailAddress (POX)](emailaddress-pox.md)
    
> [!NOTE]
> [LegacyDN (POX)](legacydn-pox.md)要素は[、EMailAddress (POX)](emailaddress-pox.md)要素の代わりとして使用できます。 
  
### <a name="version-differences"></a>バージョンの相違点

X-MapiHttpCapability ヘッダーは、ビルド 15.00.0847.032 (Exchange Server 2013 SP1) から始まる Exchange の Office 365、Exchange Online、およびオンプレミス バージョンで使用できます。
  
X-ClientCanHandle ヘッダーは、Office 365、Exchange Online、およびオンプレミスバージョンの Exchange ビルド 15.00.0995.014 から利用できます。
  
## <a name="see-also"></a>関連項目



[POX 自動検出応答のExchange](pox-autodiscover-response-for-exchange.md)


[Exchange 用 POX 自動検出 Web サービス リファレンス](pox-autodiscover-web-service-reference-for-exchange.md)
  
[POX 自動検出 XML 要素のExchange](pox-autodiscover-xml-elements-for-exchange.md)

