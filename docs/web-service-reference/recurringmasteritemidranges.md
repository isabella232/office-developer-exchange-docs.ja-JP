---
title: RecurringMasterItemIdRanges
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c9c89b5-4ce8-437b-a332-fa7ed35c8388
description: RecurringMasterItemIdRanges 要素は、発生範囲の配列を指定します。
ms.openlocfilehash: 784676844c5c58c65b8cc6177843bf26d351b7d9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528756"
---
# <a name="recurringmasteritemidranges"></a>RecurringMasterItemIdRanges

**RecurringMasterItemIdRanges**要素は、発生範囲の配列を指定します。 
  
```XML
<RecurringMasterItemIdRanges Id="" ChangeKey="">
   <Ranges/>
</RecurringMasterItemIdRanges>
```

 **RecurringMasterItemIdRangesType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**Id** <br/> |**Id**属性のテキスト値は、定期的なマスターアイテムの一意識別子です。 これは、**文字列型 (string** ) の値です。  <br/> |
|**ChangeKey** <br/> |**Changekey**属性のテキスト値は、定期的なマスターアイテムの変更キーです。 これは、**文字列型 (string** ) の値です。  <br/> |
   
### <a name="child-elements"></a>子要素

[Ranges](ranges.md)
  
### <a name="parent-elements"></a>親要素

[Itemids](itemids.md)  | [Globalitemids](globalitemids.md)  | [DraftItemIds](draftitemids.md)  | [ContactIds](contactids.md)  | [Groupids](groupids.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> ||
   

