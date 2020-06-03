---
title: 対する modifiedevent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ModifiedEvent
api_type:
- schema
ms.assetid: ca1309f4-2df7-4289-811c-75c3db0e7072
description: "\"修飾\" 要素は、アイテムまたはフォルダーが変更されるイベントを表します。"
ms.openlocfilehash: 1a798773601a0857b9064c7fa6a532a7a36517ab
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468552"
---
# <a name="modifiedevent"></a>対する modifiedevent

"修飾" 要素は、アイテムまたはフォルダーが変更されるイベントを**表します。** 
  
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
|[Watermark](watermark.md) <br/> |メールボックスイベントテーブル内のイベントブックマークを表します。  <br/> |
|[示](timestamp.md) <br/> |変更されたアイテムまたはフォルダーのメールボックスイベントのタイムスタンプを表します。  <br/> |
|[FolderId](folderid.md) <br/> |変更されたフォルダーの識別子を表します。  <br/> |
|[ItemId](itemid.md) <br/> |変更されたアイテムの識別子を表します。  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |変更されたアイテムまたはフォルダーの親フォルダーの識別子を表します。  <br/> |
|[UnreadCount](unreadcount.md) <br/> |指定したフォルダー内の未読アイテムの数を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[通知](notification-ex15websvcsotherref.md) <br/> |サブスクリプションに関する情報、および前回の通知以降に発生したイベントに関する情報が含まれます。  <br/> |
   
## <a name="remarks"></a>注釈

フォルダー内のアイテムの変更ごとに、2つの変更されたイベントが生成されます。 変更されたアイテムに関連するイベントが1つあります。 その他のイベントは、アイテムの親フォルダーに関連しています。 これは、サブスクリプションが作成されたものと同じフォルダーです。 フォルダーに関連付けられているイベントを使用して、フォルダーの[UnreadCount](unreadcount.md)プロパティに対する潜在的な変更を通知します。 
  
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

