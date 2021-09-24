---
title: 条件
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Condition
api_type:
- schema
ms.assetid: 0790a3f2-cb31-4036-a757-7821aa0722cb
description: Condition 要素は、ルールのアクション 部分を実行するために満たす必要がある条件を識別します。
ms.openlocfilehash: 80efb2121e813a966faf419233cac4d23e971bc6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512008"
---
# <a name="condition"></a>条件

**Condition 要素** は、ルールのアクション 部分を実行するために満たす必要がある条件を識別します。 
  
```xml
<Condition>
   <AllInternal/>
</Condition>
```

```xml
<Condition> 
    <SenderDepartments/> 
</Condition>
```

```xml
<Condition> 
    <True/> 
</Condition>
```

```xml
<Condition> 
    <Recipients/> 
</Condition>
```

```xml
<Condition> 
    <And/> 
</Condition>
```

**ProtectionRuleConditionType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[AllInternal](allinternal.md) <br/> |電子メール メッセージ **のすべての受信者** が送信者の組織の内部である場合は true と評価されます。  <br/> |
|[And (ProtectionRuleAndType)](and-protectionruleandtype.md) <br/> |true に評価するには、すべての子要素が一致 **する必要があります**。 複数の保護ルールの子条件が必要な場合に指定します。  <br/> |
|[RecipientIs](recipientis.md) <br/> |電子メール メッセージの受信者が、子 [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) 要素の指定された受信者と一致する値を指定します。  <br/> |
|[SenderDepartments](senderdepartments.md) <br/> |送信者の部署が、子 Value [(ProtectionRuleValueType)](value-protectionrulevaluetype.md) 要素の指定された部署と一致する必要があります。  <br/> |
|[True](true.md) <br/> |常に一致する条件を指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Rule](rule.md) <br/> |1 つの保護ルールが含まれる。  <br/> |
   
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

