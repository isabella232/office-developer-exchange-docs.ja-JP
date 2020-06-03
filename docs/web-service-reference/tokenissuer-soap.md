---
title: TokenIssuer (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2d7be675-626c-4173-89e9-e32beef81ad5
description: TokenIssuer 要素は、security token service の Uri (SOAP) とエンドポイント (SOAP) を指定します。
ms.openlocfilehash: e9c0b4140de26c7ff05daf4e863b3e8a17fedc62
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526327"
---
# <a name="tokenissuer-soap"></a>TokenIssuer (SOAP)

**Tokenissuer**要素は、security token Service の[Uri (Soap)](uri-soap.md)と[エンドポイント (soap)](endpoint-soap.md)を指定します。 
  
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
|[Uri (SOAP)](uri-soap.md) <br/> |セキュリティトークンを発行したセキュリティトークンサービスの URI。  <br/> |
|[エンドポイント (SOAP)](endpoint-soap.md) <br/> |Web サービスエンドポイント URI。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[TokenIssuers 者 (SOAP)](tokenissuers-soap.md) <br/> |セキュリティトークンサービス[Uri (soap)](uri-soap.md)と[エンドポイント (soap)](endpoint-soap.md)のコレクションを表します。  <br/> |
   
## <a name="remarks"></a>注釈

**Tokenissuer**要素を使用して、セキュリティトークンを使用するときにセキュリティトークンサービスを指定します。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目



[Exchange 用自動検出 Web サービス リファレンス](autodiscover-web-service-reference-for-exchange.md)
  
[Exchange 2013 の SOAP 自動検出 XML 要素](soap-autodiscover-xml-elements-for-exchange-2013.md)

