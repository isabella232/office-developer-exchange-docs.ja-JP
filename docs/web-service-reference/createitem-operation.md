---
title: CreateItem 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CreateItem
api_type:
- schema
ms.assetid: 78a52120-f1d0-4ed7-8748-436e554f75b6
description: CreateItem 操作は、アイテム ストアにアイテムをExchangeします。
ms.openlocfilehash: 2aee80d883aa623b8074ecc523d1a45fa71962da
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538402"
---
# <a name="createitem-operation"></a>CreateItem 操作

CreateItem 操作は、アイテム ストアにアイテムをExchangeします。
  
## <a name="using-the-createitem-operation"></a>CreateItem 操作の使用

CreateItem 操作を使用して、次の操作を作成できます。
  
- 予定表アイテム
    
- 電子メール メッセージ
    
- 会議出席依頼
    
- タスク
    
- 連絡先
    
詳細については[、「CreateItem 操作 (予定表アイテム)、CreateItem](createitem-operation-calendar-item.md)操作 (電子メール メッセージ)、CreateItem 操作 (会議出席依頼[](createitem-operation-email-message.md)[)、CreateItem 操作 (タスク)、](createitem-operation-task.md)[および CreateItem](createitem-operation-contact.md)操作 (連絡先) を参照してください。 [](createitem-operation-meeting-request.md)
  
CreateItem 操作は、応答オブジェクトの使用をサポートします。 応答オブジェクトは、会議の受け入れと拒否、および標準の電子メール メッセージに含まれる投票ボタンの処理をサポートします。 次の表に、CreateItem 操作で処理される応答オブジェクトの一覧を示します。
  
|**Response オブジェクト**|**操作**|
|:-----|:-----|
|AcceptItem  <br/> |会議出席依頼を受け入れる。  <br/> |
|CancelCalendarItem  <br/> |会議をキャンセルします。 これは、開催者の会議も削除しますので、すべての出席者を削除するのとは異なります。  <br/> |
|DeclineItem  <br/> |会議出席依頼を拒否します。  <br/> |
|ForwardItem  <br/> |会議出席依頼として他のユーザーに会議出席依頼を送信します。  <br/> |
|RemoveItem  <br/> |予定表からキャンセルされた会議を削除します。  <br/> |
|ReplyAllToItem  <br/> |元の会議出席依頼の本文を含むメッセージを会議のすべての出席者に送信します。  <br/> |
|ReplyToItem  <br/> |元の会議出席依頼の本文を含むメッセージを会議出席依頼の送信者に送信します。  <br/> |
|SendReadReceipt  <br/> |会議出席依頼の送信者に読み取り確認メッセージを送信します。  <br/> |
|TentativelyAcceptItem  <br/> |会議出席依頼を暫定的に受け入れる。  <br/> |
   
CreateItem 操作は、追加の会議オブジェクトもサポートします。 次の表に、CreateItem 操作でサポートされるその他のオブジェクトの一覧を示します。
  
|**Meeting オブジェクト**|**説明**|
|:-----|:-----|
|会議メッセージ  <br/> |会議ストア内の会議メッセージExchangeします。 これは、他の会議オブジェクトの基本オブジェクトです。  <br/> |
|会議出席依頼  <br/> |ユーザー ストア内の会議出席依頼Exchangeします。  <br/> |
|会議の応答  <br/> |会議ストアの会議の応答Exchangeします。  <br/> |
|会議のキャンセル  <br/> |会議ストアでの会議の取り消しExchangeします。  <br/> |
   
## <a name="see-also"></a>関連項目



[CreateItem 操作 (予定表アイテム)](createitem-operation-calendar-item.md)
  
[CreateItem 操作 (連絡先)](createitem-operation-contact.md)
  
[CreateItem 操作 (メール メッセージ)](createitem-operation-email-message.md)
  
[CreateItem 操作 (会議出席依頼)](createitem-operation-meeting-request.md)
  
[CreateItem 操作 (タスク)](createitem-operation-task.md)
  
 **CreateItemType**

