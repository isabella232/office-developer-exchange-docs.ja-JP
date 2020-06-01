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
ms.openlocfilehash: 669f90dfa74cd085091e9836a1d31ca53bbf165e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458944"
---
# <a name="task"></a><span data-ttu-id="997b4-103">タスク</span><span class="sxs-lookup"><span data-stu-id="997b4-103">Task</span></span>

<span data-ttu-id="997b4-104">**Task**要素は、Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="997b4-104">The **Task** element represents a task in the Exchange store.</span></span> 
  
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

<span data-ttu-id="997b4-105">**TaskType**</span><span class="sxs-lookup"><span data-stu-id="997b4-105">**TaskType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="997b4-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="997b4-106">Attributes and elements</span></span>

<span data-ttu-id="997b4-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="997b4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="997b4-108">属性</span><span class="sxs-lookup"><span data-stu-id="997b4-108">Attributes</span></span>

<span data-ttu-id="997b4-109">なし。</span><span class="sxs-lookup"><span data-stu-id="997b4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="997b4-110">子要素</span><span class="sxs-lookup"><span data-stu-id="997b4-110">Child elements</span></span>

|<span data-ttu-id="997b4-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="997b4-111">**Element**</span></span>|<span data-ttu-id="997b4-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="997b4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="997b4-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="997b4-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="997b4-114">Base64Binary 形式で表されるオブジェクトのネイティブな汎用インターネットメール内線 (MIME) ストリームが保存されています。</span><span class="sxs-lookup"><span data-stu-id="997b4-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="997b4-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="997b4-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="997b4-116">Exchange ストア内のアイテムの一意識別子および変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="997b4-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="997b4-117">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="997b4-117">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="997b4-118">アイテムまたはフォルダーを含む親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="997b4-118">Represents the identifier of the parent folder that contains the item or folder.</span></span>  <br/> |
|[<span data-ttu-id="997b4-119">ItemClass</span><span class="sxs-lookup"><span data-stu-id="997b4-119">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="997b4-120">アイテムのメッセージクラスを表します。</span><span class="sxs-lookup"><span data-stu-id="997b4-120">Represents the message class of an item.</span></span>  <br/> |
|<span data-ttu-id="997b4-121">[[件名]](subject.md)</span><span class="sxs-lookup"><span data-stu-id="997b4-121">[Subject](subject.md)</span></span> <br/> |<span data-ttu-id="997b4-122">Exchange ストアアイテムおよび応答オブジェクトの件名を表します。</span><span class="sxs-lookup"><span data-stu-id="997b4-122">Represents the subject for Exchange store items and response objects.</span></span>  <br/> |
|[<span data-ttu-id="997b4-123">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="997b4-123">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="997b4-124">アイテムの秘密度の状態を格納します。</span><span class="sxs-lookup"><span data-stu-id="997b4-124">Contains the status for an item's sensitivity.</span></span>  <br/> |
|[<span data-ttu-id="997b4-125">Body</span><span class="sxs-lookup"><span data-stu-id="997b4-125">Body</span></span>](body.md) <br/> |<span data-ttu-id="997b4-126">メッセージの実際の本文の内容を表します。</span><span class="sxs-lookup"><span data-stu-id="997b4-126">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="997b4-127">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="997b4-127">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="997b4-128">Exchange ストア内のアイテムに添付されているアイテムまたはファイルが保存されています。</span><span class="sxs-lookup"><span data-stu-id="997b4-128">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="997b4-129">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="997b4-129">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="997b4-130">メールボックス内のアイテムが受信された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="997b4-130">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|<span data-ttu-id="997b4-131">[[サイズ]](size.md)</span><span class="sxs-lookup"><span data-stu-id="997b4-131">[Size](size.md)</span></span> <br/> |<span data-ttu-id="997b4-132">アイテムのサイズ (バイト単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="997b4-132">Represents the size, in bytes, of an item.</span></span> <span data-ttu-id="997b4-133">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="997b4-133">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="997b4-134">カテゴリ</span><span class="sxs-lookup"><span data-stu-id="997b4-134">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="997b4-135">メールボックス内のアイテムが属するカテゴリを識別する文字列のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="997b4-135">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="997b4-136">Importance</span><span class="sxs-lookup"><span data-stu-id="997b4-136">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="997b4-137">アイテムの重要度について説明します。</span><span class="sxs-lookup"><span data-stu-id="997b4-137">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="997b4-138">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="997b4-138">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="997b4-139">このアイテムが返信であるアイテムの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="997b4-139">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="997b4-140">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="997b4-140">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="997b4-141">アイテムが送信トレイの既定フォルダーに送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="997b4-141">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="997b4-142">IsDraft</span><span class="sxs-lookup"><span data-stu-id="997b4-142">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="997b4-143">アイテムがまだ送信されていないかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="997b4-143">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="997b4-144">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="997b4-144">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="997b4-145">ユーザーが自分にアイテムを送信したかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="997b4-145">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="997b4-146">IsResend</span><span class="sxs-lookup"><span data-stu-id="997b4-146">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="997b4-147">アイテムが以前に送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="997b4-147">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="997b4-148">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="997b4-148">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="997b4-149">アイテムが変更されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="997b4-149">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="997b4-150">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="997b4-150">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="997b4-151">メールボックス内のアイテムに含まれるすべてのインターネットメッセージヘッダーのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="997b4-151">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="997b4-152">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="997b4-152">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="997b4-153">メールボックス内のアイテムが送信された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="997b4-153">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="997b4-154">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="997b4-154">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="997b4-155">メールボックス内の特定のアイテムが作成された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="997b4-155">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="997b4-156">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="997b4-156">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="997b4-157">Exchange ストア内のアイテムに関連付けられているすべての response オブジェクトのコレクションを格納します。</span><span class="sxs-lookup"><span data-stu-id="997b4-157">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="997b4-158">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="997b4-158">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="997b4-159">イベントが発生した日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="997b4-159">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="997b4-160">これは、アラームがいつ表示されるかを決定するために[ReminderMinutesBeforeStart](reminderminutesbeforestart.md)要素によって使用されます。</span><span class="sxs-lookup"><span data-stu-id="997b4-160">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="997b4-161">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="997b4-161">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="997b4-162">Exchange ストア内のアイテムにアラームが設定されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="997b4-162">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="997b4-163">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="997b4-163">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="997b4-164">アラームが表示されるイベントの前の時間 (分単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="997b4-164">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="997b4-165">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="997b4-165">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="997b4-166">[Cc] ボックスの内容に使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="997b4-166">Represents the display string that is used for the contents of the Cc box.</span></span> <span data-ttu-id="997b4-167">これは、すべての Cc 受信者表示名の連結された文字列です。</span><span class="sxs-lookup"><span data-stu-id="997b4-167">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="997b4-168">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="997b4-168">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="997b4-169">[宛先] ボックスの内容に対して使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="997b4-169">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="997b4-170">これは、すべての受信者の表示名の連結文字列です。</span><span class="sxs-lookup"><span data-stu-id="997b4-170">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="997b4-171">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="997b4-171">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="997b4-172">アイテムに少なくとも1つの添付ファイルがある場合に**true**に設定されるプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="997b4-172">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="997b4-173">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="997b4-173">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="997b4-174">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="997b4-174">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="997b4-175">フォルダーとアイテムの拡張プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="997b4-175">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="997b4-176">Culture</span><span class="sxs-lookup"><span data-stu-id="997b4-176">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="997b4-177">メールボックス内の特定のアイテムのカルチャを表します。</span><span class="sxs-lookup"><span data-stu-id="997b4-177">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="997b4-178">ActualWork</span><span class="sxs-lookup"><span data-stu-id="997b4-178">ActualWork</span></span>](actualwork.md) <br/> |<span data-ttu-id="997b4-179">タスクに費やした実績時間を表します。</span><span class="sxs-lookup"><span data-stu-id="997b4-179">Represents the actual amount of time that is spent on a task.</span></span>  <br/> |
|[<span data-ttu-id="997b4-180">AssignedTime</span><span class="sxs-lookup"><span data-stu-id="997b4-180">AssignedTime</span></span>](assignedtime.md) <br/> |<span data-ttu-id="997b4-181">仕事が連絡先に割り当てられている時間を表します。</span><span class="sxs-lookup"><span data-stu-id="997b4-181">Represents the time when a task is assigned to a contact.</span></span>  <br/> |
|[<span data-ttu-id="997b4-182">BillingInformation</span><span class="sxs-lookup"><span data-stu-id="997b4-182">BillingInformation</span></span>](billinginformation.md) <br/> |<span data-ttu-id="997b4-183">タスクの請求情報を保持します。</span><span class="sxs-lookup"><span data-stu-id="997b4-183">Holds billing information for a task.</span></span>  <br/> |
|[<span data-ttu-id="997b4-184">ChangeCount</span><span class="sxs-lookup"><span data-stu-id="997b4-184">ChangeCount</span></span>](changecount.md) <br/> |<span data-ttu-id="997b4-185">タスクのバージョンを指定します。</span><span class="sxs-lookup"><span data-stu-id="997b4-185">Specifies the version of the task.</span></span>  <br/> |
|[<span data-ttu-id="997b4-186">Companies</span><span class="sxs-lookup"><span data-stu-id="997b4-186">Companies</span></span>](companies.md) <br/> |<span data-ttu-id="997b4-187">連絡先またはタスクに関連付けられている会社のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="997b4-187">Represents the collection of companies that are associated with a contact or task.</span></span>  <br/> |
|[<span data-ttu-id="997b4-188">CompleteDate</span><span class="sxs-lookup"><span data-stu-id="997b4-188">CompleteDate</span></span>](completedate.md) <br/> |<span data-ttu-id="997b4-189">タスクが完了する日付を表します。</span><span class="sxs-lookup"><span data-stu-id="997b4-189">Represents the date on which a task is completed.</span></span>  <br/> |
|[<span data-ttu-id="997b4-190">連絡先</span><span class="sxs-lookup"><span data-stu-id="997b4-190">Contacts</span></span>](contacts-ex15websvcsotherref.md) <br/> |<span data-ttu-id="997b4-191">タスクに関連付けられている連絡先の一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="997b4-191">Contains a list of contacts that are associated with a task.</span></span>  <br/> |
|[<span data-ttu-id="997b4-192">DelegationState</span><span class="sxs-lookup"><span data-stu-id="997b4-192">DelegationState</span></span>](delegationstate.md) <br/> |<span data-ttu-id="997b4-193">委任されたタスクの状態を表します。</span><span class="sxs-lookup"><span data-stu-id="997b4-193">Represents the status of a delegated task.</span></span>  <br/> |
|[<span data-ttu-id="997b4-194">Delegator</span><span class="sxs-lookup"><span data-stu-id="997b4-194">Delegator</span></span>](delegator.md) <br/> |<span data-ttu-id="997b4-195">タスクを割り当てた委任者の名前が含まれます。</span><span class="sxs-lookup"><span data-stu-id="997b4-195">Contains the name of the delegator who assigned the task.</span></span>  <br/> |
|[<span data-ttu-id="997b4-196">DueDate</span><span class="sxs-lookup"><span data-stu-id="997b4-196">DueDate</span></span>](duedate.md) <br/> |<span data-ttu-id="997b4-197">タスクアイテムの期限の日付を表します。</span><span class="sxs-lookup"><span data-stu-id="997b4-197">Represents the date when a task item is due.</span></span>  <br/> |
|[<span data-ttu-id="997b4-198">Is割り当て編集可能</span><span class="sxs-lookup"><span data-stu-id="997b4-198">IsAssignmentEditable</span></span>](isassignmenteditable.md) <br/> |<span data-ttu-id="997b4-199">タスクが編集可能であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="997b4-199">Indicates whether the task is editable or not.</span></span>  <br/> |
|[<span data-ttu-id="997b4-200">IsComplete</span><span class="sxs-lookup"><span data-stu-id="997b4-200">IsComplete</span></span>](iscomplete.md) <br/> |<span data-ttu-id="997b4-201">タスクが完了したかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="997b4-201">Indicates whether the task has been completed or not.</span></span>  <br/> |
|[<span data-ttu-id="997b4-202">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="997b4-202">IsRecurring</span></span>](isrecurring.md) <br/> |<span data-ttu-id="997b4-203">タスクが定期的なアイテムの一部であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="997b4-203">Indicates whether a task is part of a recurring item.</span></span> <span data-ttu-id="997b4-204">この要素は値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="997b4-204">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="997b4-205">IsTeamTask</span><span class="sxs-lookup"><span data-stu-id="997b4-205">IsTeamTask</span></span>](isteamtask.md) <br/> |<span data-ttu-id="997b4-206">タスクがチームによって所有されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="997b4-206">Indicates whether the task is owned by a team or not.</span></span>  <br/> |
|[<span data-ttu-id="997b4-207">Mileage</span><span class="sxs-lookup"><span data-stu-id="997b4-207">Mileage</span></span>](mileage.md) <br/> |<span data-ttu-id="997b4-208">タスクアイテムのマイレージを表します。</span><span class="sxs-lookup"><span data-stu-id="997b4-208">Represents mileage for a task item.</span></span>  <br/> |
|[<span data-ttu-id="997b4-209">Owner</span><span class="sxs-lookup"><span data-stu-id="997b4-209">Owner</span></span>](owner.md) <br/> |<span data-ttu-id="997b4-210">タスクの所有者を表します。</span><span class="sxs-lookup"><span data-stu-id="997b4-210">Represents the owner of a task.</span></span>  <br/> |
|[<span data-ttu-id="997b4-211">PercentComplete</span><span class="sxs-lookup"><span data-stu-id="997b4-211">PercentComplete</span></span>](percentcomplete.md) <br/> |<span data-ttu-id="997b4-212">タスクの完了状態を表します。</span><span class="sxs-lookup"><span data-stu-id="997b4-212">Describes the completion status of a task.</span></span>  <br/> |
|[<span data-ttu-id="997b4-213">定期的なアイテム (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="997b4-213">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="997b4-214">定期的なタスクの定期的なアイテムの情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="997b4-214">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="997b4-215">StartDate</span><span class="sxs-lookup"><span data-stu-id="997b4-215">StartDate</span></span>](startdate.md) <br/> |<span data-ttu-id="997b4-216">タスクアイテムの開始日を表します。</span><span class="sxs-lookup"><span data-stu-id="997b4-216">Represents the start date of a task item.</span></span>  <br/> |
|[<span data-ttu-id="997b4-217">状態</span><span class="sxs-lookup"><span data-stu-id="997b4-217">Status</span></span>](status.md) <br/> |<span data-ttu-id="997b4-218">タスクアイテムの状態を表します。</span><span class="sxs-lookup"><span data-stu-id="997b4-218">Represents the status of a task item.</span></span>  <br/> |
|[<span data-ttu-id="997b4-219">StatusDescription</span><span class="sxs-lookup"><span data-stu-id="997b4-219">StatusDescription</span></span>](statusdescription.md) <br/> |<span data-ttu-id="997b4-220">タスクの進捗状況の説明を格納します。</span><span class="sxs-lookup"><span data-stu-id="997b4-220">Contains an explanation of the task status.</span></span>  <br/> |
|[<span data-ttu-id="997b4-221">TotalWork</span><span class="sxs-lookup"><span data-stu-id="997b4-221">TotalWork</span></span>](totalwork.md) <br/> |<span data-ttu-id="997b4-222">アイテムに関連付けられている作業量の説明を格納します。</span><span class="sxs-lookup"><span data-stu-id="997b4-222">Contains a description of how much work is associated with an item.</span></span>  <br/> |
|[<span data-ttu-id="997b4-223">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="997b4-223">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="997b4-224">アイテムまたはフォルダーのアクセス許可の設定に基づいて、クライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="997b4-224">Contains the rights of the client based on the permission settings for the item or folder.</span></span> <span data-ttu-id="997b4-225">この要素は値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="997b4-225">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="997b4-226">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="997b4-226">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="997b4-227">アイテムを最後に変更したユーザーの表示名を含みます。</span><span class="sxs-lookup"><span data-stu-id="997b4-227">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="997b4-228">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="997b4-228">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="997b4-229">アイテムが最後に変更された日時を示します。</span><span class="sxs-lookup"><span data-stu-id="997b4-229">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="997b4-230">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="997b4-230">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="997b4-231">アイテムがフォルダーに関連付けられているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="997b4-231">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="997b4-232">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="997b4-232">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="997b4-233">Outlook Web app のアイテムを読み取るために Microsoft Office Outlook Web App エンドポイントに連結する URL を表します。</span><span class="sxs-lookup"><span data-stu-id="997b4-233">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="997b4-234">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="997b4-234">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="997b4-235">Outlook web app エンドポイントに連結して Outlook Web App のアイテムを編集するための URL を表します。</span><span class="sxs-lookup"><span data-stu-id="997b4-235">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="997b4-236">ConversationId</span><span class="sxs-lookup"><span data-stu-id="997b4-236">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="997b4-237">アイテムまたは会話の識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="997b4-237">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="997b4-238">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="997b4-238">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="997b4-239">この会話の一意の本文を表す HTML フラグメントまたはプレーンテキストを表します。</span><span class="sxs-lookup"><span data-stu-id="997b4-239">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="997b4-240">親要素</span><span class="sxs-lookup"><span data-stu-id="997b4-240">Parent elements</span></span>

|<span data-ttu-id="997b4-241">**要素**</span><span class="sxs-lookup"><span data-stu-id="997b4-241">**Element**</span></span>|<span data-ttu-id="997b4-242">**説明**</span><span class="sxs-lookup"><span data-stu-id="997b4-242">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="997b4-243">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="997b4-243">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="997b4-244">会議の時刻に隣接しているすべての予定表アイテムを説明します。</span><span class="sxs-lookup"><span data-stu-id="997b4-244">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="997b4-245">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="997b4-245">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="997b4-246">[Updateitem 操作](updateitem-operation.md)中に、アイテム/フォルダーの1つのプロパティに追加するデータを識別します。</span><span class="sxs-lookup"><span data-stu-id="997b4-246">Identifies data to append to a single property of an item/folder during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="997b4-247">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="997b4-247">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="997b4-248">会議の時間と競合するすべてのアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="997b4-248">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="997b4-249">Create (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="997b4-249">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="997b4-250">ローカルクライアントストアに作成する単一のアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="997b4-250">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="997b4-251">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="997b4-251">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="997b4-252">別の Exchange アイテムに関連付けられている Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="997b4-252">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="997b4-253">Items</span><span class="sxs-lookup"><span data-stu-id="997b4-253">Items</span></span>](items.md) <br/> |<span data-ttu-id="997b4-254">項目の配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="997b4-254">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="997b4-255">SetItemField</span><span class="sxs-lookup"><span data-stu-id="997b4-255">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="997b4-256">[Updateitem 操作](updateitem-operation.md)のアイテムの1つのプロパティに対する更新を表します。</span><span class="sxs-lookup"><span data-stu-id="997b4-256">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="997b4-257">Update (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="997b4-257">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="997b4-258">ローカルクライアントストアで更新する単一のアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="997b4-258">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="997b4-259">テキスト値</span><span class="sxs-lookup"><span data-stu-id="997b4-259">Text value</span></span>

<span data-ttu-id="997b4-260">なし。</span><span class="sxs-lookup"><span data-stu-id="997b4-260">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="997b4-261">注釈</span><span class="sxs-lookup"><span data-stu-id="997b4-261">Remarks</span></span>

<span data-ttu-id="997b4-262">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="997b4-262">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="997b4-263">要素の情報</span><span class="sxs-lookup"><span data-stu-id="997b4-263">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="997b4-264">Namespace</span><span class="sxs-lookup"><span data-stu-id="997b4-264">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="997b4-265">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="997b4-265">Schema name</span></span>  <br/> |<span data-ttu-id="997b4-266">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="997b4-266">Types schema</span></span>  <br/> |
|<span data-ttu-id="997b4-267">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="997b4-267">Validation file</span></span>  <br/> |<span data-ttu-id="997b4-268">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="997b4-268">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="997b4-269">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="997b4-269">Can be empty</span></span>  <br/> |<span data-ttu-id="997b4-270">正しくない</span><span class="sxs-lookup"><span data-stu-id="997b4-270">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="997b4-271">関連項目</span><span class="sxs-lookup"><span data-stu-id="997b4-271">See also</span></span>

- [<span data-ttu-id="997b4-272">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="997b4-272">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="997b4-273">タスクの作成</span><span class="sxs-lookup"><span data-stu-id="997b4-273">Creating Tasks</span></span>](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
- [<span data-ttu-id="997b4-274">タスクの削除</span><span class="sxs-lookup"><span data-stu-id="997b4-274">Deleting Tasks</span></span>](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

