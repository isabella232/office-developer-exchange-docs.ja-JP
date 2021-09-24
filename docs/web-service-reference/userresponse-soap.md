---
title: UserResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 5007b1ba-bfcc-40d7-b1cb-e32fbaf54ffd
description: UserResponse 要素は、個々のユーザーに対する GetUserSettings 要求への応答を表します。
ms.openlocfilehash: 8def0183a5c2e212e80699a3c2f58c64f67ce690
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538542"
---
# <a name="userresponse-soap"></a>UserResponse (SOAP)

**UserResponse 要素** は、個々のユーザーに対する GetUserSettings 要求への応答を表します。 
  
```XML
<UserResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <RedirectTarget/>
   <UserSettingErrors/>
   <UserSettings/>
</UserResponse>
```

 **UserResponse**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |自動検出サービスによって返されるエラー コードを表します。  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |自動検出サービスによって返されるエラー コードに関連付けられているメッセージを表します。  <br/> |
|[RedirectTarget (SOAP)](redirecttarget-soap.md) <br/> |リダイレクト URL または電子メール アドレスのターゲットが含まれる。  <br/> |
|[UserSettingErrors (SOAP)](usersettingerrors-soap.md) <br/> |取得できない設定に関する情報のコレクションを表します。  <br/> |
|[UserSettings (SOAP)](usersettings-soap.md) <br/> |ユーザーに対して要求された設定。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ArrayOfUserResponse (SOAP)](arrayofuserresponse-soap.md) <br/> |ユーザー応答の配列を含む。  <br/> |
|[UserResponses (SOAP)](userresponses-soap.md) <br/> |要求された各ユーザーの構成設定が含まれる。  <br/> |
   
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |正解  <br/> |
   
## <a name="see-also"></a>関連項目



[SOAP 自動検出 XML 要素 (2013 Exchange)](soap-autodiscover-xml-elements-for-exchange-2013.md)

