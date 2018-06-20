---
title: 項目 (UploadItemType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ab7058f2-615f-4393-a0d4-af76727f37e9
description: Item 要素は、メールボックスにアップロードする 1 つの項目を表します。
ms.openlocfilehash: 8fecef9a2368a44e38633eb9fddaa8197620f6a1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832138"
---
# <a name="item-uploaditemtype"></a>項目 (UploadItemType)

**Item**要素は、メールボックスにアップロードする 1 つの項目を表します。 
  
[UploadItems](uploaditems.md)
  
[アイテム (NonEmptyArrayOfUploadItemsType)](items-nonemptyarrayofuploaditemstype.md)
  
[項目 (UploadItemType)](item-uploaditemtype.md)
  
```XML
<Item CreateAction="" IsAssociated="">
   <ParentFolderId/>
   <ItemId/>
   <Data/>
</Item>
```

 **UploadItemType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**CreateAction** <br/> |メールボックスにアイテムをアップロードするアクションを指定します。 この属性は、必要があります。  <br/> |
|**IsAssociated** <br/> |アップロードしたアイテムがフォルダーに関連付けられている項目であるかどうかを指定します。 この属性は、ブール値です。 **True**の場合、項目が項目に関連付けられているフォルダーであることを示します。 この属性は、省略可能です。  <br/> |
   
#### <a name="createaction-attribute"></a>CreateAction 属性

|**値**|**説明**|
|:-----|:-----|
|**CreateNew** <br/> |メールボックスを元のアイテムの新しいコピーがアップロードされたことを示します。 [ItemId](itemid.md)の要素に新しい値を使用する場合に存在できません。 新しい項目の識別子は、応答で返されます。  <br/> |
|**Update** <br/> |**ItemId**要素で指定された項目を更新することを指定します。 **ItemId**の要素が存在しない場合、または[ParentFolderId](parentfolderid.md)要素で指定されたフォルダーにアイテムが存在しない場合は、エラーが返されます。  <br/> |
|**UpdateOrCreate** <br/> |しようとしましたが最初の項目を更新することを示します。 **ParentFolderId**要素によって指定されたフォルダーにアイテムがない場合は、新しいアイテムが作成されます。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[ParentFolderId](parentfolderid.md) <br/> |新しい項目を作成または更新する項目を含む位置の親フォルダーの識別子を表します。  <br/> |
|[ItemId](itemid.md) <br/> |作成または Exchange ストア内で更新する項目の一意の識別子と変更キーが含まれています。  <br/> |
|[データ (base64Binary)](data-base64binary.md) <br/> |メールボックスにアップロードする 1 つの項目のデータが含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[アイテム (NonEmptyArrayOfUploadItemsType)](items-nonemptyarrayofuploaditemstype.md) <br/> |メールボックスにアップロードするには項目の配列が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[ExportItems 操作](exportitems-operation.md)
  
[UploadItems 操作](uploaditems-operation.md)

