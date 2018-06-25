---
title: RecurringMasterItemId (ItemIdType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 48d831cf-10d8-480b-86d2-f9c0b14b8167
description: RecurringMasterItemId (ItemIdType) の要素は、その出現の関連する項目の 1 つの識別子を識別することによって、定期的な予定のマスター アイテムを識別します。
ms.openlocfilehash: 89089067963e99ac1a6cae6ea6e1e8350d148e82
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833010"
---
# <a name="recurringmasteritemid-itemidtype"></a>RecurringMasterItemId (ItemIdType)

**RecurringMasterItemId (ItemIdType)** の要素は、その出現の関連する項目の 1 つの識別子を識別することによって、定期的な予定のマスター アイテムを識別します。 
  
```XML
<RecurringMasterItemId Id="" ChangeKey=""/>
```

 **ItemIdType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

****

|**属性**|**説明**|
|:-----|:-----|
|ID  <br/> |マスターの定期的なアイテムの 1 回の発生を識別します。 この属性は、必要があります。  <br/> |
|ChangeKey  <br/> |マスターの定期的なアイテムの 1 回の特定のバージョンを識別します。 さらに、定期的なマスター アイテムは、1 回の会議と同じキーの変更が格納されるためにも識別されます。 この属性は、省略可能です。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[Reminder](reminder.md)
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目



[Reminder](reminder.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

