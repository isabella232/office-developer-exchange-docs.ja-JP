---
title: Domain (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 849629a0-0467-422f-88f6-3b8a95c17bba
description: Domain 要素は、GetFederationInformation 応答にフェデレーション ドメインを含むか、GetDomainSettings 要求で要求される構成設定をドメインに含む。
ms.openlocfilehash: a2e69dc845f9841931263fe90e39550bceb81ab8
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520823"
---
# <a name="domain-soap"></a>Domain (SOAP)

**Domain** 要素は **、GetFederationInformation** 応答にフェデレーション ドメインを含むか **、GetDomainSettings** 要求で要求される構成設定をドメインに含む。 
  
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
|[Domains (SOAP)](domains-soap.md) <br/> |**GetDomainSettings** 操作で返される構成設定、または **GetFederationInformation** 操作で組織がフェデレーションしたドメインを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

Domain 要素のテキスト **値** は、ドメイン名を表します。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |はい  <br/> |
   

