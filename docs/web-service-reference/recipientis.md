---
title: RecipientIs
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecipientIs
api_type:
- schema
ms.assetid: 5d2fd7ce-6137-4b3c-a716-c0218dcc8a09
description: RecipientIs 要素は、電子メールメッセージのすべての受信者が、子の値 (ProtectionRuleValueType) 要素内の指定された受信者のいずれかと一致することを指定します。
ms.openlocfilehash: 8f27c4484ce310c62f9bab0e6ffeea2bfac1d3ef
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463882"
---
# <a name="recipientis"></a>RecipientIs

**RecipientIs**要素は、電子メールメッセージのすべての受信者が、子の[値 (ProtectionRuleValueType)](value-protectionrulevaluetype.md)要素内の指定された受信者のいずれかと一致することを指定します。 
  
```xml
<RecipientIs>   <Value/></RecipientIs>
```

 **Protection/の Pientistype**
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
|[条件](condition.md) <br/> |実行するルールのアクション部分に対して満たす必要がある条件を指定します。  <br/> |
|[および (ProtectionRuleAndType)](and-protectionruleandtype.md) <br/> |**True**に評価するためにすべての子要素を一致させる必要があることを示します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

