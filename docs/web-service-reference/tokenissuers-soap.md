---
title: TokenIssuers (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 26c55228-184e-4340-bd80-f86be56f3e7a
description: TokenIssuers 要素は、TokenIssuer (SOAP) のコレクションを表します。
ms.openlocfilehash: b070d85b32d5bce8461ac4e930329f237885bad7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839720"
---
# <a name="tokenissuers-soap"></a>TokenIssuers (SOAP)

**TokenIssuers**要素は、 [TokenIssuer (SOAP)](tokenissuer-soap.md)のコレクションを表します。 
  
```XML
<TokenIssuers>
    <TokenIssuer/>
</TokenIssuers>
```

 **TokenIssuers**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[TokenIssuer (SOAP)](tokenissuer-soap.md) <br/> |セキュリティ トークン サービスの[Uri (SOAP)](uri-soap.md)または[端点 (SOAP)](endpoint-soap.md)を指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetFederationInformationResponse (SOAP)](getfederationinformationresponse-soap.md) <br/> |[GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)の応答が含まれています。  <br/> |
   
## <a name="remarks"></a>備考

**TokenIssuers**は、自動検出で使用される[TokenIssuer (SOAP)](tokenissuer-soap.md)要素のコレクションを表します。 
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |スキーマの自動検出  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目



[Exchange の自動検出 web サービスの参照](autodiscover-web-service-reference-for-exchange.md)
  
[Exchange 2013 の自動検出の XML 要素を SOAP](soap-autodiscover-xml-elements-for-exchange-2013.md)

