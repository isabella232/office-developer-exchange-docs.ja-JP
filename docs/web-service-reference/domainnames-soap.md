---
title: DomainNames (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 79ffc3f9-25c4-40b5-84ce-09a3c5f892fa
description: DomainNames 要素は、ドメイン名のコレクションを表します。 DomainNames 要素は、内部使用のみを対象としています。 この要素はクライアントによって使用されません。
ms.openlocfilehash: 0b425b3cd4c0e7cb2427920d61feb04010a3b123
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458419"
---
# <a name="domainnames-soap"></a>DomainNames (SOAP)

**Domainnames**要素は、ドメイン名のコレクションを表します。 **Domainnames**要素は、内部使用のみを対象としています。 この要素はクライアントによって使用されません。 
  
```XML
<DomainNames>
    <Domains/>
</DomainNames>
```

 **DomainNames**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Domains (SOAP)](domains-soap.md) <br/> |[Getdomainsettings 操作 (soap](getdomainsettings-operation-soap.md))、 [GETFEDERATIONINFORMATION operation (soap)](getfederationinformation-operation-soap.md)、または[getruleaction relationshipsettings 操作 (soap)](getorganizationrelationshipsettings-operation-soap.md)から返されるドメインのコレクションを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[組織のリレーションシップ設定 (SOAP)](organizationrelationshipsettings-soap.md) <br/> |1つの組織の組織上の関係のリストを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素は、外部組織の SMTP ドメインを表します。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目

- [Get組織の Relationshipsettings 操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

