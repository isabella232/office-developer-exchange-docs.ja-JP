---
title: データ (base64Binary)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Data
api_type:
- schema
ms.assetid: 26d8c2d0-bed2-4aed-b381-20e2ace6892f
description: データ要素には、エクスポートされたアイテムを 1 つまたはメールボックスにアップロードするアイテムのデータが含まれています。
ms.openlocfilehash: 9560273e31a64edb2254489961733dfe7360ad01
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759902"
---
# <a name="data-base64binary"></a>データ (base64Binary)

**データ**要素には、エクスポートされたアイテムを 1 つまたはメールボックスにアップロードするアイテムのデータが含まれています。 
  
```XML
<Data/>
```

**xs:base64Binary**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ExportItemsResponseMessage](exportitemsresponsemessage.md) <br/> |状態および 1 つのメールボックス アイテムをエクスポートするのには要求の結果が含まれています。  <br/> |
|[項目 (UploadItemType)](item-uploaditemtype.md) <br/> |メールボックスにアップロードする 1 つの項目を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**データ**要素には、プロパティ名とメールボックスにアップロードするには、エクスポートされたアイテムの値が含まれています。 
  
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

- [ExportItems 操作](exportitems-operation.md)
- [UploadItems 操作](uploaditems-operation.md)

