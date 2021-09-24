---
title: ErrorMessage (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: b84dd664-4c49-42c9-a49f-2ec4a9f7588b
description: ErrorMessage 要素は、自動検出サービスによって返されるエラー コードに関連付けられたメッセージを表します。
ms.openlocfilehash: ebaa20f796787862ce3438bd496e29f88cb6ec6a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517078"
---
# <a name="errormessage-soap"></a>ErrorMessage (SOAP)

**ErrorMessage** 要素は、自動検出サービスによって返されるエラー コードに関連付けられたメッセージを表します。 
  
```XML
<ErrorMessage/>
```

 **string**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AutodiscoverResponse (SOAP)](autodiscoverresponse-soap.md) <br/> |自動検出サービスによって返されるすべての応答の基本型を表します。  <br/> |
|[DomainResponse (SOAP)](domainresponse-soap.md) <br/> |指定したドメインの要求された設定が含まれる。  <br/> |
|[GetDomainSettingsResponse (SOAP)](getdomainsettingsresponse-soap.md) <br/> |個々のドメインの [GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md) 呼び出しに対する応答を格納します。  <br/> |
|[GetFederationInformationResponse (SOAP)](getfederationinformationresponse-soap.md) <br/> |[GetFederationInformation 操作 (SOAP) 要求への応答を格納](getfederationinformation-operation-soap.md)します。  <br/> |
|[Response (SOAP)](response-soap.md) <br/> |[GetUserSettings 操作 (SOAP) 要求に対する応答を格納](getusersettings-operation-soap.md)します。  <br/> |
|[UserSettingError (SOAP)](usersettingerror-soap.md) <br/> |ユーザー設定の取得中に返されるエラーを表します。  <br/> |
|[UserResponse (SOAP)](userresponse-soap.md) <br/> |個々のユーザーに対する [GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md) 要求への応答を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値はエラー メッセージを表します。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |正解  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)
  
[GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)
  
[GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)

