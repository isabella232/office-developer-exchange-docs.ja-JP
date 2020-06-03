---
title: Data (base64Binary)
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
description: Data 要素には、1つのエクスポートされたアイテムまたはメールボックスにアップロードするアイテムのデータが含まれています。
ms.openlocfilehash: 43ee16ca7caf634756ca00a88715d9834adad92b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526971"
---
# <a name="data-base64binary"></a>Data (base64Binary)

**Data**要素には、1つのエクスポートされたアイテムまたはメールボックスにアップロードするアイテムのデータが含まれています。 
  
```XML
<Data/>
```

**xs: base64Binary**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ExportItemsResponseMessage](exportitemsresponsemessage.md) <br/> |1つのメールボックスアイテムをエクスポートする要求の状態と結果を格納します。  <br/> |
|[Item (UploadItemType)](item-uploaditemtype.md) <br/> |メールボックスにアップロードする単一のアイテムを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**Data**要素には、エクスポートされたアイテムまたはメールボックスにアップロードされるアイテムのプロパティ名と値が含まれています。 
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [ExportItems 操作](exportitems-operation.md)
- [UploadItems 操作](uploaditems-operation.md)

