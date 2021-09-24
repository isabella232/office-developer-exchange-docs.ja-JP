---
title: RecurringMasterItemIdRanges
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 5c9c89b5-4ce8-437b-a332-fa7ed35c8388
description: RecurringMasterItemIdRanges 要素は、出現範囲の配列を指定します。
ms.openlocfilehash: 582cbe27d468c1ff7ec22f03ba9f6976d244e234
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59529371"
---
# <a name="recurringmasteritemidranges"></a>RecurringMasterItemIdRanges

**RecurringMasterItemIdRanges 要素は**、出現範囲の配列を指定します。 
  
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
|**Id** <br/> |Id 属性のテキスト **値** は、定期的なマスター アイテムの一意の識別子です。 これは文字列 **値** です。  <br/> |
|**ChangeKey** <br/> |ChangeKey 属性の **テキスト値** は、定期的なマスター アイテムの変更キーです。 これは文字列 **値** です。  <br/> |
   
### <a name="child-elements"></a>子要素

[Ranges](ranges.md)
  
### <a name="parent-elements"></a>親要素

[ItemIds](itemids.md)  | [GlobalItemIds](globalitemids.md)  | [DraftItemIds](draftitemids.md)  | [ContactIds](contactids.md)  | [GroupIds](groupids.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> ||
   

