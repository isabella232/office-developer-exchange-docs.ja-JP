---
title: RecurringMasterItemId (ItemIdType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 48d831cf-10d8-480b-86d2-f9c0b14b8167
description: RecurringMasterItemId (ItemIdType) 要素は、関連するオカレンスアイテムの1つの識別子を識別することによって、定期的なアイテムのマスターアイテムを識別します。
ms.openlocfilehash: c725998ad3a728ef1f47ff6491592b461753b895
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468440"
---
# <a name="recurringmasteritemid-itemidtype"></a>RecurringMasterItemId (ItemIdType)

**RecurringMasterItemId (ItemIdType)** 要素は、関連するオカレンスアイテムの1つの識別子を識別することによって、定期的なアイテムのマスターアイテムを識別します。 
  
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
|ID  <br/> |定期的なアイテムのマスターアイテムの1つの発生を識別します。 この属性は必須です。  <br/> |
|ChangeKey  <br/> |定期的なアイテムの1つのオカレンスの特定のバージョンを識別します。 また、定期的なマスターアイテムと単一のオカレンスに同じ変更キーが含まれているため、これらも確認されます。 この属性は省略可能です。  <br/> |
   
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
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目



[Reminder](reminder.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

