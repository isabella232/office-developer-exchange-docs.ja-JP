---
title: RecurringMasterItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecurringMasterItemId
api_type:
- schema
ms.assetid: 5800b58c-f3d7-4d8f-acc0-d13e02f4e258
description: RecurringMasterItemId 要素は、その出現の関連する項目の 1 つの識別子を識別することによって、定期的な予定のマスター アイテムを識別します。
ms.openlocfilehash: ae59e33ece55d85435ece4c9030ccda32eb62eab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833015"
---
# <a name="recurringmasteritemid"></a>RecurringMasterItemId

**RecurringMasterItemId**要素は、その出現の関連する項目の 1 つの識別子を識別することによって、定期的な予定のマスター アイテムを識別します。 
  
```XML
<RecurringMasterItemId OccurrenceId="" ChangeKey="" />
```

 **RecurringMasterItemIdType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**OccurrenceId** <br/> |マスターの定期的なアイテムの 1 回の発生を識別します。 この属性は、必要があります。  <br/> |
|**変更キー** <br/> |マスターの定期的なアイテムの 1 回の特定のバージョンを識別します。 さらに、定期的なマスター アイテムは、1 回の会議と同じキーの変更が格納されるためにも識別されます。 この属性は、省略可能です。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GlobalItemIds](globalitemids.md) <br/> |メールボックス内のすべての会話項目の項目の識別子のコレクションが含まれています。  <br/> |
|[ItemChange](itemchange.md) <br/> |アイテム識別子と、アイテムに適用する更新プログラムが含まれています。 <br/> <br/> この要素への XPath 式は、次のようにします。 <br/> <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
|[Itemid](itemids.md) <br/> | アイテム、出現アイテム、および削除、送信、取得、移動、または Exchange ストア内のアイテムのコピーに使用される、マスターの定期的なアイテムの一意の id が含まれています。 <br/> <br/>  この要素への XPath 式は、次のように。  <br/><br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/>  `/MoveItem/ItemIds` <br/>  `/CopyItem//ItemIds` <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="example"></a>例

次の例では、その識別子の 56lkjh6 とのいずれかを識別することによって定期的なマスター アイテムを識別します。
  
```XML
<RecurringMasterItemId OccurrenceId="56lkjh6" />
```

## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [OccurrenceItemId](occurrenceitemid.md)
- 
  [FindConversation 操作](findconversation-operation.md)

