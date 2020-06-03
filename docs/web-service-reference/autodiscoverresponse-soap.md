---
title: AutodiscoverResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 203a5ac3-ebd0-4514-acbe-bc1c74638127
description: AutodiscoverResponse (SOAP) 要素は、自動検出サービスによって返されるすべての応答の基本要素を表します。
ms.openlocfilehash: 81fd557578bde9552d07e24386c93903e44a9afa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463966"
---
# <a name="autodiscoverresponse-soap"></a>AutodiscoverResponse (SOAP)

**AutodiscoverResponse (SOAP)** 要素は、自動検出サービスによって返されるすべての応答の基本要素を表します。 
  
- [AutodiscoverResponse (SOAP)](autodiscoverresponse-soap.md)
  
```XML
<AutodiscoverResponse>
    <UserResponses/>
    <UserSettingErrors/>
    <UserSettings/>
</AutodiscoverResponse>

```

 **AutodiscoverResponse**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[UserResponses (SOAP)](userresponses-soap.md) <br/> |[Userresponse (SOAP)](userresponse-soap.md)要素のコレクションを表します。  <br/> |
|[UserSettingErrors (SOAP)](usersettingerrors-soap.md) <br/> |[Usersettingerror (SOAP)](usersettingerror-soap.md)要素のコレクションを表します。  <br/> |
|[UserSettings (SOAP)](usersettings-soap.md) <br/> |[Usersetting (SOAP)](usersetting-soap.md)要素のコレクションを表します。  <br/> |
   
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

- [GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)
- [GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)
- [GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)

