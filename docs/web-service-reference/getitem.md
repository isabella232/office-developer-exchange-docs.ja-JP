---
title: GetItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItem
api_type:
- schema
ms.assetid: 769df8eb-9c72-48b5-a49f-82c6b86bc5fc
description: GetItem 要素は、Exchange ストア内のメールボックスからアイテムを取得するための要求を定義します。
ms.openlocfilehash: a02403ee84195a41387d5dbe1785ae6d12b47da5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458699"
---
# <a name="getitem"></a>GetItem

**GetItem**要素は、Exchange ストア内のメールボックスからアイテムを取得するための要求を定義します。 
  
```xml
<GetItem>
   <ItemShape/>
   <ItemIds/>
</GetItem>
```

 **GetItemType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ItemShape](itemshape.md) <br/> |**GetItem**応答に含めるアイテムのプロパティとコンテンツを識別します。  <br/> |
|[ItemIds](itemids.md) <br/> |Exchange ストアからアイテムを取得するために使用されるアイテム、オカレンスアイテム、定期的なマスターアイテムの一意の id が含まれています。 これらのアイテムは、メールボックス内の連絡先、タスク、メッセージ、予定表アイテム、会議出席依頼、およびその他の有効なアイテムを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目




  [GetItem 操作](getitem-operation.md)

