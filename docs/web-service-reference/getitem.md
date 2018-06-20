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
description: GetItem 要素は、Exchange ストア内のメールボックスからアイテムを取得する要求を定義します。
ms.openlocfilehash: 39db141bad62c34bec5ae6a937ba94c2d1288090
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760780"
---
# <a name="getitem"></a>GetItem

**GetItem**要素は、Exchange ストア内のメールボックスからアイテムを取得する要求を定義します。 
  
```xml
<GetItem>
   <ItemShape/>
   <ItemIds/>
</GetItem>
```

 **GetItemType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[ItemShape](itemshape.md) <br/> |**GetItem**応答に含めるコンテンツ アイテムのプロパティを識別します。  <br/> |
|[Itemid](itemids.md) <br/> |アイテム、出現アイテム、および Exchange ストアから項目を取得するための定期的なマスター アイテムの一意の id が含まれています。 これらの項目は、連絡先、タスク、メッセージ、予定表アイテム、会議出席依頼、およびその他のメールボックス内の有効なアイテムを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>備考

MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目




  [GetItem 操作](getitem-operation.md)

