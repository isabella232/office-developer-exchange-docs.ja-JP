---
title: TokenIssuers (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 26c55228-184e-4340-bd80-f86be56f3e7a
description: TokenIssuers 要素は、TokenIssuer (SOAP) コレクションを表します。
ms.openlocfilehash: 68ff3ed515b346a84734596fae6fe127768b4476
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520403"
---
# <a name="tokenissuers-soap"></a>TokenIssuers (SOAP)

**TokenIssuers 要素は**[、TokenIssuer (SOAP) コレクションを表](tokenissuer-soap.md)します。 
  
```XML
<TokenIssuers>
    <TokenIssuer/>
</TokenIssuers>
```

 **TokenIssuers**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[TokenIssuer (SOAP)](tokenissuer-soap.md) <br/> |セキュリティ トークン サービス [の Uri (SOAP)](uri-soap.md) と [エンドポイント (SOAP)](endpoint-soap.md) を指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetFederationInformationResponse (SOAP)](getfederationinformationresponse-soap.md) <br/> |[GetFederationInformation 操作 (SOAP) 応答が含](getfederationinformation-operation-soap.md)まれる。  <br/> |
   
## <a name="remarks"></a>注釈

**TokenIssuers は**、自動検出で使用する [TokenIssuer (SOAP)](tokenissuer-soap.md)要素のコレクションを表します。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |正解  <br/> |
   
## <a name="see-also"></a>関連項目



[Exchange 用自動検出 Web サービス リファレンス](autodiscover-web-service-reference-for-exchange.md)
  
[SOAP 自動検出 XML 要素 (2013 Exchange)](soap-autodiscover-xml-elements-for-exchange-2013.md)

