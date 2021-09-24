---
title: GetFederationInformationResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 2033c14f-dcc8-43c2-9fd9-a51946ec7055
description: GetFederationInformationResponse 要素には、GetFederationInformation 操作 (SOAP) 応答が含まれる。
ms.openlocfilehash: 20d00f047acae6c9eba1347ae7e8110656fefb4b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59529880"
---
# <a name="getfederationinformationresponse-soap"></a>GetFederationInformationResponse (SOAP)

**GetFederationInformationResponse** 要素には [、GetFederationInformation 操作 (SOAP) 応答が含](getfederationinformation-operation-soap.md)まれる。 
  
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
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |自動検出サービスによって返されるエラー コードを表します。  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |自動検出サービスによって返されるエラー コードに関連付けられているメッセージを表します。  <br/> |
|[ApplicationUri (SOAP)](applicationuri-soap.md) <br/> |アプリケーションの場所を定義します。  <br/> |
|[TokenIssuers (SOAP)](tokenissuers-soap.md) <br/> |セキュリティ トークン サービス識別子とエンドポイントを含むセキュリティ トークンのコレクションを表します。  <br/> |
|[Domains (SOAP)](domains-soap.md) <br/> |[GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md) **GetDomainSettings** 操作で返される構成、または組織が [GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md) **GetFederationInformation** 操作でフェデレーションしたドメインを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |正解  <br/> |
   
## <a name="see-also"></a>関連項目



[GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)

