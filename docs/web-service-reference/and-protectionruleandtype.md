---
title: および (ProtectionRuleAndType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- And
api_type:
- schema
ms.assetid: 7fafd1c8-cd29-43a0-b383-f6595f934f48
description: And 要素は、すべての子要素が true に評価されるように一致する必要があることを指定します。
ms.openlocfilehash: ba898ccd77518971afaf713d1c7c7955f46465d5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464736"
---
# <a name="and-protectionruleandtype"></a>および (ProtectionRuleAndType)

**And**要素は、すべての子要素が**true**に評価されるように一致する必要があることを指定します。
  
```xml
<And>
   <AllInternal/>
   <And/>
   <RecipientIs/>
   <SenderDepartments/>
   <True/>
</And>
```

 **ProtectionRuleAndType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[AllInternal](allinternal.md) <br/> |電子メールメッセージのすべての受信者が送信者の組織の内部にある場合は、 **true**に評価されます。  <br/> |
|**And** <br/> |**True**に評価するためにすべての子要素を一致させる必要があることを指定します。  <br/> |
|[RecipientIs](recipientis.md) <br/> |電子メールメッセージのすべての受信者が、子の[値 (ProtectionRuleValueType)](value-protectionrulevaluetype.md)要素で指定された受信者のいずれかと一致するように指定します。  <br/> |
|[SenderDepartments](senderdepartments.md) <br/> |送信者の部署が、子の[値 (ProtectionRuleValueType)](value-protectionrulevaluetype.md)要素で指定された部署のいずれかと一致することを指定します。  <br/> |
|[True](true.md) <br/> |常に一致する条件を指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[条件](condition.md) <br/> |実行するルールのアクション部分に対して満たす必要がある条件を指定します。  <br/> |
|**And** <br/> |**True**に評価するためにすべての子要素を一致させる必要があることを指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

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

