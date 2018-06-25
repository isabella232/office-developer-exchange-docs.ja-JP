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
description: 応答要素には、GetUserSettings 操作 (SOAP)、GetDomainSettings の操作 (SOAP)、または GetFederationInformation の操作 (SOAP) 要求への応答が含まれています。
ms.openlocfilehash: 240c8e1f904ad685b51c1f657b2bc18e14fd985e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833179"
---
# <a name="response-soap"></a>応答 (SOAP)

**応答**要素には、 [GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)、 [GetDomainSettings の操作 (SOAP)](getdomainsettings-operation-soap.md)、または[GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)要求への応答が含まれています。 
  
```XML
<Response>
   <ErrorCode/>
   <ErrorMessage/>
   <UserResponses/>
</Response>
```

 **GetUserSettingsResponse**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[エラー コード (SOAP)](errorcode-soap.md) <br/> |自動検出サービスによって返されるエラー コードを表します。  <br/> |
|[エラー メッセージ (SOAP)](errormessage-soap.md) <br/> |自動検出サービスによって返されるエラー コードに関連付けられているメッセージを表します。  <br/> |
|[UserResponses (SOAP)](userresponses-soap.md) <br/> |要求された各ユーザーの構成設定が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetUserSettingsResponseMessage (SOAP)](getusersettingsresponsemessage-soap.md) <br/> |[GetUserSettingsRequest (SOAP)](getusersettingsrequest-soap.md)への応答を定義します。 <br/> |
|[GetDomainSettingsResponseMessage (SOAP)](getdomainsettingsresponsemessage-soap.md) <br/> |[GetDomainSettingsRequest (SOAP)](getdomainsettingsrequest-soap.md)への応答を定義します。  <br/> |
|[GetFederationInformationResponseMessage (SOAP)](getfederationinformationresponsemessage-soap.md) <br/> |[GetFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md)への応答を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |スキーマの自動検出  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)


[Exchange の自動検出 web サービスの参照](autodiscover-web-service-reference-for-exchange.md)
  
[Exchange 2013 の自動検出の XML 要素を SOAP](soap-autodiscover-xml-elements-for-exchange-2013.md)

