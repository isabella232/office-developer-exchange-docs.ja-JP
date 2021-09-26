---
title: SeekToConditionPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: b3b86720-d086-47c3-94af-921fdd719edf
description: SeekToConditionPageItemView 要素は、検索の終了、検索の開始インデックス、返す最大エントリ、および FindItem または FindConversation 検索の検索方向を識別するために使用される条件を識別します。
ms.openlocfilehash: 6f4797a6b90456a50922db1c829757711816273e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546106"
---
# <a name="seektoconditionpageitemview"></a>SeekToConditionPageItemView

**SeekToConditionPageItemView** 要素は、検索の終了、検索の開始インデックス、返す最大エントリ、**および FindItem** または **FindConversation** 検索の検索方向を識別するために使用される条件を識別します。 
  
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
|BasePoint  <br/> |BasePoint 属性の **テキスト値** は、検索が開始される基点です。 Start のテキスト **値は** 、検索が結果セットの先頭から始まるかどうかを示します。 End のテキスト **値は** 、検索が結果セットの末尾から始まるかどうかを示します。  <br/> |
|MaxEntriesReturned  <br/> |**MaxEntriesReturned** 属性のテキスト値は、結果セットで返されるアイテムの最大数です。  <br/> |
   
### <a name="child-elements"></a>子要素

[Condition (RestrictionType)](condition-restrictiontype.md)
  
### <a name="parent-elements"></a>親要素

[FindConversation](findconversation.md)  | [FindItem](finditem.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空の場合  <br/> |false  <br/> |
   

