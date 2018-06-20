---
title: エラー コード (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5e5ec861-0191-4ecb-a906-47ce8ed96381
description: エラー コード要素は、自動検出サービスによって返されるエラー コードを表します。
ms.openlocfilehash: 2dd91cec4645325c02bc8588af0ee0547909b945
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760320"
---
# <a name="errorcode-soap"></a>エラー コード (SOAP)

**エラー コード**要素は、自動検出サービスによって返されるエラー コードを表します。 
  
```XML
<ErrorCode/>
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

テキスト値は、自動検出エラー応答のエラー コードを表します。 可能なテキスト要素の値、**エラー コード**を次の表に一覧します。 
  
|**エラー コードのテキスト値**|**説明**|
|:-----|:-----|
|NoError  <br/> |エラーはありませんでした。  <br/> |
|RedirectAddress  <br/> |呼び出し元は、自動検出によって返された電子メール アドレスのリダイレクトに従う必要があります。  <br/> |
|RedirectUrl  <br/> |呼び出し元は、自動検出によって返された URL のリダイレクトに従う必要があります。  <br/> |
|InvalidUser  <br/> |要求で渡されたユーザーが正しくありません。  <br/> |
|InvalidRequest  <br/> |要求が有効ではありません。  <br/> |
|InvalidSetting  <br/> |指定した設定が正しくありません。  <br/> |
|SettingIsNotAvailable  <br/> |指定した設定が使用可能ではありません。  <br/> |
|ServerBusy  <br/> |サーバは、要求を処理するがビジー状態です。  <br/> |
|InvalidDomain  <br/> |要求されたドメインが正しくありません。  <br/> |
|NotFederated  <br/> |組織は連合がないです。  <br/> |
|InternalServerError  <br/> |内部サーバー エラーが表示されます。  <br/> |
   
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

