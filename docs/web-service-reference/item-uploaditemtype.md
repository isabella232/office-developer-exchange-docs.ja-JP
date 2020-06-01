---
title: Item (UploadItemType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ab7058f2-615f-4393-a0d4-af76727f37e9
description: Item 要素は、メールボックスにアップロードする単一のアイテムを表します。
ms.openlocfilehash: 82c0fdf89c06ddfb812c2b2f1899b589eedeb7d8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467551"
---
# <a name="item-uploaditemtype"></a>Item (UploadItemType)

**Item**要素は、メールボックスにアップロードする単一のアイテムを表します。 
  
[UploadItems](uploaditems.md)
  
[アイテム (NonEmptyArrayOfUploadItemsType)](items-nonemptyarrayofuploaditemstype.md)
  
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
|**CreateAction** <br/> |メールボックスにアイテムをアップロードするアクションを指定します。 この属性は必須です。  <br/> |
|**IsAssociated** <br/> |アップロードされたアイテムがフォルダーに関連付けられたアイテムであるかどうかを指定します。 この属性はブール値です。 値が**true の場合**は、アイテムがフォルダーに関連付けられたアイテムであることを示します。 この属性は省略可能です。  <br/> |
   
#### <a name="createaction-attribute"></a>CreateAction 属性

|**値**|**説明**|
|:-----|:-----|
|**CreateNew** <br/> |元のアイテムの新しいコピーがメールボックスにアップロードされることを示します。 CreateNew 値が使用されている場合、 [ItemId](itemid.md)要素を指定することはできません。 新しいアイテム識別子が応答で返されます。  <br/> |
|**Update** <br/> |**ItemId**要素によって指定されたアイテムが更新されるように指定します。 **ItemId**要素が存在しない場合、またはアイテムが[ParentFolderId](parentfolderid.md)要素によって識別されるフォルダー内に存在しない場合は、エラーが返されます。  <br/> |
|**UpdateOrCreate** <br/> |アイテムを更新するために最初に試行が行われたことを示します。 **ParentFolderId**要素によって指定されたフォルダーにアイテムが存在しない場合は、新しいアイテムが作成されます。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ParentFolderId](parentfolderid.md) <br/> |新しいアイテムが作成された、または更新するアイテムを含む親フォルダーの識別子を表します。  <br/> |
|[ItemId](itemid.md) <br/> |Exchange ストアで作成または更新するアイテムの一意識別子および変更キーが含まれています。  <br/> |
|[Data (base64Binary)](data-base64binary.md) <br/> |メールボックスにアップロードする1つのアイテムのデータを格納します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[アイテム (NonEmptyArrayOfUploadItemsType)](items-nonemptyarrayofuploaditemstype.md) <br/> |メールボックスにアップロードするアイテムの配列が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[ExportItems 操作](exportitems-operation.md)
  
[UploadItems 操作](uploaditems-operation.md)

