---
title: Rule
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Rule
api_type:
- schema
ms.assetid: c30f3851-bd56-4473-9106-dc85e9619486
description: ルール要素には、1 つの保護ルールが含まれています。
ms.openlocfilehash: 9abbb70381c214211172d2d5ba1ed43ee4797f17
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833263"
---
# <a name="rule"></a>Rule

**ルール**要素には、1 つの保護ルールが含まれています。 
  
```XML
<Rule Name="" UserOverridable=="" Priority="">
   <Condition/>
   <Action/>
</Rule>
```

 **ProtectionRuleType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**名前** <br/> |ルールの名前を識別します。 1 の最小の長さと文字列型の必須の属性です。  <br/> |
|**UserOverridable** <br/> |ルールが必須かどうかを指定します。 ルールが必須の場合は、この属性値は**false を指定**する必要があります。 ブール型の必須の属性です。  <br/> |
|**Priority** <br/> |ルールの優先度を指定します。 1 の最小値を int 型の必須の属性です。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[条件](condition.md) <br/> |実行するルールのアクション部の満たされている必要がある条件を識別します。  <br/> |
|[アクション (ProtectionRuleActionType)](action-protectionruleactiontype.md) <br/> |ルールの条件部分と一致する場合、どのようなアクションを実行する必要がありますを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ルール](rules-ex15websvcsotherref.md) <br/> |保護規則の配列が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

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

