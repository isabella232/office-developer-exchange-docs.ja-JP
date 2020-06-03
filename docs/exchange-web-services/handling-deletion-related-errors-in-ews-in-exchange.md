---
title: Exchange の EWS での削除に関連するエラーの処理
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1bbe8507-7730-45e5-9232-c4f6fc39c2d9
description: Exchange の EWS マネージ API または EWS を使用して、開発したアプリケーションの削除に関連するエラーを処理する方法を確認します。
ms.openlocfilehash: 41c217c1c3815606d898b8237ea327f34869174b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455948"
---
# <a name="handling-deletion-related-errors-in-ews-in-exchange"></a>Exchange の EWS での削除に関連するエラーの処理

Exchange の EWS マネージ API または EWS を使用して、開発したアプリケーションの削除に関連するエラーを処理する方法を確認します。
  
アプリケーションが[アイテムとフォルダーを削除する](deleting-items-by-using-ews-in-exchange.md)場合は、削除に関連するエラーを処理する必要があります。これらのエラーは実行時に、または EWS アプリケーションを開発するときに処理することができます。
  
**表 1: 削除に関連するエラーとその処理方法**

|**エラー**|**発生するタイミング**|**処理方法**|
|:-----|:-----|:-----|
|ErrorAffectedTaskOccurrencesRequired  <br/> |定期的なタスクのインスタンスを削除するときに、**AffectedTaskOccurrence** プロパティが設定されていない場合。  <br/> |**AffectedTaskOccurrence** プロパティを設定し、削除を再試行します。  <br/> |
|ErrorCalendarCannotUpdateDeletedItem  <br/> |削除済みアイテム フォルダーにある予定表アイテムを更新すると、その更新によって出席者に会議出席依頼が送信されることになります。  <br/> |更新をキャンセルするか、予定表アイテムを既定の予定表フォルダーに移動して、予定表アイテムを更新します。  <br/> |
|ErrorCalendarOccurrenceIsDeletedFromRecurrence  <br/> |定期的な予定の、削除された発生アイテムを参照しています。  <br/> |削除された発生アイテムへの参照を削除します。  <br/> |
|ErrorCannotDeleteObject  <br/> |削除できないアイテムを削除しています。  <br/> |アイテムの削除の試行をやめます。  <br/> |
|ErrorCannotDeleteTaskOccurrence  <br/> |非定期的なタスクの発生アイテムを削除しているか、定期的なタスクの最後の発生アイテムを削除しています。  <br/> |非定期的なタスクを削除するか、定期的なタスクの最後の発生アイテムの削除の試みをやめます。  <br/> |
|ErrorDeleteDistinguishedFolder  <br/> |識別されたフォルダーを削除しています。  <br/> |既定のフォルダーは削除できないことを示します。  <br/> |
|ErrorItemNotFound  <br/> |完全に削除されたアイテムにアクセスしています。  <br/> |ストアから削除されるときに、アイテムへの参照を削除します。アイテムを復元する場合は、クライアントに必要な参照を戻してください。  <br/> |
|ErrorSendMeetingCancellationsRequired  <br/> |会議のキャンセルを送信するかどうかを指定せずに予定表アイテムを削除しています。  <br/> |会議のキャンセルを送信する必要があるかどうかを指定します。  <br/> |
   
## <a name="see-also"></a>関連項目


- [Exchange で EWS を使用してアイテムを削除する](deleting-items-by-using-ews-in-exchange.md)
    
- [Exchange での EWS の削除に関連するメールボックス イベントのプル通知](pull-notifications-for-ews-deletion-related-mailbox-events-in-exchange.md)
    
- [Exchange の EWS を使用して、予定を削除し、会議をキャンセルする](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    

