---
title: 値 (ProtectionRuleValueType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Value
api_type:
- schema
ms.assetid: b039bd6e-2198-47cf-9c78-a5e8b9d51c98
description: 値要素は、1 つの受信者または送信者の部署を識別します。
ms.openlocfilehash: 6173f94dcfb83eafd62e35f185a5e8c669d50f6c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839975"
---
# <a name="value-protectionrulevaluetype"></a>値 (ProtectionRuleValueType)

**値**要素は、1 つの受信者または送信者の部署を識別します。 
  
```XML
<Value/>
```

**ProtectionRuleValueType**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[RecipientIs](recipientis.md) <br/> |電子メール メッセージの受信者と一致している**値**の子要素で指定した受信者のいずれかを指定します。  <br/> |
|[SenderDepartments](senderdepartments.md) <br/> |送信者の部署と一致している**値**の子要素で指定された部門のいずれかを指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素は空でない文字列の値を含める必要があります。
  
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

