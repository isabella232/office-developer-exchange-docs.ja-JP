---
title: OrganizationRelationshipSettingsCollection (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 33456abf-a1b6-46da-a864-3ec8af2780de
description: OrganizationRelationshipSettingsCollection 要素は、クエリに一致する組織との関係のリストを表します。 OrganizationRelationshipSettingsCollection 要素は、内部使用のみ。 クライアントでは、この要素は使用されません。
ms.openlocfilehash: 18e71ce39d48598868d677a37d5ba439fa6d59c4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832663"
---
# <a name="organizationrelationshipsettingscollection-soap"></a>OrganizationRelationshipSettingsCollection (SOAP)

**OrganizationRelationshipSettingsCollection**要素は、クエリに一致する組織との関係のリストを表します。 **OrganizationRelationshipSettingsCollection**要素は、内部使用のみ。 クライアントでは、この要素は使用されません。 
  
```XML
<OrganizationRelationshipSettingsCollection>
   <OrganizationRelationshipSettings/>
</OrganizationRelationshipSettingsCollection>
```

 **OrganizationRelationshipSettingsCollection**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[OrganizationRelationshipSettings (SOAP)](organizationrelationshipsettings-soap.md) <br/> |選択した組織と SMTP アドレスの組織との関係の一覧を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[応答 (GetOrganizationRelationship) (SOAP)](response-getorganizationrelationshipsoap.md) <br/> |[GetOrganizationRelationshipSettings 操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)応答の情報が含まれています。  <br/> |
   
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



[GetOrganizationRelationshipSettings 操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

