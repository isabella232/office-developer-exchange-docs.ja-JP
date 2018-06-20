---
title: CreateItem 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItem
api_type:
- schema
ms.assetid: 78a52120-f1d0-4ed7-8748-436e554f75b6
description: CreateItem 操作は、Exchange ストア内のアイテムを作成します。
ms.openlocfilehash: 7e1808c685cdbaa1e8867aa7425b2cc52218d001
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759839"
---
# <a name="createitem-operation"></a>CreateItem 操作

CreateItem 操作は、Exchange ストア内のアイテムを作成します。
  
## <a name="using-the-createitem-operation"></a>CreateItem 操作を使用します。

CreateItem 操作を使用して、次を作成できます。
  
- 予定表アイテム
    
- 電子メール メッセージ
    
- 会議出席依頼
    
- タスク
    
- 連絡先
    
詳細については、 [CreateItem 操作 (予定表アイテム)](createitem-operation-calendar-item.md)、 [CreateItem 操作 (電子メール メッセージ)](createitem-operation-email-message.md)、 [CreateItem 操作 (会議出席依頼)](createitem-operation-meeting-request.md)、 [CreateItem 操作 (タスク)](createitem-operation-task.md)、および[CreateItem 操作 (連絡先) を参照してください。](createitem-operation-contact.md).
  
CreateItem 操作には、応答オブジェクトの使用がサポートされています。 応答オブジェクトは、承認と却下の会議と、標準の電子メール メッセージに含まれる返信ボタンの処理をサポートします。 次の表に、CreateItem 操作で処理される応答オブジェクトを示します。
  
|**応答オブジェクト**|**アクション**|
|:-----|:-----|
|AcceptItem  <br/> |会議出席依頼を承諾します。  <br/> |
|CancelCalendarItem  <br/> |会議をキャンセルします。 これも、開催者の会議が削除されるので、すべての出席者を削除すると異なります。  <br/> |
|DeclineItem  <br/> |会議出席依頼を辞退します。  <br/> |
|ForwardItem  <br/> |他のユーザーに会議出席依頼と会議出席依頼を送信します。  <br/> |
|RemoveItem  <br/> |キャンセルされた会議を予定表から削除します。  <br/> |
|ReplyAllToItem  <br/> |会議のすべての出席者に、元の会議出席依頼の本文を含むメッセージを送信します。  <br/> |
|ReplyToItem  <br/> |会議出席依頼の送信者に、元の会議出席依頼の本文を含むメッセージを送信します。  <br/> |
|SendReadReceipt  <br/> |会議出席依頼の送信者に開封確認メッセージを送信します。  <br/> |
|TentativelyAcceptItem  <br/> |会議出席依頼を仮承諾します。  <br/> |
   
CreateItem 操作には、会議の他のオブジェクトもサポートしています。 CreateItem 操作をサポートする追加のオブジェクトを次の表に一覧します。
  
|**会議オブジェクト**|**説明**|
|:-----|:-----|
|会議出席依頼  <br/> |Exchange ストア内の会議のメッセージを表します。 これは、他の会議オブジェクトの基本オブジェクトです。  <br/> |
|会議出席依頼  <br/> |Exchange ストア内の会議出席依頼を表します。  <br/> |
|会議の返信  <br/> |Exchange ストア内の会議の返信を表します。  <br/> |
|会議の取り消し  <br/> |Exchange ストア内の会議の取り消し通知を表します。  <br/> |
   
## <a name="see-also"></a>関連項目



[CreateItem 操作 (予定表アイテム)](createitem-operation-calendar-item.md)
  
[CreateItem 操作 (連絡先)](createitem-operation-contact.md)
  
[CreateItem 操作 (電子メール)](createitem-operation-email-message.md)
  
[CreateItem 操作 (会議出席依頼)](createitem-operation-meeting-request.md)
  
[CreateItem 操作 (タスク)](createitem-operation-task.md)
  
 **CreateItemType**

