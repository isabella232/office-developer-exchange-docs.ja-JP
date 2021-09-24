---
title: RecurringMasterItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RecurringMasterItemId
api_type:
- schema
ms.assetid: 5800b58c-f3d7-4d8f-acc0-d13e02f4e258
description: RecurringMasterItemId 要素は、関連するオカレンス アイテムの 1 つの識別子を識別することで、定期的なマスター アイテムを識別します。
ms.openlocfilehash: d00794f2b5b1893e1829a3f09df9f3e88266964d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523630"
---
# <a name="recurringmasteritemid"></a>RecurringMasterItemId

**RecurringMasterItemId** 要素は、関連するオカレンス アイテムの 1 つの識別子を識別することで、定期的なマスター アイテムを識別します。 
  
```XML
<RecurringMasterItemId OccurrenceId="" ChangeKey="" />
```

 **RecurringMasterItemIdType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**OccurrenceId** <br/> |定期的なマスター アイテムの 1 回の出現を識別します。 この属性は必須です。  <br/> |
|**ChangeKey** <br/> |定期的なマスター アイテムが 1 回出現する特定のバージョンを識別します。 また、定期的なマスター アイテムと 1 つのオカレンスに同じ変更キーが含まれるため、定期的なマスター アイテムも識別されます。 この属性は省略可能です。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GlobalItemIds](globalitemids.md) <br/> |メールボックス内のすべての会話アイテムのアイテム識別子のコレクションを格納します。  <br/> |
|[ItemChange](itemchange.md) <br/> |アイテム識別子とアイテムに適用する更新プログラムが含まれています。 <br/> <br/> 次に、この要素の XPath 式を示します。 <br/> <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
|[ItemIds](itemids.md) <br/> | Exchange ストア内のアイテムの削除、送信、取得、移動、またはコピーに使用されるアイテム、オカレンス アイテム、および定期的なマスター アイテムの一意の ID をExchangeします。 <br/> <br/>  この要素の XPath 式を次に示します。  <br/><br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/>  `/MoveItem/ItemIds` <br/>  `/CopyItem//ItemIds` <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="example"></a>例

次の例では、識別子 56lkjh6 を使用して、定期的なマスター アイテムの 1 つを識別します。
  
```XML
<RecurringMasterItemId OccurrenceId="56lkjh6" />
```

## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [OccurrenceItemId](occurrenceitemid.md)
- [FindConversation 操作](findconversation-operation.md)

