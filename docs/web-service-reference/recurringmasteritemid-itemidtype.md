---
title: RecurringMasterItemId (ItemIdType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 48d831cf-10d8-480b-86d2-f9c0b14b8167
description: RecurringMasterItemId (ItemIdType) 要素は、関連するオカレンス アイテムの 1 つの識別子を識別することで、定期的なマスター アイテムを識別します。
ms.openlocfilehash: 491bb6686ad6cc9ee8169144b659d828e3920e45
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522741"
---
# <a name="recurringmasteritemid-itemidtype"></a>RecurringMasterItemId (ItemIdType)

**RecurringMasterItemId (ItemIdType)** 要素は、関連するオカレンス アイテムの 1 つの識別子を識別することで、定期的なマスター アイテムを識別します。 
  
```XML
<RecurringMasterItemId Id="" ChangeKey=""/>
```

 **ItemIdType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

****

|**属性**|**説明**|
|:-----|:-----|
|ID  <br/> |定期的なマスター アイテムの 1 回の出現を識別します。 この属性は必須です。  <br/> |
|ChangeKey  <br/> |定期的なマスター アイテムが 1 回出現する特定のバージョンを識別します。 また、定期的なマスター アイテムと 1 つのオカレンスに同じ変更キーが含まれるため、定期的なマスター アイテムも識別されます。 この属性は省略可能です。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[Reminder](reminder.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |正解  <br/> |
   
## <a name="see-also"></a>関連項目



[Reminder](reminder.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

