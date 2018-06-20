---
title: TokenIssuer (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2d7be675-626c-4173-89e9-e32beef81ad5
description: TokenIssuer 要素は、セキュリティ トークン サービスの Uri (SOAP) または端点 (SOAP) を指定します。
ms.openlocfilehash: 1c267fc6cbfdadd471c568473cc9aeeafb43ae2d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839708"
---
# <a name="tokenissuer-soap"></a>TokenIssuer (SOAP)

**TokenIssuer**要素は、セキュリティ トークン サービスの[Uri (SOAP)](uri-soap.md)または[端点 (SOAP)](endpoint-soap.md)を指定します。 
  
```XML
<TokenIssuer>
   <Uri/>
   <Endpoint/>
</TokenIssuer>
```

 **TokenIssuer**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[Uri (SOAP)](uri-soap.md) <br/> |セキュリティ トークンを発行したセキュリティ トークン サービスの URI。  <br/> |
|[エンドポイント (SOAP)](endpoint-soap.md) <br/> |Web サービス エンドポイントの URI です。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[TokenIssuers (SOAP)](tokenissuers-soap.md) <br/> |[エンドポイント (SOAP)](endpoint-soap.md)セキュリティ トークン サービスの[Uri (SOAP)](uri-soap.md)のコレクションを表します。  <br/> |
   
## <a name="remarks"></a>備考

**TokenIssuer**要素を使用して、セキュリティ トークンを使用する場合は、セキュリティ トークン サービスを指定します。 
  
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

