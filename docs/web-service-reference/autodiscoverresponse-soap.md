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
description: AutodiscoverResponse (SOAP) の要素は、自動検出サービスによって返されるすべての応答の基本要素を表します。
ms.openlocfilehash: b92a71deb77e2b1dee42d970e2dc43a56044487a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759476"
---
# <a name="autodiscoverresponse-soap"></a>AutodiscoverResponse (SOAP)

**AutodiscoverResponse (SOAP)** の要素は、自動検出サービスによって返されるすべての応答の基本要素を表します。 
  
- [AutodiscoverResponse (SOAP)](autodiscoverresponse-soap.md)
  
```XML
<AutodiscoverResponse>
    <UserResponses/>
    <UserSettingErrors/>
    <UserSettings/>
</AutodiscoverResponse>

```

 **AutodiscoverResponse**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[UserResponses (SOAP)](userresponses-soap.md) <br/> |[UserResponse (SOAP)](userresponse-soap.md)要素のコレクションを表します。  <br/> |
|[UserSettingErrors (SOAP)](usersettingerrors-soap.md) <br/> |[UserSettingError (SOAP)](usersettingerror-soap.md)要素のコレクションを表します。  <br/> |
|[ユーザー (SOAP)](usersettings-soap.md) <br/> |[UserSetting (SOAP)](usersetting-soap.md)要素のコレクションを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
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

- [GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)
- [GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)
- [GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)

