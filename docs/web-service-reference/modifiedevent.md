---
title: ModifiedEvent
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
description: ModifiedEvent 要素は、アイテムまたはフォルダーが変更されるイベントを表します。
ms.openlocfilehash: fb464fb0a270d8ca7d33d40e5425e260970b2f1e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832482"
---
# <a name="modifiedevent"></a>ModifiedEvent

**ModifiedEvent**要素は、アイテムまたはフォルダーが変更されるイベントを表します。 
  
```xml
<ModifiedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
   <UnreadCount/>
</ModifiedEvent>
```

 **ModifiedEventType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[透かし](watermark.md) <br/> |メールボックス イベント テーブル内のイベント ブックマークを表します。  <br/> |
|[タイムスタンプ](timestamp.md) <br/> |変更されたアイテムまたはフォルダーのメールボックス イベントのタイムスタンプを表します。  <br/> |
|[フォルダー Id](folderid.md) <br/> |変更されたフォルダーの識別子を表します。  <br/> |
|[ItemId](itemid.md) <br/> |変更されたアイテムの識別子を表します。  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |変更されたアイテムまたはフォルダーの親フォルダーの識別子を表します。  <br/> |
|[UnreadCount](unreadcount.md) <br/> |指定したフォルダー内の未読アイテムの数を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[通知](notification-ex15websvcsotherref.md) <br/> |サブスクリプションおよび最後の通知以降に発生したイベントに関する情報が含まれています。  <br/> |
   
## <a name="remarks"></a>備考

フォルダー内のアイテムの各変更に対して 2 つの変更イベントが生成されます。 1 つのイベントは、変更されたアイテムに関連します。 その他のイベントは、アイテムの親フォルダーに関連します。 これは、サブスクリプションが作成されたのと同じフォルダーです。 フォルダーの[UnreadCount](unreadcount.md)プロパティへの潜在的な変更を通信するためにこのフォルダーに関連付けられているイベントを使用します。 
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[サブスクライブ操作](subscribe-operation.md)
  
[GetEvents 操作](getevents-operation.md)
  
[Unsubscribe 操作](unsubscribe-operation.md)

