---
title: POX の自動検出要求の交換
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 75671b1d-f35b-497b-8d8c-706f3f2535fd
description: 自動検出要求には、ユーザーのクライアント アクセスの構成のクエリが含まれています。
ms.openlocfilehash: 48d6c30946e75936ed93a6f4507d8a8d3ae47d40
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832865"
---
# <a name="pox-autodiscover-request-for-exchange"></a>POX の自動検出要求の交換

自動検出要求には、ユーザーのクライアント アクセスの構成のクエリが含まれています。
  
## <a name="autodiscover-request-example"></a>自動検出要求の例

### <a name="description"></a>説明

次の XML の例では、自動検出の要求の本体を示します。
  
### <a name="code"></a>コード

```XML
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
   <Request>
     <EMailAddress>user@contoso.com</EMailAddress>
     <AcceptableResponseSchema>http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
   </Request>
 </Autodiscover>
```

### <a name="request-headers"></a>要求ヘッダー

自動検出要求を送信するとき、次の HTTP ヘッダーはオプションです。
  
**表 1 です。HTTP 要求のヘッダー**

|**Header**|**説明**|
|:-----|:-----|
|X MapiHttpCapability  <br/> |場合は存在し、設定を「1」に、クライアントが MAPI または HTTP プロトコルを使用してサーバーに接続するために使用する情報を要求していることを示します。 このヘッダーは、MAPI または HTTP プロトコルを実装するクライアントに適用されます。  <br/> |
|X ClientCanHandle  <br/> |このヘッダーには、クライアントをサポートする機能のコンマ区切りのリストが含まれています。 表 2 には、使用可能な値が指定されています。  <br/> |
   
**表 2 になります。X ClientCanHandle ヘッダー値**

|**X ClientCanHandle の値 (大文字)**|**サーバーの最小バージョン**|**説明**|
|:-----|:-----|:-----|
|交渉  <br/> |15.00.0995.014  <br/> |この値が存在する場合、サーバーは、サーバーは、ネゴシエート認証を受け付けるように構成されている場合[AuthPackage (POX)](authpackage-pox.md)の要素で"Negotiate"の値を返すは。 この値が存在しない場合は、サーバーでは、 **AuthPackage**要素では、"Negotiate"の値は返しません。  <br/> |
|ExHttpInfo  <br/> |15.00.0995.014  <br/> |この値が存在する場合、サーバーはサーバーが RPC または HTTP 接続を受け付けるように構成されている場合は、"EXHTTP"に設定[の種類 (POX)](type-pox.md)要素を持つ[プロトコル (POX)](protocol-pox.md)の要素を返します。 この値が存在しない場合は、サーバーには、"EXHTTP"に設定**の種類**の要素の**プロトコル**要素は返されません。  <br/> |
   
### <a name="request-elements"></a>要素を要求します。

次の要素は、要求の本体で使用されます。
  
- [(POX) を自動検出](autodiscover-pox.md)
    
- [要求 (POX)](request-pox.md)
    
- [AcceptableResponseSchema (POX)](acceptableresponseschema-pox.md)
    
- [EMailAddress (POX)](emailaddress-pox.md)
    
> [!NOTE]
> [LegacyDN (POX)](legacydn-pox.md)要素は、 [EMailAddress (POX)](emailaddress-pox.md)要素の代わりに使用できます。 
  
### <a name="version-differences"></a>バージョンの相違点

X MapiHttpCapability ヘッダーは、Exchange Online では、Office 365 で利用可能なとオンプレミスから Exchange のバージョンが 15.00.0847.032 (Exchange Server 2013 SP1) を構築します。
  
X ClientCanHandle ヘッダーは、Exchange Online では、Office 365 で利用可能なとオンプレミスから Exchange のバージョンが 15.00.0995.014 を構築します。
  
## <a name="see-also"></a>関連項目



[POX Exchange の自動検出の応答](pox-autodiscover-response-for-exchange.md)


[Exchange の POX の自動検出 web サービスの参照](pox-autodiscover-web-service-reference-for-exchange.md)
  
[交換の POX の自動検出の XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

