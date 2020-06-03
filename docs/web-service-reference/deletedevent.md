---
title: DeletedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeletedEvent
api_type:
- schema
ms.assetid: c4565eb4-b537-466c-b1ff-11602533812b
description: DeletedEvent 要素は、アイテムまたはフォルダーが削除されるイベントを表します。
ms.openlocfilehash: 5eb0c947aacc592f81c595da2cc00bf4874f300b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526943"
---
# <a name="deletedevent"></a>DeletedEvent

**Deletedevent**要素は、アイテムまたはフォルダーが削除されるイベントを表します。 
  
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
|[Watermark](watermark.md) <br/> |メールボックスイベントテーブル内のイベントブックマークを表します。  <br/> |
|[示](timestamp.md) <br/> |削除されたアイテムまたはフォルダーのメールボックスイベントのタイムスタンプを表します。  <br/> |
|[FolderId](folderid.md) <br/> |削除されたフォルダーの識別子を表します。  <br/> |
|[ItemId](itemid.md) <br/> |削除されたアイテムの識別子を表します。  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |削除する前に削除されたアイテムまたはフォルダーの親フォルダーの識別子を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[通知](notification-ex15websvcsotherref.md) <br/> |サブスクリプションに関する情報、および前回の通知以降に発生したイベントに関する情報が含まれます。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [サブスクライブ操作](subscribe-operation.md)  
- [GetEvents 操作](getevents-operation.md)  
- [Unsubscribe 操作](unsubscribe-operation.md)

