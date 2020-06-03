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
description: CreateItem 操作は、Exchange ストアにアイテムを作成します。
ms.openlocfilehash: f6aaa9ed8e8257f19780492d6137fb015c1b6136
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458867"
---
# <a name="createitem-operation"></a>CreateItem 操作

CreateItem 操作は、Exchange ストアにアイテムを作成します。
  
## <a name="using-the-createitem-operation"></a>CreateItem 操作の使用

CreateItem 操作を使用して、次のものを作成できます。
  
- 予定表アイテム
    
- 電子メール メッセージ
    
- 会議出席依頼
    
- タスク
    
- 連絡先
    
詳細については、「 [CreateItem 操作 (予定表アイテム)](createitem-operation-calendar-item.md)」、「 [CreateItem 操作 (電子メールメッセージ)](createitem-operation-email-message.md)」、「 [CreateItem operation (meeting request)](createitem-operation-meeting-request.md)、 [CreateItem operation (task)](createitem-operation-task.md)、 [CreateItem operation (contact)](createitem-operation-contact.md)」を参照してください。
  
CreateItem 操作では、response オブジェクトの使用がサポートされています。 応答オブジェクトは、会議の承諾と却下、および標準の電子メールメッセージに含まれる投票ボタンの処理をサポートします。 次の表に、CreateItem 操作で処理される応答オブジェクトを示します。
  
|**Response オブジェクト**|**Action**|
|:-----|:-----|
|AcceptItem  <br/> |会議出席依頼を承諾します。  <br/> |
|CancelCalendarItem  <br/> |会議をキャンセルします。 これは、開催者の会議も削除するため、すべての出席者を削除するのとは異なります。  <br/> |
|DeclineItem  <br/> |会議出席依頼を辞退します。  <br/> |
|Forwarditem と  <br/> |会議出席依頼として他のユーザーに会議出席依頼を送信します。  <br/> |
|RemoveItem  <br/> |予定表からキャンセルされた会議を削除します。  <br/> |
|Replyalltoitem と  <br/> |元の会議出席依頼の本文を含むメッセージを、会議のすべての出席者に送信します。  <br/> |
|ReplyToItem  <br/> |元の会議出席依頼の本文を含むメッセージを、会議出席依頼の送信者に送信します。  <br/> |
|SendReadReceipt  <br/> |会議出席依頼の送信者に開封確認メッセージを送信します。  <br/> |
|TentativelyAcceptItem  <br/> |会議出席依頼を仮承諾します。  <br/> |
   
CreateItem 操作では、追加の会議オブジェクトもサポートされます。 次の表に、CreateItem 操作がサポートする追加のオブジェクトを示します。
  
|**会議オブジェクト**|**説明**|
|:-----|:-----|
|会議メッセージ  <br/> |Exchange ストア内の会議メッセージを表します。 これは、その他の会議オブジェクトの基本オブジェクトです。  <br/> |
|会議出席依頼  <br/> |Exchange ストア内の会議出席依頼を表します。  <br/> |
|会議出席依頼の返信  <br/> |Exchange ストア内の会議の応答を表します。  <br/> |
|会議の取り消し  <br/> |Exchange ストア内の会議の取り消しを表します。  <br/> |
   
## <a name="see-also"></a>関連項目



[CreateItem 操作 (予定表アイテム)](createitem-operation-calendar-item.md)
  
[CreateItem 操作 (連絡先)](createitem-operation-contact.md)
  
[CreateItem 操作 (電子メールメッセージ)](createitem-operation-email-message.md)
  
[CreateItem 操作 (会議出席依頼)](createitem-operation-meeting-request.md)
  
[CreateItem 操作 (タスク)](createitem-operation-task.md)
  
 **CreateItemType**

