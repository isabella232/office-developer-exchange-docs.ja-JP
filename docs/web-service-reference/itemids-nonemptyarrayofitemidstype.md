---
title: Itemid (NonEmptyArrayOfItemIdsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemIds
api_type:
- schema
ms.assetid: e895782a-74fe-4216-8ac2-c3c88c4b232d
description: Itemid の要素には、メールボックスからエクスポートする項目を識別する項目 id の配列が含まれています。
ms.openlocfilehash: c6d48832c5435080c7cec8e43093ea60825b604a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832151"
---
# <a name="itemids-nonemptyarrayofitemidstype"></a>Itemid (NonEmptyArrayOfItemIdsType)

**Itemid**の要素には、メールボックスからエクスポートする項目を識別する項目 id の配列が含まれています。 
  
[ExportItems](exportitems.md)
  
[Itemid (NonEmptyArrayOfItemIdsType)](itemids-nonemptyarrayofitemidstype.md)
  
```XML
<ItemIds>
   <ItemId/>
</ItemIds>
```

 **NonEmptyArrayOfItemIdsType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[ItemId](itemid.md) <br/> |Exchange ストア内のアイテムの一意の識別子と変更キーが含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ExportItems](exportitems.md) <br/> |メールボックスからアイテムをエクスポートするための要求を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[ExportItems 操作](exportitems-operation.md)
  
[UploadItems 操作](uploaditems-operation.md)

