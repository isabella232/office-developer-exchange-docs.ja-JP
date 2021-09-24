---
title: AllInternal
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AllInternal
api_type:
- schema
ms.assetid: b7e5072f-5d9f-4ee0-b58b-4d75d878ea1c
description: 電子メール メッセージのすべての受信者が送信者の組織の内部である場合、AllInternal 要素は true と評価されます。
ms.openlocfilehash: 5ccc484de19449bc47a39f170f691649ae4beb7f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523230"
---
# <a name="allinternal"></a>AllInternal

電子メール メッセージのすべての受信者が送信者の組織の内部である場合 **、AllInternal** 要素は true と評価されます。 
  
```xml
<AllInternal/>
```

 **ProtectionRuleAllInternalType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Condition](condition.md) <br/> |ルールのアクション 部分を実行するために満たす必要がある条件を識別します。  <br/> |
|[And (ProtectionRuleAndType)](and-protectionruleandtype.md) <br/> |true に評価するには、すべての子要素が一致 **する必要があります**。  <br/> |
   
## <a name="text-value"></a>テキスト値

**AllInternal 要素は** 空である必要があります。 
  
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

