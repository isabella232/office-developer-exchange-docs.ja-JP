---
title: Item (UploadItemType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: ab7058f2-615f-4393-a0d4-af76727f37e9
description: Item 要素は、メールボックスにアップロードする 1 つのアイテムを表します。
ms.openlocfilehash: bd4681a19df2018db9e54ee39095cd602662650a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514446"
---
# <a name="item-uploaditemtype"></a>Item (UploadItemType)

**Item 要素** は、メールボックスにアップロードする 1 つのアイテムを表します。 
  
[UploadItems](uploaditems.md)
  
[Items (NonEmptyArrayOfUploadItemsType)](items-nonemptyarrayofuploaditemstype.md)
  
[Item (UploadItemType)](item-uploaditemtype.md)
  
```XML
<Item CreateAction="" IsAssociated="">
   <ParentFolderId/>
   <ItemId/>
   <Data/>
</Item>
```

 **UploadItemType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**CreateAction** <br/> |アイテムをメールボックスにアップロードするアクションを指定します。 この属性は必須です。  <br/> |
|**IsAssociated** <br/> |アップロードされたアイテムがフォルダー関連アイテムかどうかを指定します。 この属性はブール値です。 true の値 **は** 、アイテムがフォルダーに関連付けられているアイテムを示します。 この属性は省略可能です。  <br/> |
   
#### <a name="createaction-attribute"></a>CreateAction 属性

|**値**|**説明**|
|:-----|:-----|
|**CreateNew** <br/> |元のアイテムの新しいコピーがメールボックスにアップロードされるかどうかを示します。 [CreateNew 値](itemid.md)を使用する場合は、ItemId 要素を指定できません。 新しいアイテム識別子が応答で返されます。  <br/> |
|**Update** <br/> |**ItemId** 要素で示されるアイテムを更新する方法を指定します。 **ItemId** 要素が存在しない場合、または [ParentFolderId](parentfolderid.md)要素によって識別されるフォルダーにアイテムが存在しない場合は、エラーが返されます。  <br/> |
|**UpdateOrCreate** <br/> |アイテムの更新が最初に行われたかどうかを示します。 **ParentFolderId** 要素で指定されたフォルダーにアイテムが存在しない場合は、新しいアイテムが作成されます。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ParentFolderId](parentfolderid.md) <br/> |新しいアイテムが作成される親フォルダー、または更新するアイテムを含む親フォルダーの識別子を表します。  <br/> |
|[ItemId](itemid.md) <br/> |アイテムストアで作成または更新するアイテムの一意の識別子と変更キー Exchangeします。  <br/> |
|[Data (base64Binary)](data-base64binary.md) <br/> |メールボックスにアップロードする 1 つのアイテムのデータを格納します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Items (NonEmptyArrayOfUploadItemsType)](items-nonemptyarrayofuploaditemstype.md) <br/> |メールボックスにアップロードするアイテムの配列を含む。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web Services をホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[ExportItems 操作](exportitems-operation.md)
  
[UploadItems 操作](uploaditems-operation.md)

