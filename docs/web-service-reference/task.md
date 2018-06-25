---
title: タスク
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Task
api_type:
- schema
ms.assetid: 7c84927e-db28-4c5d-b0b5-cbcc2b88d869
description: Task 要素は、Exchange ストア内のタスクを表します。
ms.openlocfilehash: 2c61fca6ac85290e34f1365b0cb9e841e1fe279f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839655"
---
# <a name="task"></a><span data-ttu-id="3c198-103">タスク</span><span class="sxs-lookup"><span data-stu-id="3c198-103">Task</span></span>

<span data-ttu-id="3c198-104">**Task**要素は、Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="3c198-104">The **Task** element represents a task in the Exchange store.</span></span> 
  
```xml
<Task>
   <MimeContent/>
   <ItemId/>
   <ParentFolderId/>
   <ItemClass/>
   <Subject/>
   <Sensitivity/>
   <Body/>
   <Attachments/>
   <DateTimeReceived/>
   <Size/>
   <Categories/>
   <InReplyTo/>
   <IsSubmitted/>
   <IsDraft/>
   <IsFromMe/>
   <IsResend/>
   <IsUnmodified/>
   <InternetMessageHeaders/>
   <DateTimeSent/>
   <DateTimeCreated/>
   <ResponseObjects/>
   <ReminderDueBy/>
   <ReminderIsSet/>
   <ReminderMinutesBeforeStart/>
   <DisplayCc/>
   <DisplayTo/>
   <HasAttachments/>
   <ExtendedProperty/>
   <Culture/>
   <ActualWork/>
   <AssignedTime/>
   <BillingInformation/>
   <ChangeCount/>
   <Companies/>
   <CompleteDate/>
   <Contacts/>
   <DelegationState/>
   <Delegator/>
   <DueDate/>
   <IsAssignmentEditable/>
   <IsComplete/>
   <IsRecurring/>
   <IsTeamTask/>
   <Mileage/>
   <Owner/>
   <PercentComplete/>
   <Recurrence/>
   <StartDate/>
   <Status/>
   <StatusDescription/>
   <TotalWork/>
   <EffectiveRights/>
   <LastModifiedName/>
   <LastModifiedTime/>
   <IsAssociated/>
   <WebClientReadFormQueryString/>
   <WebClientEditFormQueryString/>
   <ConversationId/>
   <UniqueBody/>
</Task>
```

<span data-ttu-id="3c198-105">**TaskType**</span><span class="sxs-lookup"><span data-stu-id="3c198-105">**TaskType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="3c198-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="3c198-106">Attributes and elements</span></span>

<span data-ttu-id="3c198-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3c198-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3c198-108">属性</span><span class="sxs-lookup"><span data-stu-id="3c198-108">Attributes</span></span>

<span data-ttu-id="3c198-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3c198-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3c198-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3c198-110">Child elements</span></span>

|<span data-ttu-id="3c198-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="3c198-111">**Element**</span></span>|<span data-ttu-id="3c198-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="3c198-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3c198-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="3c198-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="3c198-114">Base64Binary の形式で表されるオブジェクトのネイティブの多目的インターネット メール拡張 (MIME) ストリームが含まれています。</span><span class="sxs-lookup"><span data-stu-id="3c198-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="3c198-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="3c198-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="3c198-116">Exchange ストア内のアイテムの一意の識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="3c198-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3c198-117">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="3c198-117">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="3c198-118">アイテムまたはフォルダーを含む親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="3c198-118">Represents the identifier of the parent folder that contains the item or folder.</span></span>  <br/> |
|[<span data-ttu-id="3c198-119">ItemClass</span><span class="sxs-lookup"><span data-stu-id="3c198-119">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="3c198-120">アイテムのメッセージ クラスを表します。</span><span class="sxs-lookup"><span data-stu-id="3c198-120">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="3c198-121">Subject</span><span class="sxs-lookup"><span data-stu-id="3c198-121">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="3c198-122">Exchange ストアのアイテムおよび応答オブジェクトのサブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="3c198-122">Represents the subject for Exchange store items and response objects.</span></span>  <br/> |
|[<span data-ttu-id="3c198-123">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="3c198-123">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="3c198-124">アイテムの秘密度の状態が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3c198-124">Contains the status for an item's sensitivity.</span></span>  <br/> |
|[<span data-ttu-id="3c198-125">Body/本文</span><span class="sxs-lookup"><span data-stu-id="3c198-125">Body</span></span>](body.md) <br/> |<span data-ttu-id="3c198-126">メッセージの実際の本文の内容を表します。</span><span class="sxs-lookup"><span data-stu-id="3c198-126">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="3c198-127">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="3c198-127">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="3c198-128">アイテムや、Exchange ストア内のアイテムに関連付けられているファイルが含まれています。</span><span class="sxs-lookup"><span data-stu-id="3c198-128">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3c198-129">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="3c198-129">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="3c198-130">メールボックス内のアイテムを受信したときの日時を表します。</span><span class="sxs-lookup"><span data-stu-id="3c198-130">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="3c198-131">Size</span><span class="sxs-lookup"><span data-stu-id="3c198-131">Size</span></span>](size.md) <br/> |<span data-ttu-id="3c198-132">アイテムのバイト単位でサイズを表します。</span><span class="sxs-lookup"><span data-stu-id="3c198-132">Represents the size, in bytes, of an item.</span></span> <span data-ttu-id="3c198-133">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="3c198-133">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="3c198-134">Categories</span><span class="sxs-lookup"><span data-stu-id="3c198-134">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="3c198-135">メールボックス内のアイテムが属するカテゴリを識別する文字列のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="3c198-135">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="3c198-136">Importance</span><span class="sxs-lookup"><span data-stu-id="3c198-136">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="3c198-137">アイテムの重要性をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="3c198-137">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="3c198-138">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="3c198-138">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="3c198-139">このアイテムの返信するアイテムの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="3c198-139">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="3c198-140">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="3c198-140">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="3c198-141">アイテムが [送信トレイ] 既定フォルダーに送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3c198-141">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="3c198-142">IsDraft</span><span class="sxs-lookup"><span data-stu-id="3c198-142">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="3c198-143">アイテムはまだ送信されていないかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="3c198-143">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="3c198-144">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="3c198-144">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="3c198-145">ユーザーが彼または彼女自身にアイテムを送信するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3c198-145">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="3c198-146">IsResend</span><span class="sxs-lookup"><span data-stu-id="3c198-146">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="3c198-147">アイテムが以前送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3c198-147">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="3c198-148">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="3c198-148">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="3c198-149">アイテムが変更されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3c198-149">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="3c198-150">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="3c198-150">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="3c198-151">メールボックス内のアイテムに含まれるすべてのインターネット メッセージ ヘッダーのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="3c198-151">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="3c198-152">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="3c198-152">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="3c198-153">メールボックス内のアイテムが送信された日時を表します。</span><span class="sxs-lookup"><span data-stu-id="3c198-153">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="3c198-154">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="3c198-154">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="3c198-155">メールボックス内の特定のアイテムが作成された日時を表します。</span><span class="sxs-lookup"><span data-stu-id="3c198-155">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="3c198-156">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="3c198-156">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="3c198-157">Exchange ストア内のアイテムに関連付けられているすべての応答オブジェクトのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="3c198-157">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3c198-158">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="3c198-158">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="3c198-159">イベントが発生したときの日時を表します。</span><span class="sxs-lookup"><span data-stu-id="3c198-159">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="3c198-160">[ReminderMinutesBeforeStart](reminderminutesbeforestart.md)要素によってアラームが表示されたときを決定する使用されます。</span><span class="sxs-lookup"><span data-stu-id="3c198-160">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="3c198-161">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="3c198-161">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="3c198-162">Exchange ストアのアイテムのアラームが設定されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3c198-162">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3c198-163">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="3c198-163">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="3c198-164">分前にアラームが表示されるときに、イベントの数を表します。</span><span class="sxs-lookup"><span data-stu-id="3c198-164">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="3c198-165">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="3c198-165">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="3c198-166">[Cc] ボックスの内容のために使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="3c198-166">Represents the display string that is used for the contents of the Cc box.</span></span> <span data-ttu-id="3c198-167">これは、すべての Cc 受信者の表示名の連結された文字列です。</span><span class="sxs-lookup"><span data-stu-id="3c198-167">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="3c198-168">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="3c198-168">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="3c198-169">ボックスの内容のために使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="3c198-169">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="3c198-170">これは、すべての受信者の表示名の連結された文字列です。</span><span class="sxs-lookup"><span data-stu-id="3c198-170">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="3c198-171">添付ファイル付き</span><span class="sxs-lookup"><span data-stu-id="3c198-171">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="3c198-172">アイテムに表示されている 1 つ以上の添付ファイルがある場合に**true**に設定されているプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="3c198-172">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="3c198-173">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="3c198-173">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="3c198-174">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="3c198-174">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="3c198-175">フォルダーおよびアイテムの拡張プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="3c198-175">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="3c198-176">カルチャ</span><span class="sxs-lookup"><span data-stu-id="3c198-176">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="3c198-177">メールボックス内の指定したアイテムのカルチャを表します。</span><span class="sxs-lookup"><span data-stu-id="3c198-177">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="3c198-178">ActualWork</span><span class="sxs-lookup"><span data-stu-id="3c198-178">ActualWork</span></span>](actualwork.md) <br/> |<span data-ttu-id="3c198-179">タスクに費やされた時間の実際の量を表します。</span><span class="sxs-lookup"><span data-stu-id="3c198-179">Represents the actual amount of time that is spent on a task.</span></span>  <br/> |
|[<span data-ttu-id="3c198-180">AssignedTime</span><span class="sxs-lookup"><span data-stu-id="3c198-180">AssignedTime</span></span>](assignedtime.md) <br/> |<span data-ttu-id="3c198-181">連絡先にタスクを割り当てると時間を表します。</span><span class="sxs-lookup"><span data-stu-id="3c198-181">Represents the time when a task is assigned to a contact.</span></span>  <br/> |
|[<span data-ttu-id="3c198-182">BillingInformation</span><span class="sxs-lookup"><span data-stu-id="3c198-182">BillingInformation</span></span>](billinginformation.md) <br/> |<span data-ttu-id="3c198-183">課金タスクの情報を保持します。</span><span class="sxs-lookup"><span data-stu-id="3c198-183">Holds billing information for a task.</span></span>  <br/> |
|[<span data-ttu-id="3c198-184">ChangeCount</span><span class="sxs-lookup"><span data-stu-id="3c198-184">ChangeCount</span></span>](changecount.md) <br/> |<span data-ttu-id="3c198-185">タスクのバージョンを指定します。</span><span class="sxs-lookup"><span data-stu-id="3c198-185">Specifies the version of the task.</span></span>  <br/> |
|[<span data-ttu-id="3c198-186">Companies</span><span class="sxs-lookup"><span data-stu-id="3c198-186">Companies</span></span>](companies.md) <br/> |<span data-ttu-id="3c198-187">連絡先またはタスクに関連付けられている企業のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="3c198-187">Represents the collection of companies that are associated with a contact or task.</span></span>  <br/> |
|[<span data-ttu-id="3c198-188">CompleteDate</span><span class="sxs-lookup"><span data-stu-id="3c198-188">CompleteDate</span></span>](completedate.md) <br/> |<span data-ttu-id="3c198-189">タスクが完了する日付を表します。</span><span class="sxs-lookup"><span data-stu-id="3c198-189">Represents the date on which a task is completed.</span></span>  <br/> |
|[<span data-ttu-id="3c198-190">連絡先</span><span class="sxs-lookup"><span data-stu-id="3c198-190">Contacts</span></span>](contacts-ex15websvcsotherref.md) <br/> |<span data-ttu-id="3c198-191">タスクに関連付けられている連絡先の一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3c198-191">Contains a list of contacts that are associated with a task.</span></span>  <br/> |
|[<span data-ttu-id="3c198-192">DelegationState</span><span class="sxs-lookup"><span data-stu-id="3c198-192">DelegationState</span></span>](delegationstate.md) <br/> |<span data-ttu-id="3c198-193">委任されたタスクの状態を表します。</span><span class="sxs-lookup"><span data-stu-id="3c198-193">Represents the status of a delegated task.</span></span>  <br/> |
|[<span data-ttu-id="3c198-194">Delegator</span><span class="sxs-lookup"><span data-stu-id="3c198-194">Delegator</span></span>](delegator.md) <br/> |<span data-ttu-id="3c198-195">タスクを割り当てられている代理人の名前が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3c198-195">Contains the name of the delegator who assigned the task.</span></span>  <br/> |
|[<span data-ttu-id="3c198-196">DueDate</span><span class="sxs-lookup"><span data-stu-id="3c198-196">DueDate</span></span>](duedate.md) <br/> |<span data-ttu-id="3c198-197">タスク アイテムの期限の日付を表します。</span><span class="sxs-lookup"><span data-stu-id="3c198-197">Represents the date when a task item is due.</span></span>  <br/> |
|[<span data-ttu-id="3c198-198">IsAssignmentEditable</span><span class="sxs-lookup"><span data-stu-id="3c198-198">IsAssignmentEditable</span></span>](isassignmenteditable.md) <br/> |<span data-ttu-id="3c198-199">タスクが編集可能かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3c198-199">Indicates whether the task is editable or not.</span></span>  <br/> |
|[<span data-ttu-id="3c198-200">完了</span><span class="sxs-lookup"><span data-stu-id="3c198-200">IsComplete</span></span>](iscomplete.md) <br/> |<span data-ttu-id="3c198-201">タスクが完了したかどうかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3c198-201">Indicates whether the task has been completed or not.</span></span>  <br/> |
|[<span data-ttu-id="3c198-202">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="3c198-202">IsRecurring</span></span>](isrecurring.md) <br/> |<span data-ttu-id="3c198-203">タスクが定期的なアイテムの一部であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3c198-203">Indicates whether a task is part of a recurring item.</span></span> <span data-ttu-id="3c198-204">この要素は、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="3c198-204">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="3c198-205">IsTeamTask</span><span class="sxs-lookup"><span data-stu-id="3c198-205">IsTeamTask</span></span>](isteamtask.md) <br/> |<span data-ttu-id="3c198-206">か、タスクが、チームが所有するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3c198-206">Indicates whether the task is owned by a team or not.</span></span>  <br/> |
|[<span data-ttu-id="3c198-207">マイレージ</span><span class="sxs-lookup"><span data-stu-id="3c198-207">Mileage</span></span>](mileage.md) <br/> |<span data-ttu-id="3c198-208">タスク アイテムの経費情報を表します。</span><span class="sxs-lookup"><span data-stu-id="3c198-208">Represents mileage for a task item.</span></span>  <br/> |
|[<span data-ttu-id="3c198-209">所有者</span><span class="sxs-lookup"><span data-stu-id="3c198-209">Owner</span></span>](owner.md) <br/> |<span data-ttu-id="3c198-210">タスクの所有者を表します。</span><span class="sxs-lookup"><span data-stu-id="3c198-210">Represents the owner of a task.</span></span>  <br/> |
|[<span data-ttu-id="3c198-211">達成率</span><span class="sxs-lookup"><span data-stu-id="3c198-211">PercentComplete</span></span>](percentcomplete.md) <br/> |<span data-ttu-id="3c198-212">タスクの完了状態を説明します。</span><span class="sxs-lookup"><span data-stu-id="3c198-212">Describes the completion status of a task.</span></span>  <br/> |
|[<span data-ttu-id="3c198-213">定期的な予定 (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="3c198-213">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="3c198-214">定期タスクの頻度に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3c198-214">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="3c198-215">開始日</span><span class="sxs-lookup"><span data-stu-id="3c198-215">StartDate</span></span>](startdate.md) <br/> |<span data-ttu-id="3c198-216">作業項目の開始日を表します。</span><span class="sxs-lookup"><span data-stu-id="3c198-216">Represents the start date of a task item.</span></span>  <br/> |
|[<span data-ttu-id="3c198-217">Status</span><span class="sxs-lookup"><span data-stu-id="3c198-217">Status</span></span>](status.md) <br/> |<span data-ttu-id="3c198-218">作業項目の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="3c198-218">Represents the status of a task item.</span></span>  <br/> |
|[<span data-ttu-id="3c198-219">StatusDescription</span><span class="sxs-lookup"><span data-stu-id="3c198-219">StatusDescription</span></span>](statusdescription.md) <br/> |<span data-ttu-id="3c198-220">タスクの進捗状況の説明が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3c198-220">Contains an explanation of the task status.</span></span>  <br/> |
|[<span data-ttu-id="3c198-221">TotalWork</span><span class="sxs-lookup"><span data-stu-id="3c198-221">TotalWork</span></span>](totalwork.md) <br/> |<span data-ttu-id="3c198-222">アイテムに関連付けられている作業量の説明が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3c198-222">Contains a description of how much work is associated with an item.</span></span>  <br/> |
|[<span data-ttu-id="3c198-223">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="3c198-223">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="3c198-224">アイテムまたはフォルダーのアクセス許可の設定に基づいてクライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3c198-224">Contains the rights of the client based on the permission settings for the item or folder.</span></span> <span data-ttu-id="3c198-225">この要素は、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="3c198-225">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="3c198-226">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="3c198-226">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="3c198-227">最後の項目を変更するのにはユーザーの表示名が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3c198-227">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="3c198-228">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="3c198-228">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="3c198-229">アイテムが最後に修正された日時を示します。</span><span class="sxs-lookup"><span data-stu-id="3c198-229">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="3c198-230">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="3c198-230">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="3c198-231">アイテムがフォルダーに関連付けられているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3c198-231">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="3c198-232">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="3c198-232">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="3c198-233">Outlook Web App 内の項目を参照するのには Microsoft Office Outlook の Web アプリケーションのエンドポイントを結合するための URL を表します。</span><span class="sxs-lookup"><span data-stu-id="3c198-233">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="3c198-234">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="3c198-234">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="3c198-235">Outlook Web App 内の項目を編集するのには Outlook Web App エンドポイントへの連結に URL を表します。</span><span class="sxs-lookup"><span data-stu-id="3c198-235">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="3c198-236">ConversationId</span><span class="sxs-lookup"><span data-stu-id="3c198-236">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="3c198-237">アイテムや会話の識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3c198-237">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="3c198-238">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="3c198-238">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="3c198-239">このスレッドの一意の本文を表すテキストまたは HTML フラグメントを表します。</span><span class="sxs-lookup"><span data-stu-id="3c198-239">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3c198-240">親要素</span><span class="sxs-lookup"><span data-stu-id="3c198-240">Parent elements</span></span>

|<span data-ttu-id="3c198-241">**要素**</span><span class="sxs-lookup"><span data-stu-id="3c198-241">**Element**</span></span>|<span data-ttu-id="3c198-242">**説明**</span><span class="sxs-lookup"><span data-stu-id="3c198-242">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3c198-243">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="3c198-243">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="3c198-244">会議の時刻に隣接しているすべての予定表のアイテムについて説明します。</span><span class="sxs-lookup"><span data-stu-id="3c198-244">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="3c198-245">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="3c198-245">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="3c198-246">[UpdateItem 操作](updateitem-operation.md)中に、アイテムやフォルダーの 1 つのプロパティを追加するデータを識別します。</span><span class="sxs-lookup"><span data-stu-id="3c198-246">Identifies data to append to a single property of an item/folder during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="3c198-247">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="3c198-247">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="3c198-248">会議の時間と競合するすべての項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="3c198-248">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="3c198-249">(ItemSync) を作成します。</span><span class="sxs-lookup"><span data-stu-id="3c198-249">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="3c198-250">ローカル クライアント ストアに作成する 1 つの項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="3c198-250">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="3c198-251">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="3c198-251">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="3c198-252">Exchange の他のアイテムに関連付けられている Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="3c198-252">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="3c198-253">Items</span><span class="sxs-lookup"><span data-stu-id="3c198-253">Items</span></span>](items.md) <br/> |<span data-ttu-id="3c198-254">項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3c198-254">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="3c198-255">SetItemField</span><span class="sxs-lookup"><span data-stu-id="3c198-255">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="3c198-256">[UpdateItem 操作](updateitem-operation.md)内の項目の 1 つのプロパティには、更新プログラムを表します。</span><span class="sxs-lookup"><span data-stu-id="3c198-256">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="3c198-257">更新プログラム (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="3c198-257">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="3c198-258">ローカル クライアント ストアで更新する 1 つの項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="3c198-258">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3c198-259">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3c198-259">Text value</span></span>

<span data-ttu-id="3c198-260">なし。</span><span class="sxs-lookup"><span data-stu-id="3c198-260">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3c198-261">備考</span><span class="sxs-lookup"><span data-stu-id="3c198-261">Remarks</span></span>

<span data-ttu-id="3c198-262">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="3c198-262">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3c198-263">要素情報</span><span class="sxs-lookup"><span data-stu-id="3c198-263">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3c198-264">名前空間</span><span class="sxs-lookup"><span data-stu-id="3c198-264">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3c198-265">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3c198-265">Schema name</span></span>  <br/> |<span data-ttu-id="3c198-266">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="3c198-266">Types schema</span></span>  <br/> |
|<span data-ttu-id="3c198-267">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3c198-267">Validation file</span></span>  <br/> |<span data-ttu-id="3c198-268">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3c198-268">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3c198-269">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="3c198-269">Can be empty</span></span>  <br/> |<span data-ttu-id="3c198-270">False</span><span class="sxs-lookup"><span data-stu-id="3c198-270">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3c198-271">関連項目</span><span class="sxs-lookup"><span data-stu-id="3c198-271">See also</span></span>

- [<span data-ttu-id="3c198-272">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="3c198-272">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="3c198-273">タスクを作成します。</span><span class="sxs-lookup"><span data-stu-id="3c198-273">Creating Tasks</span></span>](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
- [<span data-ttu-id="3c198-274">タスクを削除します。</span><span class="sxs-lookup"><span data-stu-id="3c198-274">Deleting Tasks</span></span>](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

