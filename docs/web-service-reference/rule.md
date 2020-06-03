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
description: Rule 要素には、1つの保護ルールが含まれています。
ms.openlocfilehash: 6c18a2bd026893cd333bc7007203abf04a6f0be7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465002"
---
# <a name="rule"></a>Rule

**Rule**要素には、1つの保護ルールが含まれています。 
  
```XML
<Rule Name="" UserOverridable=="" Priority="">
   <Condition/>
   <Action/>
</Rule>
```

 **ProtectionRuleType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**名前** <br/> |ルールの名前を識別します。 最小の長さが1の文字列型の必須属性。  <br/> |
|**UserOverridable** <br/> |ルールが必須であるかどうかを指定します。 ルールが必須の場合、この属性値は**false**にする必要があります。 Boolean 型の必須の属性。  <br/> |
|**[優先度]** <br/> |ルールの優先度を指定します。 最小値が1の int 型の必須属性。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[条件](condition.md) <br/> |実行するルールのアクション部分に対して満たす必要がある条件を指定します。  <br/> |
|[アクション (ProtectionRuleActionType)](action-protectionruleactiontype.md) <br/> |ルールの条件部分が一致する場合に実行する必要のあるアクションを指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ルール](rules-ex15websvcsotherref.md) <br/> |保護ルールの配列を格納します。  <br/> |
   
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

