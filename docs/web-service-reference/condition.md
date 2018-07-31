---
title: Condition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Condition
api_type:
- schema
ms.assetid: 0790a3f2-cb31-4036-a757-7821aa0722cb
description: 条件要素では、実行されるルールのアクション部の満たされている必要がある条件を識別します。
ms.openlocfilehash: d49f2984799b15c0499af59abecbb34abe15f7c3
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353561"
---
# <a name="condition"></a>Condition

**条件**要素では、実行されるルールのアクション部の満たされている必要がある条件を識別します。 
  
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

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[AllInternal](allinternal.md) <br/> |電子メール メッセージのすべての受信者が送信者の組織の内部場合は、 **true**に評価されます。  <br/> |
|[And (ProtectionRuleAndType)](and-protectionruleandtype.md) <br/> |すべての子要素と一致するが**true**と評価されるかを指定します。 保護ルール子の 1 つ以上の条件が存在する必要がありますを指定します。  <br/> |
|[RecipientIs](recipientis.md) <br/> |電子メール メッセージの受信者と一致している[値 (ProtectionRuleValueType)](value-protectionrulevaluetype.md)の子要素で指定した受信者のいずれかを指定します。  <br/> |
|[SenderDepartments](senderdepartments.md) <br/> |送信者の部署と一致している[値 (ProtectionRuleValueType)](value-protectionrulevaluetype.md)の子要素で指定された部門のいずれかを指定します。  <br/> |
|[True](true.md) <br/> |常に一致する条件を指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Rule](rule.md) <br/> |1 つの保護ルールが含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

