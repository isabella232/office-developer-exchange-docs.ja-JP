---
title: SeekToConditionPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b3b86720-d086-47c3-94af-921fdd719edf
description: SeekToConditionPageItemView 要素は、検索の終了を識別するために使用される条件、検索の開始インデックス、返される最大エントリ、および FindItem または FindConversation 検索の検索方向を指定します。
ms.openlocfilehash: dbb073263740ccdf75367f85f672b7d5ec78f7a0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466837"
---
# <a name="seektoconditionpageitemview"></a>SeekToConditionPageItemView

**Seektoconditionpageitemview**要素は、検索の終了を識別するために使用される条件、検索の開始インデックス、返される最大エントリ、および**FindItem**または**findconversation**検索の検索方向を指定します。 
  
```XML
<SeekToConditionPageItemView BasePoint="" MaxEntriesReturned="">
   <Condition/>
</SeekToConditionPageItemView>
```

 **SeekToConditionPageViewType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|BasePoint  <br/> |**BasePoint**属性のテキスト値は、検索が開始されるベースポイントです。 **先頭**のテキスト値は、検索が結果セットの先頭から開始されることを示します。 テキスト値**End**は、検索が結果セットの末尾から開始されることを示します。  <br/> |
|MaxEntriesReturned  <br/> |**Maxん返され**た属性のテキスト値は、結果セットで返すことができるアイテムの最大数です。  <br/> |
   
### <a name="child-elements"></a>子要素

[条件 (RestrictionType)](condition-restrictiontype.md)
  
### <a name="parent-elements"></a>親要素

[Findconversation](findconversation.md)  | [FindItem](finditem.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空にすることができます。  <br/> |false  <br/> |
   

