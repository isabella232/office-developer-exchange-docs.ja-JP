---
title: And (ProtectionRuleAndType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- And
api_type:
- schema
ms.assetid: 7fafd1c8-cd29-43a0-b383-f6595f934f48
description: And 要素は、すべての子要素が true に評価するために一致する必要がある場合に指定します。
ms.openlocfilehash: 01721b460d87d3282a1a793966b0259e0f1342dd
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518939"
---
# <a name="and-protectionruleandtype"></a>And (ProtectionRuleAndType)

**And 要素は**、すべての子要素が true に評価するために一致する必要がある場合に指定 **します**。
  
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
|[AllInternal](allinternal.md) <br/> |電子メール メッセージ **のすべての受信者** が送信者の組織の内部である場合は true と評価されます。  <br/> |
|**And** <br/> |true に評価するには、すべての子要素が一致 **する必要があります**。  <br/> |
|[RecipientIs](recipientis.md) <br/> |電子メール メッセージの受信者が、子 [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) 要素の指定された受信者と一致する値を指定します。  <br/> |
|[SenderDepartments](senderdepartments.md) <br/> |送信者の部署が、子 Value [(ProtectionRuleValueType)](value-protectionrulevaluetype.md) 要素の指定された部署と一致する必要があります。  <br/> |
|[True](true.md) <br/> |常に一致する条件を指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Condition](condition.md) <br/> |ルールのアクション 部分を実行するために満たす必要がある条件を識別します。  <br/> |
|**And** <br/> |true に評価するには、すべての子要素が一致 **する必要があります**。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

