---
title: Data (base64Binary)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Data
api_type:
- schema
ms.assetid: 26d8c2d0-bed2-4aed-b381-20e2ace6892f
description: Data 要素には、エクスポートされた 1 つのアイテムまたはメールボックスにアップロードするアイテムのデータが含まれる。
ms.openlocfilehash: 69e15746f17febb74a0ec2f56eef0eaa1e298015
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59535935"
---
# <a name="data-base64binary"></a>Data (base64Binary)

**Data 要素** には、エクスポートされた 1 つのアイテムまたはメールボックスにアップロードするアイテムのデータが含まれる。 
  
```XML
<Data/>
```

**xs:base64Binary**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ExportItemsResponseMessage](exportitemsresponsemessage.md) <br/> |1 つのメールボックス アイテムをエクスポートする要求の状態と結果を格納します。  <br/> |
|[Item (UploadItemType)](item-uploaditemtype.md) <br/> |メールボックスにアップロードする 1 つのアイテムを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**Data 要素** には、エクスポートされたアイテムまたはメールボックスにアップロードされるアイテムのプロパティ名と値が含まれます。 
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web Services をホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [ExportItems 操作](exportitems-operation.md)
- [UploadItems 操作](uploaditems-operation.md)

