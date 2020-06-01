---
title: InternalDomains (SmtpDomainList)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InternalDomains
api_type:
- schema
ms.assetid: 0f2cbb05-338d-4302-8871-a06e78b33f98
description: InternalDomains 要素は、組織の内部 SMTP ドメインのリストを識別します。
ms.openlocfilehash: ec7ef2d72ae922c751f8f50b72ff7d6b31b212ca
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459967"
---
# <a name="internaldomains-smtpdomainlist"></a>InternalDomains (SmtpDomainList)

**Internaldomains**要素は、組織の内部 SMTP ドメインのリストを識別します。 
  
```XML
<InternalDomains>
   <Domain/>
</InternalDomains>
```

 **SmtpDomainList**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ドメイン](domain.md) <br/> |単一の SMTP ドメインを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Mailヒント構成 (MailTipsServiceConfiguration)](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |メールヒントサービスのサービス構成情報が保存されています。  <br/> |
|[Protectionルールの構成](protectionrulesconfiguration.md) <br/> |保護ルールサービスのサービス構成情報が保存されています。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素は必須です。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

