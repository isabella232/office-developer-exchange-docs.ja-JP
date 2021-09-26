---
title: GetItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetItem
api_type:
- schema
ms.assetid: 769df8eb-9c72-48b5-a49f-82c6b86bc5fc
description: GetItem 要素は、メールボックス ストア内のメールボックスからアイテムを取得する要求Exchangeします。
ms.openlocfilehash: 7d5a7253db54fd67bb8e8772c2a5aedb86abdeee
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546232"
---
# <a name="getitem"></a>GetItem

**GetItem 要素は**、アイテム ストア内のメールボックスからアイテムを取得する要求Exchangeします。 
  
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
|[ItemShape](itemshape.md) <br/> |GetItem 応答に含めるアイテムのプロパティとコンテンツ **を識別** します。  <br/> |
|[ItemIds](itemids.md) <br/> |アイテム、オカレンス アイテム、およびアイテムをストアから取得するために使用される定期的なマスター アイテムの一意の id Exchangeします。 これらのアイテムは、メールボックス内の連絡先、タスク、メッセージ、予定表アイテム、会議出席依頼、その他の有効なアイテムを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetItem 操作](getitem-operation.md)

