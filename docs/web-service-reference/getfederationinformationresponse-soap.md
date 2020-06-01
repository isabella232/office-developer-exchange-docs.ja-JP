---
title: GetFederationInformationResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 2033c14f-dcc8-43c2-9fd9-a51946ec7055
description: GetFederationInformationResponse 要素には、GetFederationInformation 操作 (SOAP) 応答が含まれています。
ms.openlocfilehash: c9e65a2b1759946b8493b3c730f08df6fe353fd8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460044"
---
# <a name="getfederationinformationresponse-soap"></a>GetFederationInformationResponse (SOAP)

**GetFederationInformationResponse**要素には、 [GETFEDERATIONINFORMATION 操作 (SOAP)](getfederationinformation-operation-soap.md)応答が含まれています。 
  
```XML
<GetFederationInformationResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <TokenIssuers/>
   <ApplicationUri/>
   <Domains/>
</GetFederationInformationResponse>
```

 **GetFederationInformationResponse**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |自動検出サービスによって返されるエラーコードを表します。  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |自動検出サービスによって返されるエラーコードに関連付けられているメッセージを表します。  <br/> |
|[ApplicationUri (SOAP)](applicationuri-soap.md) <br/> |アプリケーションの場所を定義します。  <br/> |
|[TokenIssuers 者 (SOAP)](tokenissuers-soap.md) <br/> |セキュリティトークンサービスの識別子とエンドポイントを含むセキュリティトークンのコレクションを表します。  <br/> |
|[Domains (SOAP)](domains-soap.md) <br/> |[Getdomainsettings 操作 (soap)](getdomainsettings-operation-soap.md)の**getdomainsettings**操作または組織が[GetFederationInformation operation (soap)](getfederationinformation-operation-soap.md) **GetFederationInformation**操作でフェデレーションを行ったドメインを表します。.  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目



[GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)

