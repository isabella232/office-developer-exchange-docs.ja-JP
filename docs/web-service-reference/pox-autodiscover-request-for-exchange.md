---
title: POX Exchange の自動検出要求
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 75671b1d-f35b-497b-8d8c-706f3f2535fd
description: 自動検出要求には、ユーザーのクライアントアクセス構成に対するクエリが含まれています。
ms.openlocfilehash: b2138f9813c7b75aef9afb90089b9b874aac7532
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461668"
---
# <a name="pox-autodiscover-request-for-exchange"></a>POX Exchange の自動検出要求

自動検出要求には、ユーザーのクライアントアクセス構成に対するクエリが含まれています。
  
## <a name="autodiscover-request-example"></a>自動検出要求の例

### <a name="description"></a>説明

次の XML の例は、自動検出要求本文を示しています。
  
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

次の HTTP ヘッダーは、自動検出要求を送信するときにオプションです。
  
**表1HTTP 要求ヘッダー**

|**ヘッダー**|**説明**|
|:-----|:-----|
|MapiHttpCapability  <br/> |"1" に設定されている場合は、MAPI/HTTP プロトコルを使用してサーバーへの接続に使用できる情報をクライアントが要求していることを示します。 このヘッダーは、MAPI/HTTP プロトコルを実装するクライアントに適用されます。  <br/> |
|X-ClientCanHandle  <br/> |このヘッダーには、クライアントがサポートする機能のコンマ区切りリストが含まれています。 使用可能な値は表2で指定されています。  <br/> |
   
**表2X-ClientCanHandle ヘッダー値**

|**X-ClientCanHandle 値 (大文字と小文字を区別しない)**|**最小サーバーバージョン**|**説明**|
|:-----|:-----|:-----|
|取り決め  <br/> |15.00.0995.014  <br/> |この値が存在する場合、サーバーがネゴシエート認証を受け入れるように構成されている場合、サーバーは[Authpackage (POX)](authpackage-pox.md)要素で値 "Negotiate" を返します。 この値が指定されていない場合、サーバーは**Authpackage**要素に "Negotiate" という値を返しません。  <br/> |
|ExHttpInfo  <br/> |15.00.0995.014  <br/> |この値が存在する場合、サーバーは RPC/HTTP 接続を受け入れるように構成されている場合は、 [Type (POX)](type-pox.md)要素が "exhttp" に設定された[プロトコル (POX)](protocol-pox.md)要素を返します。 この値が指定されていない場合、サーバーは**Type**要素が "exhttp" に設定されている**Protocol**要素を返しません。  <br/> |
   
### <a name="request-elements"></a>Request 要素

要求本文では、次の要素が使用されます。
  
- [自動検出 (POX)](autodiscover-pox.md)
    
- [要求 (POX)](request-pox.md)
    
- [AcceptableResponseSchema (POX)](acceptableresponseschema-pox.md)
    
- [EMailAddress (POX)](emailaddress-pox.md)
    
> [!NOTE]
> [LegacyDN (POX)](legacydn-pox.md)要素は、 [EMailAddress (POX)](emailaddress-pox.md)要素の代わりに使用できます。 
  
### <a name="version-differences"></a>バージョンの相違点

MapiHttpCapability ヘッダーは、Office 365、Exchange Online、およびオンプレミスバージョンの Exchange (build 15.00.0847.032 (Exchange Server 2013 SP1) 以降で利用できます。
  
X-ClientCanHandle ヘッダーは、Office 365、Exchange Online、およびオンプレミスバージョンの Exchange で使用できます。これは、build 15.00.0995.014 から始まります。
  
## <a name="see-also"></a>関連項目



[POX Exchange の自動検出応答](pox-autodiscover-response-for-exchange.md)


[Exchange 用 POX 自動検出 Web サービス リファレンス](pox-autodiscover-web-service-reference-for-exchange.md)
  
[Exchange の POX 自動検出 XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

