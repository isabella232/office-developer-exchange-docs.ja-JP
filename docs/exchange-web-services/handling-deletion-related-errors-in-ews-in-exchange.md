---
title: Exchange の EWS での削除に関連するエラーの処理
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1bbe8507-7730-45e5-9232-c4f6fc39c2d9
description: EWS マネージ API または Exchange の EWS を使用して、開発したアプリケーションの削除に関連するエラーを処理する方法を確認します。
ms.openlocfilehash: 0dc16c3350bb75fb1e91650f0a0f0b7423727eeb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758887"
---
# <a name="handling-deletion-related-errors-in-ews-in-exchange"></a><span data-ttu-id="7b367-103">Exchange の EWS での削除に関連するエラーの処理</span><span class="sxs-lookup"><span data-stu-id="7b367-103">Handling deletion-related errors in EWS in Exchange</span></span>

<span data-ttu-id="7b367-104">EWS マネージ API または Exchange の EWS を使用して、開発したアプリケーションの削除に関連するエラーを処理する方法を確認します。</span><span class="sxs-lookup"><span data-stu-id="7b367-104">Find out how to handle deletion-related errors in applications that you develop by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="7b367-105">かどうか、アプリケーションが[アイテムとフォルダーの削除](deleting-items-by-using-ews-in-exchange.md)をする必要があります削除に関連するエラーを処理します。</span><span class="sxs-lookup"><span data-stu-id="7b367-105">If your application [deletes items and folders](deleting-items-by-using-ews-in-exchange.md), you might have to handle deletion-related errors.</span></span> <span data-ttu-id="7b367-106">または、EWS アプリケーションを開発するとき、実行時にこれらのエラーを処理することができます。</span><span class="sxs-lookup"><span data-stu-id="7b367-106">You can handle these errors at runtime, or while you are developing your EWS application.</span></span>
  
<span data-ttu-id="7b367-107">**表 1: 削除に関連するエラーと、それらを処理する方法**</span><span class="sxs-lookup"><span data-stu-id="7b367-107">**Table 1: Deletion-related errors and how to handle them**</span></span>

|<span data-ttu-id="7b367-108">**Error**</span><span class="sxs-lookup"><span data-stu-id="7b367-108">**Error**</span></span>|<span data-ttu-id="7b367-109">**しようとするときに発生しています.**</span><span class="sxs-lookup"><span data-stu-id="7b367-109">**Occurs when you try to…**</span></span>|<span data-ttu-id="7b367-110">**処理方法**</span><span class="sxs-lookup"><span data-stu-id="7b367-110">**Handle it by…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="7b367-111">ErrorAffectedTaskOccurrencesRequired</span><span class="sxs-lookup"><span data-stu-id="7b367-111">ErrorAffectedTaskOccurrencesRequired</span></span>  <br/> |<span data-ttu-id="7b367-112">定期的なタスクのインスタンスを削除し、 **AffectedTaskOccurrence**プロパティが設定されていません。</span><span class="sxs-lookup"><span data-stu-id="7b367-112">Delete an instance of a recurring task, and the **AffectedTaskOccurrence** property is not set.</span></span>  <br/> |<span data-ttu-id="7b367-113">**AffectedTaskOccurrence**プロパティを設定し、削除を再試行します。</span><span class="sxs-lookup"><span data-stu-id="7b367-113">Setting the **AffectedTaskOccurrence** property, and retrying the deletion.</span></span>  <br/> |
|<span data-ttu-id="7b367-114">ErrorCalendarCannotUpdateDeletedItem</span><span class="sxs-lookup"><span data-stu-id="7b367-114">ErrorCalendarCannotUpdateDeletedItem</span></span>  <br/> |<span data-ttu-id="7b367-115">削除済みアイテム フォルダーにある予定表アイテムを更新すると、その更新によって出席者に会議出席依頼が送信されることになります。</span><span class="sxs-lookup"><span data-stu-id="7b367-115">Update a calendar item located in the Deleted Items folder when the update would result in sending a meeting invite to attendees.</span></span>  <br/> |<span data-ttu-id="7b367-116">更新をキャンセルするか、予定表アイテムを既定の予定表フォルダーに移動して、予定表アイテムを更新します。</span><span class="sxs-lookup"><span data-stu-id="7b367-116">Canceling the update or moving the calendar item back to the default Calendar folder and updating the calendar item.</span></span>  <br/> |
|<span data-ttu-id="7b367-117">ErrorCalendarOccurrenceIsDeletedFromRecurrence</span><span class="sxs-lookup"><span data-stu-id="7b367-117">ErrorCalendarOccurrenceIsDeletedFromRecurrence</span></span>  <br/> |<span data-ttu-id="7b367-118">定期的な予定の、削除された発生アイテムを参照しています。</span><span class="sxs-lookup"><span data-stu-id="7b367-118">Reference a deleted occurrence of a recurring appointment.</span></span>  <br/> |<span data-ttu-id="7b367-119">削除された発生アイテムへの参照を削除します。</span><span class="sxs-lookup"><span data-stu-id="7b367-119">Removing a reference to a deleted occurrence.</span></span>  <br/> |
|<span data-ttu-id="7b367-120">ErrorCannotDeleteObject</span><span class="sxs-lookup"><span data-stu-id="7b367-120">ErrorCannotDeleteObject</span></span>  <br/> |<span data-ttu-id="7b367-121">削除できないアイテムを削除しています。</span><span class="sxs-lookup"><span data-stu-id="7b367-121">Delete an item that cannot be deleted.</span></span>  <br/> |<span data-ttu-id="7b367-122">アイテムの削除の試行をやめます。</span><span class="sxs-lookup"><span data-stu-id="7b367-122">Quitting attempts to delete the item.</span></span>  <br/> |
|<span data-ttu-id="7b367-123">ErrorCannotDeleteTaskOccurrence</span><span class="sxs-lookup"><span data-stu-id="7b367-123">ErrorCannotDeleteTaskOccurrence</span></span>  <br/> |<span data-ttu-id="7b367-124">非定期的なタスクの発生アイテムを削除しているか、定期的なタスクの最後の発生アイテムを削除しています。</span><span class="sxs-lookup"><span data-stu-id="7b367-124">Delete an occurrence of a nonrecurring task or delete the last occurrence of a recurring task.</span></span>  <br/> |<span data-ttu-id="7b367-125">非定期的なタスクを削除するか、定期的なタスクの最後の発生アイテムの削除の試みをやめます。 </span><span class="sxs-lookup"><span data-stu-id="7b367-125">Deleting a nonrecurring task or quitting attempts to delete the last occurrence of a recurring task.</span></span>  <br/> |
|<span data-ttu-id="7b367-126">ErrorDeleteDistinguishedFolder</span><span class="sxs-lookup"><span data-stu-id="7b367-126">ErrorDeleteDistinguishedFolder</span></span>  <br/> |<span data-ttu-id="7b367-127">識別されたフォルダーを削除しています。</span><span class="sxs-lookup"><span data-stu-id="7b367-127">Delete a distinguished folder.</span></span>  <br/> |<span data-ttu-id="7b367-128">既定のフォルダーは削除できないことを示します。</span><span class="sxs-lookup"><span data-stu-id="7b367-128">Indicating that default folders cannot be deleted.</span></span>  <br/> |
|<span data-ttu-id="7b367-129">ErrorItemNotFound</span><span class="sxs-lookup"><span data-stu-id="7b367-129">ErrorItemNotFound</span></span>  <br/> |<span data-ttu-id="7b367-130">完全に削除されたアイテムにアクセスしています。</span><span class="sxs-lookup"><span data-stu-id="7b367-130">Access a permanently deleted item.</span></span>  <br/> |<span data-ttu-id="7b367-p102">ストアから削除されるときに、アイテムへの参照を削除します。アイテムを復元する場合は、クライアントに必要な参照を戻してください。</span><span class="sxs-lookup"><span data-stu-id="7b367-p102">Removing references to an item when it is deleted from the store. If an item is recovered, make sure that you reinstate required references to the client.</span></span>  <br/> |
|<span data-ttu-id="7b367-133">ErrorSendMeetingCancellationsRequired</span><span class="sxs-lookup"><span data-stu-id="7b367-133">ErrorSendMeetingCancellationsRequired</span></span>  <br/> |<span data-ttu-id="7b367-134">会議のキャンセルを送信するかどうかを指定せずに予定表アイテムを削除しています。</span><span class="sxs-lookup"><span data-stu-id="7b367-134">Delete a calendar item without specifying whether meeting cancellations should be sent.</span></span>  <br/> |<span data-ttu-id="7b367-135">会議のキャンセルを送信する必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="7b367-135">Specifying that meeting cancellations should or should not be sent.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7b367-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="7b367-136">See also</span></span>


- [<span data-ttu-id="7b367-137">Exchange の EWS を使用するアイテムの削除</span><span class="sxs-lookup"><span data-stu-id="7b367-137">Deleting items by using EWS in Exchange</span></span>](deleting-items-by-using-ews-in-exchange.md)
    
- <span data-ttu-id="7b367-138">[EWS の [メールボックスの削除に関連するイベントの通知を Exchange でプルします。](pull-notifications-for-ews-deletion-related-mailbox-events-in-exchange.md)</span><span class="sxs-lookup"><span data-stu-id="7b367-138">[Pull notifications for EWS deletion-related mailbox events in Exchange](pull-notifications-for-ews-deletion-related-mailbox-events-in-exchange.md)</span></span>
    
- [<span data-ttu-id="7b367-139">予定を削除して、Exchange で EWS を使用して会議をキャンセル</span><span class="sxs-lookup"><span data-stu-id="7b367-139">Delete appointments and cancel meetings by using EWS in Exchange</span></span>](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    

