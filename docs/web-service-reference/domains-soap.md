---
title: Domains (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 5f81d1b7-c6a4-456f-9935-13d04a3d92d7
description: Domains 要素は、GetDomainSettings 操作 (SOAP) で返されるドメイン コレクション、組織が GetFederationInformation 操作 (SOAP) でフェデレーションしたドメイン、または GetOrganizationRelationshipSettings 操作 (SOAP) によって返される組織関係を持つドメインを表します。
ms.openlocfilehash: 667b2611ce8b393252f9bdda6dd7ec201b605047
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538324"
---
# <a name="domains-soap"></a>Domains (SOAP)

Domains 要素は[、GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)で返されるドメイン コレクション、組織が[GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)でフェデレーションしたドメイン、[または GetOrganizationRelationshipSettings 操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)によって返される組織関係を持つドメインを表します。 
  
```XML
<Domains>
   <Domain/>
</Domains>
```

 **ドメイン**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Domain (SOAP)](domain-soap.md) <br/> |1 つのドメインを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetDomainSettingsRequest (SOAP)](getdomainsettingsrequest-soap.md) <br/> |[GetDomainSettings 操作 (SOAP) 要求を表](getdomainsettings-operation-soap.md)します。  <br/> |
|[Response (GetFederationInformation) (SOAP)](response-getfederationinformationsoap.md) <br/> |[GetFederationInformation 操作 (SOAP) 応答情報が](getfederationinformation-operation-soap.md)含まれる。  <br/> |
|[GetOrganizationRelationshipSettingsRequest (SOAP)](getorganizationrelationshipsettingsrequest-soap.md) <br/> |[GetOrganizationRelationshipSettings 操作 (SOAP) 要求を表](getorganizationrelationshipsettings-operation-soap.md)します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |正解  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetDomainSettingsRequest (SOAP)](getdomainsettingsrequest-soap.md)  
- [GetFederationInformationResponse (SOAP)](getfederationinformationresponse-soap.md)

