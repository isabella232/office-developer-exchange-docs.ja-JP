---
title: SeekToConditionPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b3b86720-d086-47c3-94af-921fdd719edf
description: SeekToConditionPageItemView 要素は、検索の終了、検索、戻るには、最大のエントリと FindItem または FindConversation の検索に検索方向の開始インデックスを識別するために使用される条件を識別します。
ms.openlocfilehash: e95246079f8c6e7acffac1dabb278895265767d9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833328"
---
# <a name="seektoconditionpageitemview"></a>SeekToConditionPageItemView

**FindItem**または**FindConversation の最後の検索、検索、戻るには、最大のエントリ、および検索方向の開始インデックスを識別するために使用される条件を識別する**SeekToConditionPageItemView**要素**検索します。 
  
```XML
<SeekToConditionPageItemView BasePoint="" MaxEntriesReturned="">
   <Condition/>
</SeekToConditionPageItemView>
```

 **SeekToConditionPageViewType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|ベース ポイント  <br/> |**ベース ポイント**属性のテキスト値は、検索の開始位置から基本のポイントです。 **先頭**のテキスト値は、結果セットの先頭に、検索を開始することを示します。 **最後**のテキスト値は、結果セットの最後に、検索を開始することを示します。  <br/> |
|MaxEntriesReturned  <br/> |**MaxEntriesReturned**属性のテキスト値は、結果セットで返すことができるアイテムの最大数です。  <br/> |
   
### <a name="child-elements"></a>子要素

[条件 (RestrictionType)](condition-restrictiontype.md)
  
### <a name="parent-elements"></a>親要素

[FindConversation](findconversation.md) | [FindItem](finditem.md)
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空にすることができます。  <br/> |false  <br/> |
   

