---
title: Value (ProtectionRuleValueType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Value
api_type:
- schema
ms.assetid: b039bd6e-2198-47cf-9c78-a5e8b9d51c98
description: Value 要素は、単一の受信者または送信者部門を識別します。
ms.openlocfilehash: 2c4bbdcb3364f0ef8f608469f0dc1b289c4eeaf6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541624"
---
# <a name="value-protectionrulevaluetype"></a>Value (ProtectionRuleValueType)

**Value 要素は**、単一の受信者または送信者部門を識別します。 
  
```XML
<Value/>
```

**ProtectionRuleValueType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[RecipientIs](recipientis.md) <br/> |電子メール メッセージの受信者が、子 Value 要素の指定された受信者と一致する値を **指定** します。  <br/> |
|[SenderDepartments](senderdepartments.md) <br/> |送信者の部署が、子 Value 要素の指定された部署と一致する場合に **指定** します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素には、文字列値が含まれている必要があります。
  
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

