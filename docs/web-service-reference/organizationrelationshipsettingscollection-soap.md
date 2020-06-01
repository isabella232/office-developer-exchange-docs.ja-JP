---
title: 組織/リレーションシップ設定コレクション (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 33456abf-a1b6-46da-a864-3ec8af2780de
description: 組織のリレーションシップ要素は、クエリに一致する組織上の関係のリストを表します。 組織内で使用されるのは、組織内のすべてのオブジェクトのコレクションです。 この要素はクライアントによって使用されません。
ms.openlocfilehash: 52f84d932e74393a844f5f55fbd1d09bfb0a5d4e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462424"
---
# <a name="organizationrelationshipsettingscollection-soap"></a>組織/リレーションシップ設定コレクション (SOAP)

組織の**リレーションシップ要素は、クエリ**に一致する組織上の関係のリストを表します。 組織内で使用されるのは、組織内のすべてのオブジェクトの**コレクション**です。 この要素はクライアントによって使用されません。 
  
```XML
<OrganizationRelationshipSettingsCollection>
   <OrganizationRelationshipSettings/>
</OrganizationRelationshipSettingsCollection>
```

 **組織の Relationshiprelationshipsettingscollection**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[組織のリレーションシップ設定 (SOAP)](organizationrelationshipsettings-soap.md) <br/> |選択された組織と SMTP アドレスの組織上の関係のリストを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Response (Get組織関係) (SOAP)](response-getorganizationrelationshipsoap.md) <br/> |[Get組織の設定操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)応答情報が含まれています。  <br/> |
   
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



[Get組織の Relationshipsettings 操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

