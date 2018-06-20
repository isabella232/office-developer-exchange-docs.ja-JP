---
title: 名 (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: dce6d823-dc33-4a47-babe-6370a15ac7b4
description: Name 要素は、設定の名前を表します。
ms.openlocfilehash: 4689c306bb805a40fea0d58c9e04a5a47d3bb14d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832506"
---
# <a name="name-soap"></a>名 (SOAP)

**Name**要素は、設定の名前を表します。 
  
```XML
<Name/>
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
|[DomainSetting (SOAP)](domainsetting-soap.md) <br/> |[GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)要求によって返されるドメインの設定が含まれています。  <br/> |
|[DomainStringSetting (SOAP)](domainstringsetting-soap.md) <br/> |文字列型の値は、ドメインの設定を表します。  <br/> |
|[OrganizationRelationshipSettings (SOAP)](organizationrelationshipsettings-soap.md) <br/> |1 つの組織の組織との関係のリストを表します。  <br/> |
|[UserSetting (SOAP)](usersetting-soap.md) <br/> |1 つのユーザー設定を表します。  <br/> |
|[ProtocolConnectionCollectionSetting (SOAP)](protocolconnectioncollectionsetting-soap.md) <br/> |サーバー プロトコル接続の設定のコレクションを表します。  <br/> |
|[StringSetting (SOAP)](stringsetting-soap.md) <br/> |文字列型の値は、ユーザー設定を表します。  <br/> |
|[WebClientUrlCollectionSetting (SOAP)](webclienturlcollectionsetting-soap.md) <br/> |Exchange Web クライアントの Url のコレクションに設定されているユーザーを表します。  <br/> |
|[AlternateMailboxCollectionSetting (SOAP)](alternatemailboxcollectionsetting-soap.md) <br/> |代替メールボックスの設定のコレクションが含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

**Name**要素のテキスト値は、設定の名前です。 
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |スキーマの自動検出  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)
- [GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)
- [GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)
- [GetOrganizationRelationshipSettings 操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

