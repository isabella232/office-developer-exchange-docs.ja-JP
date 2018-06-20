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
description: ドメイン要素は、GetFederationInformation 応答内のフェデレーション ドメインが含まれています。 または、対象の構成の設定が GetDomainSettings の要求で要求されたドメインが含まれています。
ms.openlocfilehash: 411ca866800322ef06eeecc2ab92adc6f711917c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760145"
---
# <a name="domain-soap"></a>ドメイン (SOAP)

**ドメイン**要素は、 **GetFederationInformation**応答内のフェデレーション ドメインが含まれています。 または、対象の構成の設定が**GetDomainSettings**の要求で要求されたドメインが含まれています。 
  
```XML
<Domain/> 
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
|[ドメイン (SOAP)](domains-soap.md) <br/> |対象の構成の設定が**GetDomainSettings**の操作で返されるドメインまたは組織は、 **GetFederationInformation**の操作でフェデレーション ドメインを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**ドメイン**要素のテキスト値は、ドメイン名を表します。 
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |スキーマの自動検出  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   

