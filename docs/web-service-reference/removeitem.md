---
title: RemoveItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RemoveItem
api_type:
- schema
ms.assetid: 766878e3-9007-454f-8501-45139bc5c0e2
description: RemoveItem 要素は、MeetingCancellation メッセージを受信するときに会議アイテムを削除するために使用される応答オブジェクトを表します。
ms.openlocfilehash: 4dbe9ede36bf6e3c008a2186cfe617519ecfae1f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517960"
---
# <a name="removeitem"></a>RemoveItem

**RemoveItem 要素は**、MeetingCancellation メッセージを受信するときに会議アイテムを削除するために使用される応答オブジェクトを表します。 
  
```xml
<RemoveItem ObjectName="">
   <ReferenceItemId/>
</RemoveItem>
```

 **RemoveItemType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**ObjectName** <br/> |RemoveItem 応答オブジェクト クラスの名前を英語の文字列として表します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ReferenceItemId](referenceitemid.md) <br/> |RemoveItem 応答オブジェクトが参照するアイテムを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)要素によって識別されるフォルダー内に作成するアイテムの配列を格納します。  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |ストア内のアイテムに関連付けられているすべての応答オブジェクトのコレクションをExchangeします。  <br/> |
   
## <a name="remarks"></a>注釈

 **RemoveItem** は [MeetingCancellation でのみ有効です](meetingcancellation.md)。 それ以外の場合は、エラーがスローされます。
  
> [!NOTE]
> 会議 [の取り消](itemclass.md) しの ItemClass は IPM です。Schedule.Meeting.Canceled。 
  
[MeetingRequest と関連](meetingrequest.md)付けられた [CalendarItem](calendaritem.md)を削除するには [、RemoveItem](declineitem.md)の代わりに DeclineItem 応答オブジェクト **を使用します**。
  
 **RemoveItem** は、代理人アクセスではサポートされていません。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

