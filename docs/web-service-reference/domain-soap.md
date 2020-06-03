---
title: ドメイン (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 849629a0-0467-422f-88f6-3b8a95c17bba
description: ドメイン要素には、GetFederationInformation 応答のフェデレーションドメインが含まれているか、または GetDomainSettings 要求で要求される構成設定がドメインに含まれています。
ms.openlocfilehash: f90c608ee1fc3356a227bca6411eaeff0c1e8b22
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456984"
---
# <a name="domain-soap"></a>ドメイン (SOAP)

**ドメイン**要素には、 **GetFederationInformation**応答のフェデレーションドメインが含まれているか、または**getdomainsettings**要求で要求される構成設定がドメインに含まれています。 
  
```XML
<Domain/> 
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
|[Domains (SOAP)](domains-soap.md) <br/> |**Getdomainsettings**操作または組織が**GetFederationInformation**操作でフェデレーションしたドメインで返される構成設定のドメインを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**Domain**要素のテキスト値は、ドメイン名を表します。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |はい  <br/> |
   

