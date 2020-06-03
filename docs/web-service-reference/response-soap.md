---
title: 応答 (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 4c2bcdeb-95ce-4ffa-bd83-118af53b534f
description: Response 要素には、GetUserSettings 操作 (SOAP)、GetDomainSettings operation (SOAP)、または GetFederationInformation operation (SOAP) 要求への応答が含まれています。
ms.openlocfilehash: 90cb29dd4ce4026211a5b592f149c8190dc81d29
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456417"
---
# <a name="response-soap"></a>応答 (SOAP)

**Response**要素には、 [getusersettings 操作 (soap)](getusersettings-operation-soap.md)、 [GETDOMAINSETTINGS operation (Soap)](getdomainsettings-operation-soap.md)、または[GetFederationInformation operation (soap)](getfederationinformation-operation-soap.md)要求への応答が含まれています。 
  
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
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |自動検出サービスによって返されるエラーコードを表します。  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |自動検出サービスによって返されるエラーコードに関連付けられているメッセージを表します。  <br/> |
|[UserResponses (SOAP)](userresponses-soap.md) <br/> |要求された各ユーザーの構成設定が含まれます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetUserSettingsResponseMessage (SOAP)](getusersettingsresponsemessage-soap.md) <br/> |[Getusersettingsrequest (SOAP)](getusersettingsrequest-soap.md)への応答を定義します。 <br/> |
|[GetDomainSettingsResponseMessage (SOAP)](getdomainsettingsresponsemessage-soap.md) <br/> |[Getdomainsettingsrequest (SOAP)](getdomainsettingsrequest-soap.md)への応答を定義します。  <br/> |
|[GetFederationInformationResponseMessage (SOAP)](getfederationinformationresponsemessage-soap.md) <br/> |[GetFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md)への応答を定義します。  <br/> |
   
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



[GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)


[Exchange 用自動検出 Web サービス リファレンス](autodiscover-web-service-reference-for-exchange.md)
  
[Exchange 2013 の SOAP 自動検出 XML 要素](soap-autodiscover-xml-elements-for-exchange-2013.md)

