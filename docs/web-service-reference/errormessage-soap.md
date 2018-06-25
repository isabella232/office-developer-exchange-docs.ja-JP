---
title: エラー メッセージ (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: b84dd664-4c49-42c9-a49f-2ec4a9f7588b
description: エラー メッセージ要素は、自動検出サービスによって返されるエラー コードに関連付けられているメッセージを表します。
ms.openlocfilehash: 888eedc9c7cbbd1aad5cba21e76d999699c7ed02
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760330"
---
# <a name="errormessage-soap"></a>エラー メッセージ (SOAP)

**エラー メッセージ**要素は、自動検出サービスによって返されるエラー コードに関連付けられているメッセージを表します。 
  
```XML
<ErrorMessage/>
```

 **string**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AutodiscoverResponse (SOAP)](autodiscoverresponse-soap.md) <br/> |自動検出サービスによって返されるすべての応答の基本型を表します。  <br/> |
|[DomainResponse (SOAP)](domainresponse-soap.md) <br/> |指定したドメインの指定された設定が含まれています。  <br/> |
|[GetDomainSettingsResponse (SOAP)](getdomainsettingsresponse-soap.md) <br/> |個々 のドメインの[GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)呼び出しへの応答が含まれています。  <br/> |
|[GetFederationInformationResponse (SOAP)](getfederationinformationresponse-soap.md) <br/> |[GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)要求への応答が含まれています。  <br/> |
|[応答 (SOAP)](response-soap.md) <br/> |[GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)要求への応答が含まれています。  <br/> |
|[UserSettingError (SOAP)](usersettingerror-soap.md) <br/> |ユーザー設定の取得中に返されるエラーを表します。  <br/> |
|[UserResponse (SOAP)](userresponse-soap.md) <br/> |個々 のユーザーに対して[GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)要求に対する応答を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、エラー メッセージを表します。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |スキーマの自動検出  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)
  
[GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)
  
[GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)

