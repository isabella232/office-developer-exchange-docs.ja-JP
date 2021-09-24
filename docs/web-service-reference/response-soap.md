---
title: Response (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 4c2bcdeb-95ce-4ffa-bd83-118af53b534f
description: Response 要素には、GetUserSettings 操作 (SOAP)、GetDomainSettings 操作 (SOAP)、または GetFederationInformation 操作 (SOAP) 要求に対する応答が含まれる。
ms.openlocfilehash: d42014991db8e93f88b80bed97970f043290cfb1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512360"
---
# <a name="response-soap"></a>Response (SOAP)

**Response** 要素には [、GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md) [、GetDomainSettings 操作 (SOAP)、](getdomainsettings-operation-soap.md)[または GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)要求に対する応答が含まれる。 
  
```XML
<Response>
   <ErrorCode/>
   <ErrorMessage/>
   <UserResponses/>
</Response>
```

 **GetUserSettingsResponse**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |自動検出サービスによって返されるエラー コードを表します。  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |自動検出サービスによって返されるエラー コードに関連付けられているメッセージを表します。  <br/> |
|[UserResponses (SOAP)](userresponses-soap.md) <br/> |要求された各ユーザーの構成設定が含まれる。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetUserSettingsResponseMessage (SOAP)](getusersettingsresponsemessage-soap.md) <br/> |[GetUserSettingsRequest (SOAP) への応答を定義します。](getusersettingsrequest-soap.md) <br/> |
|[GetDomainSettingsResponseMessage (SOAP)](getdomainsettingsresponsemessage-soap.md) <br/> |[GetDomainSettingsRequest (SOAP) への応答を定義します](getdomainsettingsrequest-soap.md)。  <br/> |
|[GetFederationInformationResponseMessage (SOAP)](getfederationinformationresponsemessage-soap.md) <br/> |[GetFederationInformationRequest (SOAP) への応答を定義します](getfederationinformationrequest-soap.md)。  <br/> |
   
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



[GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)


[Exchange 用自動検出 Web サービス リファレンス](autodiscover-web-service-reference-for-exchange.md)
  
[SOAP 自動検出 XML 要素 (2013 Exchange)](soap-autodiscover-xml-elements-for-exchange-2013.md)

