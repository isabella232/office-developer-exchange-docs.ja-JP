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
description: RecurringMasterItemId 要素は、関連するオカレンスアイテムの1つの識別子を識別することによって、定期的なアイテムのマスターアイテムを識別します。
ms.openlocfilehash: 896a9ce95d619e7bb44c8158288bc4f62ce417d9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529883"
---
# <a name="recurringmasteritemid"></a>RecurringMasterItemId

**RecurringMasterItemId**要素は、関連するオカレンスアイテムの1つの識別子を識別することによって、定期的なアイテムのマスターアイテムを識別します。 
  
```XML
<RecurringMasterItemId OccurrenceId="" ChangeKey="" />
```

 **RecurringMasterItemIdType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**OccurrenceId** <br/> |定期的なアイテムのマスターアイテムの1つの発生を識別します。 この属性は必須です。  <br/> |
|**ChangeKey** <br/> |定期的なアイテムの1つのオカレンスの特定のバージョンを識別します。 また、定期的なマスターアイテムと単一のオカレンスに同じ変更キーが含まれているため、これらも確認されます。 この属性は省略可能です。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GlobalItemIds](globalitemids.md) <br/> |メールボックス内のすべての会話アイテムのアイテム識別子のコレクションが含まれています。  <br/> |
|[ItemChange](itemchange.md) <br/> |アイテム識別子と、アイテムに適用する更新を含みます。 <br/> <br/> この要素の XPath 式を次に示します。 <br/> <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
|[ItemIds](itemids.md) <br/> | Exchange ストア内のアイテムの削除、送信、取得、移動、またはコピーに使用されるアイテム、オカレンスアイテム、定期的なマスターアイテムの一意の id が含まれています。 <br/> <br/>  この要素の XPath 式は次のとおりです。  <br/><br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/>  `/MoveItem/ItemIds` <br/>  `/CopyItem//ItemIds` <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="example"></a>例

次の例では、56lkjh6 という識別子を持つオカレンスの1つを識別することによって、定期的なマスターアイテムを識別します。
  
```XML
<RecurringMasterItemId OccurrenceId="56lkjh6" />
```

## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [OccurrenceItemId](occurrenceitemid.md)
- [FindConversation 操作](findconversation-operation.md)

