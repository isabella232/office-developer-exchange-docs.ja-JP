---
title: TokenIssuer (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 2d7be675-626c-4173-89e9-e32beef81ad5
description: TokenIssuer 要素は、セキュリティ トークン サービスの Uri (SOAP) とエンドポイント (SOAP) を指定します。
ms.openlocfilehash: ea1c93493e4f47a6f2551c24586e54614f4f45e6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59527266"
---
# <a name="tokenissuer-soap"></a>TokenIssuer (SOAP)

**TokenIssuer 要素** は、セキュリティ トークン サービスの [Uri (SOAP)](uri-soap.md)と [エンドポイント (SOAP)](endpoint-soap.md)を指定します。 
  
```XML
<TokenIssuer>
   <Uri/>
   <Endpoint/>
</TokenIssuer>
```

 **TokenIssuer**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Uri (SOAP)](uri-soap.md) <br/> |セキュリティ トークンを発行したセキュリティ トークン サービスの URI。  <br/> |
|[Endpoint (SOAP)](endpoint-soap.md) <br/> |Web サービスエンドポイント URI。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[TokenIssuers (SOAP)](tokenissuers-soap.md) <br/> |セキュリティ トークン サービス Uri [(SOAP)](uri-soap.md) とエンドポイント [(SOAP) のコレクションを表します](endpoint-soap.md)。  <br/> |
   
## <a name="remarks"></a>注釈

**TokenIssuer 要素を使用** して、セキュリティ トークン を使用する場合のセキュリティ トークン サービスを指定します。 
  
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

