---
title: 条件 (RestrictionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4fdb373e-bf1b-4cb0-bbfb-444c6c6cec50
description: 条件要素は、FindItem または FindConversation 操作の検索の終了を識別するために使用される条件を指定します。
ms.openlocfilehash: 513fc21be52a90698f1c292d6d20d7cdaab07371
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759646"
---
# <a name="condition-restrictiontype"></a>条件 (RestrictionType)

**条件**要素ではの**FindItem**または**FindConversation**操作の検索の終了を識別するために使用される条件を指定します。 
  
```XML
<Condition>
    <SearchExpression></SearchExpression>
</Condition>
```

 **RestrictionType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[SearchExpression](searchexpression.md) <br/> |制限内の代替要素を表す抽象型の要素です。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[SeekToConditionPageItemView](seektoconditionpageitemview.md) <br/> |の**FindItem**または**FindConversation**操作の検索の終了、検索、戻るには、最大のエントリ、および検索方向の開始インデックスを識別するために使用される条件を識別します。  <br/> |
   
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型のスキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

