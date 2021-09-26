---
title: RecipientIs
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RecipientIs
api_type:
- schema
ms.assetid: 5d2fd7ce-6137-4b3c-a716-c0218dcc8a09
description: RecipientIs 要素は、電子メール メッセージの受信者が、子 Value (ProtectionRuleValueType) 要素の指定された受信者と一致する値を指定します。
ms.openlocfilehash: 0bf9d96469c626ddc223b128a6d7fabebbfebc84
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542898"
---
# <a name="recipientis"></a>RecipientIs

**RecipientIs 要素** は、電子メール メッセージの受信者が、子 [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md)要素の指定された受信者と一致する値を指定します。 
  
```xml
<RecipientIs>   <Value/></RecipientIs>
```

 **ProtectionRuleRecipientIsType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) <br/> |受信者を識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Condition](condition.md) <br/> |ルールのアクション 部分を実行するために満たす必要がある条件を識別します。  <br/> |
|[And (ProtectionRuleAndType)](and-protectionruleandtype.md) <br/> |true に評価するには、すべての子要素が一致 **する必要があります**。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

