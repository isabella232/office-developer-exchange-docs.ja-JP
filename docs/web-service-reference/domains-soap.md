---
title: Domains (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5f81d1b7-c6a4-456f-9935-13d04a3d92d7
description: Domains 要素は、GetDomainSettings 操作 (SOAP) で返されるドメインコレクション、組織が GetFederationInformation 操作 (SOAP) に対してフェデレーションされているドメイン、または Getruleaction Relationshipsettings 操作 (SOAP) によって返される組織上の関係を持つドメインに相当します。
ms.openlocfilehash: c56fb72841776c0060c1300b52b2f6a06b1ec0ed
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526306"
---
# <a name="domains-soap"></a>Domains (SOAP)

**Domains**要素は、 [getdomainsettings 操作 (soap)](getdomainsettings-operation-soap.md)で返されるドメインコレクション、組織が[GetFederationInformation 操作 (soap)](getfederationinformation-operation-soap.md)に対してフェデレーションされているドメイン、または[getruleaction relationshipsettings 操作 (soap)](getorganizationrelationshipsettings-operation-soap.md)によって返される組織上の関係を持つドメインに相当します。
  
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
|[ドメイン (SOAP)](domain-soap.md) <br/> |単一のドメインを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetDomainSettingsRequest (SOAP)](getdomainsettingsrequest-soap.md) <br/> |[Getdomainsettings 操作 (SOAP)](getdomainsettings-operation-soap.md)要求を表します。  <br/> |
|[Response (GetFederationInformation) (SOAP)](response-getfederationinformationsoap.md) <br/> |[GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)応答情報を格納します。  <br/> |
|[Get組織の Relationshipsettingsrequest (SOAP)](getorganizationrelationshipsettingsrequest-soap.md) <br/> |[Get組織の設定操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)要求を表します。  <br/> |
   
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

- [GetDomainSettingsRequest (SOAP)](getdomainsettingsrequest-soap.md)  
- [GetFederationInformationResponse (SOAP)](getfederationinformationresponse-soap.md)

