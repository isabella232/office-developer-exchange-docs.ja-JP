---
title: Name (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: dce6d823-dc33-4a47-babe-6370a15ac7b4
description: Name 要素は、設定の名前を表します。
ms.openlocfilehash: 74e6d6b59d972d7230c23b38cd3f4a8591401bbd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466886"
---
# <a name="name-soap"></a>Name (SOAP)

**Name**要素は、設定の名前を表します。 
  
```XML
<Name/>
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
|[DomainSetting (SOAP)](domainsetting-soap.md) <br/> |[Getdomainsettings 操作 (SOAP)](getdomainsettings-operation-soap.md)要求によって返されるドメイン設定が保存されています。  <br/> |
|[DomainStringSetting (SOAP)](domainstringsetting-soap.md) <br/> |文字列型 (string) の値を設定するドメインを表します。  <br/> |
|[組織のリレーションシップ設定 (SOAP)](organizationrelationshipsettings-soap.md) <br/> |1つの組織の組織上の関係のリストを表します。  <br/> |
|[UserSetting (SOAP)](usersetting-soap.md) <br/> |1つのユーザー設定を表します。  <br/> |
|[ProtocolConnectionCollectionSetting (SOAP)](protocolconnectioncollectionsetting-soap.md) <br/> |サーバープロトコルの接続設定のコレクションを表します。  <br/> |
|[StringSetting (SOAP)](stringsetting-soap.md) <br/> |文字列型 (string) の値を設定するユーザーを表します。  <br/> |
|[WebClientUrlCollectionSetting (SOAP)](webclienturlcollectionsetting-soap.md) <br/> |Exchange Web クライアントの Url のコレクションであるユーザー設定を表します。  <br/> |
|[AlternateMailboxCollectionSetting (SOAP)](alternatemailboxcollectionsetting-soap.md) <br/> |代替メールボックス設定のコレクションを格納します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**Name**要素のテキスト値は、設定の名前です。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)
- [GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)
- [GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)
- [Get組織の Relationshipsettings 操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

