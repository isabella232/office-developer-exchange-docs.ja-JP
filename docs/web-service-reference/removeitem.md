---
title: RemoveItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RemoveItem
api_type:
- schema
ms.assetid: 766878e3-9007-454f-8501-45139bc5c0e2
description: RemoveItem 要素は、MeetingCancellation メッセージを受信したとき、会議アイテムを削除するために使用される応答オブジェクトを表します。
ms.openlocfilehash: 6897363eba602e6a135ad255822197f9296dd44a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833108"
---
# <a name="removeitem"></a>RemoveItem

**RemoveItem**要素は、MeetingCancellation メッセージを受信したとき、会議アイテムを削除するために使用される応答オブジェクトを表します。 
  
```xml
<RemoveItem ObjectName="">
   <ReferenceItemId/>
</RemoveItem>
```

 **RemoveItemType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**ObjectName** <br/> |英語の文字列での RemoveItem 応答オブジェクトのクラスの名前を表します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[ReferenceItemId](referenceitemid.md) <br/> |RemoveItem 応答オブジェクトが参照する項目を識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[アイテム (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)の要素で識別されるフォルダーを作成する項目の配列が含まれています。  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Exchange ストア内のアイテムに関連付けられているすべての応答オブジェクトのコレクションが含まれています。  <br/> |
   
## <a name="remarks"></a>備考

 **RemoveItem**はの[MeetingCancellation](meetingcancellation.md)に対してのみ有効です。 それ以外の場合、エラーがスローされます。
  
> [!NOTE]
> 会議の取り消しの[ItemClass](itemclass.md)は、IPM.Schedule.Meeting.Canceled。 
  
の[MeetingRequest](meetingrequest.md)と関連付けられている[カレンダー項目](calendaritem.md)を削除する**での RemoveItem**の代わりに[DeclineItem](declineitem.md)の応答オブジェクトを使用します。
  
 **RemoveItem**を代理人アクセスはサポートされていません。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

