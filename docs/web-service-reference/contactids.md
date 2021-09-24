---
title: ContactIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: c444f818-412b-41ac-9523-50246e50eae0
description: ContactIds 要素には、連絡先アイテム識別子の配列が含まれる。
ms.openlocfilehash: 05c26af6dc1a5b826025e4145116d3df5eee8d62
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59529218"
---
# <a name="contactids"></a>ContactIds

**ContactIds 要素には**、連絡先アイテム識別子の配列が含まれる。 
  
```XML
<ContactIds>
   <ItemId/>
   <OccurrenceItemId/>
   <RecurringMasterItemId/>
   <RecurringMasterItemIdRanges/>
</ContactIds>
```

 **NonEmptyArrayOfBaseItemIdsType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[ItemId](itemid.md)  | [OccurrenceItemId](occurrenceitemid.md)  | [RecurringMasterItemId](recurringmasteritemid.md)  | [RecurringMasterItemIdRanges](recurringmasteritemidranges.md)
  
### <a name="parent-elements"></a>親要素

[GetImItems](getimitems.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空の場合  <br/> |false  <br/> |
   

