---
title: DeletedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DeletedEvent
api_type:
- schema
ms.assetid: c4565eb4-b537-466c-b1ff-11602533812b
description: DeletedEvent 要素は、アイテムまたはフォルダーが削除されるイベントを表します。
ms.openlocfilehash: 601b09273fb0fe52a40079e63952a50f592eaf5c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510268"
---
# <a name="deletedevent"></a>DeletedEvent

**DeletedEvent** 要素は、アイテムまたはフォルダーが削除されるイベントを表します。 
  
```xml
<DeletedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
</DeletedEvent>
```

```xml
<DeletedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
</DeletedEvent>
```

**BaseObjectChangedEventType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Watermark](watermark.md) <br/> |メールボックス イベント テーブルのイベント ブックマークを表します。  <br/> |
|[TimeStamp](timestamp.md) <br/> |削除済みアイテムまたはフォルダー メールボックス イベントのタイムスタンプを表します。  <br/> |
|[FolderId](folderid.md) <br/> |削除されたフォルダーの識別子を表します。  <br/> |
|[ItemId](itemid.md) <br/> |削除されたアイテムの識別子を表します。  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |削除前の削除済みアイテムまたはフォルダーの親フォルダーの識別子を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[通知](notification-ex15websvcsotherref.md) <br/> |サブスクリプションと、前回の通知以降に発生したイベントに関する情報が格納されます。  <br/> |
   
## <a name="remarks"></a>注釈

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

