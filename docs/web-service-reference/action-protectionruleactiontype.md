---
title: Action (ProtectionRuleActionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Action
api_type:
- schema
ms.assetid: ca090dec-e2c5-49c8-a057-8d1f2409147f
description: Action 要素は、ルールの条件部分が一致する場合に実行する必要があるアクションを識別します。
ms.openlocfilehash: 6ca051622bb05b2ae2690f6b32ee11662161a4c1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59534006"
---
# <a name="action-protectionruleactiontype"></a>Action (ProtectionRuleActionType)

**Action 要素は**、ルールの条件部分が一致する場合に実行する必要があるアクションを識別します。 
  
```xml
<Action Name="">
   <Argument/>
</Action>

```

 **ProtectionRuleActionType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**名前** <br/> |アクションの名前を識別します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Arg1 と Arg2 の値](argument.md) <br/> |アクションの引数を指定します。 指定したアクションで引数を指定する必要がなされない場合、この要素は発生しません。 アクションに 1 つ以上の引数が必要な場合、この要素は 1 つ以上発生する可能性があります。 **RightsProtectMessage アクションには**、1 つの引数が含まれる。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Rule](rule.md) <br/> |1 つの保護ルールが含まれる。  <br/> |
   
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

