---
title: Get組織の Relationshipsettingsrequest (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 4e8aa3b3-4bfc-40c3-b96b-9f7062b09309
description: GetOrganizationRelationshipSettingsRequest 要素は、Get組織の設定操作 (SOAP) 操作の呼び出しのパラメーターを表します。 Get組織の設定要求要素は、内部使用のみを対象としています。 この要素はクライアントによって使用されません。
ms.openlocfilehash: 053bbb8cbe2ccdcf6d544ab1fc92bb81765997e1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44452735"
---
# <a name="getorganizationrelationshipsettingsrequest-soap"></a>Get組織の Relationshipsettingsrequest (SOAP)

**Getorganizationrelationshipsettingsrequest**要素は、 [Get組織の設定操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)操作の呼び出しのパラメーターを表します。 **Get組織**の設定要求要素は、内部使用のみを対象としています。 この要素はクライアントによって使用されません。 
  
```XML
<GetOrganizationRelationshipSettingsRequest>
   <Domains/>
</GetOrganizationRelationshipSettingsRequest>
```

 **Get組織の Relationshipsettingsrequest**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Domains (SOAP)](domains-soap.md) <br/> |ドメイン識別子のコレクションを表します。  <br/> |
|||
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目



[Get組織の Relationshipsettings 操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

