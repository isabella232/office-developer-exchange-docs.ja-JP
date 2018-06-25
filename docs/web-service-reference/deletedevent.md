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
ms.openlocfilehash: f06ca0727916f415c648e876f88bf7eacef5a5ff
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759969"
---
# <a name="deletedevent"></a>DeletedEvent

**DeletedEvent**要素は、アイテムまたはフォルダーが削除されるイベントを表します。 
  
```xml
<DeletedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
</DeletedEvent>
```

**BaseObjectChangedEventType**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[透かし](watermark.md) <br/> |メールボックス イベント テーブル内のイベント ブックマークを表します。  <br/> |
|[タイムスタンプ](timestamp.md) <br/> |アイテムまたはフォルダーの削除済みメールボックス イベントのタイムスタンプを表します。  <br/> |
|[フォルダー Id](folderid.md) <br/> |削除されたフォルダーの識別子を表します。  <br/> |
|[ItemId](itemid.md) <br/> |削除された項目の識別子を表します。  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |フォルダーを削除する前に、削除された項目の親フォルダーの識別子を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[通知](notification-ex15websvcsotherref.md) <br/> |サブスクリプションおよび最後の通知以降に発生したイベントに関する情報が含まれています。  <br/> |
   
## <a name="remarks"></a>備考

MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [サブスクライブ操作](subscribe-operation.md)  
- [GetEvents 操作](getevents-operation.md)  
- [Unsubscribe 操作](unsubscribe-operation.md)

