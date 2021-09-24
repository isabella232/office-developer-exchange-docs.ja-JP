---
title: ModifiedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ModifiedEvent
api_type:
- schema
ms.assetid: ca1309f4-2df7-4289-811c-75c3db0e7072
description: ModifiedEvent 要素は、アイテムまたはフォルダーが変更されるイベントを表します。
ms.openlocfilehash: 92002c2824168687e6984913dbf46ee85da921e7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539360"
---
# <a name="modifiedevent"></a>ModifiedEvent

**ModifiedEvent 要素** は、アイテムまたはフォルダーが変更されるイベントを表します。 
  
```xml
<ModifiedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
   <UnreadCount/>
</ModifiedEvent>
```

```xml
<ModifiedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/> 
   <ParentFolderId/>
   <UnreadCount/>
</ModifiedEvent>
```

**ModifiedEventType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Watermark](watermark.md) <br/> |メールボックス イベント テーブルのイベント ブックマークを表します。  <br/> |
|[TimeStamp](timestamp.md) <br/> |変更されたアイテムまたはフォルダー メールボックス イベントのタイムスタンプを表します。  <br/> |
|[FolderId](folderid.md) <br/> |変更されたフォルダーの識別子を表します。  <br/> |
|[ItemId](itemid.md) <br/> |変更されたアイテムの識別子を表します。  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |変更されたアイテムまたはフォルダーの親フォルダーの識別子を表します。  <br/> |
|[UnreadCount](unreadcount.md) <br/> |特定のフォルダー内の未読アイテムの数を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[通知](notification-ex15websvcsotherref.md) <br/> |サブスクリプションと、前回の通知以降に発生したイベントに関する情報が格納されます。  <br/> |
   
## <a name="remarks"></a>注釈

フォルダー内のアイテムの変更ごとに 2 つの変更イベントが生成されます。 1 つのイベントは、変更されたアイテムに関連します。 もう 1 つのイベントは、アイテムの親フォルダーに関連します。 これは、サブスクリプションが作成されたフォルダーと同じです。 フォルダーに関連付けられているイベントは、フォルダーの [UnreadCount](unreadcount.md) プロパティに潜在的な変更を伝えるのに使用されます。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [サブスクライブ操作](subscribe-operation.md)  
- [GetEvents 操作](getevents-operation.md)  
- [Unsubscribe 操作](unsubscribe-operation.md)

