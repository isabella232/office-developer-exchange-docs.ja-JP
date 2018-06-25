---
title: AllInternal
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AllInternal
api_type:
- schema
ms.assetid: b7e5072f-5d9f-4ee0-b58b-4d75d878ea1c
description: AllInternal 要素は、電子メール メッセージのすべての受信者が送信者の組織に内部にある場合に、true に評価します。
ms.openlocfilehash: 0ffd4178e711e3117497eed682e3fd3e0594989b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759310"
---
# <a name="allinternal"></a>AllInternal

**AllInternal**要素は、電子メール メッセージのすべての受信者が送信者の組織に内部にある場合に**true**に評価されました。 
  
```xml
<AllInternal/>
```

 **ProtectionRuleAllInternalType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[条件](condition.md) <br/> |実行するルールのアクション部の満たされている必要がある条件を識別します。  <br/> |
|[(ProtectionRuleAndType)](and-protectionruleandtype.md) <br/> |すべての子要素と一致するが**true**と評価されるかを指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**AllInternal**要素を空にする必要があります。 
  
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

