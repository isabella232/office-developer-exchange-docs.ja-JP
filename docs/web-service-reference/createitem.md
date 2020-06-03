---
title: CreateItem
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
ms.assetid: c3707feb-3fd4-4b8a-a68f-2abadd455163
description: CreateItem 要素は、Exchange ストア内のアイテムを作成するための要求を定義します。
ms.openlocfilehash: 235664b7baeceeccb14135fd346123f0f7d99346
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527062"
---
# <a name="createitem"></a><span data-ttu-id="14a83-103">CreateItem</span><span class="sxs-lookup"><span data-stu-id="14a83-103">CreateItem</span></span>

<span data-ttu-id="14a83-104">**CreateItem**要素は、Exchange ストア内のアイテムを作成するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="14a83-104">The **CreateItem** element defines a request to create an item in the Exchange store.</span></span> 
  
```xml
<CreateItem MessageDisposition="" SendMeetingInvitations="">
   <SavedItemFolderId/>
   <Items/>
</CreateItem>
```

<span data-ttu-id="14a83-105">**CreateItemType**</span><span class="sxs-lookup"><span data-stu-id="14a83-105">**CreateItemType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="14a83-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="14a83-106">Attributes and elements</span></span>

<span data-ttu-id="14a83-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="14a83-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="14a83-108">属性</span><span class="sxs-lookup"><span data-stu-id="14a83-108">Attributes</span></span>

|<span data-ttu-id="14a83-109">属性</span><span class="sxs-lookup"><span data-stu-id="14a83-109">Attribute</span></span>|<span data-ttu-id="14a83-110">説明</span><span class="sxs-lookup"><span data-stu-id="14a83-110">Description</span></span>|
|:-----|:-----|
|<span data-ttu-id="14a83-111">**MessageDisposition**</span><span class="sxs-lookup"><span data-stu-id="14a83-111">**MessageDisposition**</span></span> <br/> |<span data-ttu-id="14a83-112">アイテムが作成された後に処理される方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="14a83-112">Describes how the item will be handled after it is created.</span></span> <span data-ttu-id="14a83-113">電子メールメッセージの属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="14a83-113">The attribute is required for e-mail messages.</span></span> <span data-ttu-id="14a83-114">この属性は、電子メールメッセージにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="14a83-114">This attribute is only applicable to e-mail messages.</span></span>  <br/> |
|<span data-ttu-id="14a83-115">**Send会議の招待**</span><span class="sxs-lookup"><span data-stu-id="14a83-115">**SendMeetingInvitations**</span></span> <br/> |<span data-ttu-id="14a83-116">会議出席依頼が作成された後に処理される方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="14a83-116">Describes how meeting requests are handled after they are created.</span></span> <span data-ttu-id="14a83-117">この属性は、予定表アイテムに必要です。</span><span class="sxs-lookup"><span data-stu-id="14a83-117">This attribute is required for calendar items.</span></span>  <br/> |
   
#### <a name="messagedisposition-attribute"></a><span data-ttu-id="14a83-118">MessageDisposition 属性</span><span class="sxs-lookup"><span data-stu-id="14a83-118">MessageDisposition Attribute</span></span>

|<span data-ttu-id="14a83-119">値</span><span class="sxs-lookup"><span data-stu-id="14a83-119">Value</span></span>|<span data-ttu-id="14a83-120">説明</span><span class="sxs-lookup"><span data-stu-id="14a83-120">Description</span></span>|
|:-----|:-----|
|<span data-ttu-id="14a83-121">SaveOnly</span><span class="sxs-lookup"><span data-stu-id="14a83-121">SaveOnly</span></span>  <br/> |<span data-ttu-id="14a83-122">メッセージアイテムは、 [SavedItemFolderId](saveditemfolderid.md)要素によって指定されたフォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="14a83-122">The message item is saved in the folder that is specified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span> <span data-ttu-id="14a83-123">メッセージは、 [SendItem 操作](senditem-operation.md)を使用して後で送信できます。</span><span class="sxs-lookup"><span data-stu-id="14a83-123">Messages can be sent later by using the [SendItem operation](senditem-operation.md).</span></span> <span data-ttu-id="14a83-124">アイテム識別子が応答で返されます。</span><span class="sxs-lookup"><span data-stu-id="14a83-124">An item identifier is returned in the response.</span></span> <span data-ttu-id="14a83-125">アイテムの識別子は、メッセージアイテム以外のアイテムの種類に対しては返されません。</span><span class="sxs-lookup"><span data-stu-id="14a83-125">Item identifiers are not returned for any item types except for message items.</span></span> <span data-ttu-id="14a83-126">これには、応答オブジェクトが含まれます。</span><span class="sxs-lookup"><span data-stu-id="14a83-126">This includes response objects.</span></span>  <br/> |
|<span data-ttu-id="14a83-127">SendOnly</span><span class="sxs-lookup"><span data-stu-id="14a83-127">SendOnly</span></span>  <br/> |<span data-ttu-id="14a83-128">アイテムは送信されますが、[送信済みアイテム] フォルダーにコピーは保存されません。</span><span class="sxs-lookup"><span data-stu-id="14a83-128">The item is sent but no copy is saved in the Sent Items folder.</span></span> <span data-ttu-id="14a83-129">応答では、アイテム識別子は返されません。</span><span class="sxs-lookup"><span data-stu-id="14a83-129">An item identifier is not returned in the response.</span></span><br/><br/><span data-ttu-id="14a83-130">**注**: このオプションでは宛先フォルダーを指定できないため、 **CreateItem**は、sendonly オプションが使用されている場合は代理人アクセスをサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="14a83-130">**NOTE**: **CreateItem** does not support delegate access when the SendOnly option is used because a destination folder cannot be specified with this option.</span></span> <span data-ttu-id="14a83-131">回避策として、アイテムを作成し、アイテム識別子を取得してから、SendItem 操作を使用してアイテムを送信します。</span><span class="sxs-lookup"><span data-stu-id="14a83-131">The workaround is to create the item, get the item identifier, and then use the SendItem operation to send the item.</span></span>           |
|<span data-ttu-id="14a83-132">SendAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="14a83-132">SendAndSaveCopy</span></span>  <br/> |<span data-ttu-id="14a83-133">アイテムが送信され、 [SavedItemFolderId](saveditemfolderid.md)要素によって識別されるフォルダーにコピーが保存されます。</span><span class="sxs-lookup"><span data-stu-id="14a83-133">The item is sent and a copy is saved in the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span> <span data-ttu-id="14a83-134">応答では、アイテム識別子は返されません。</span><span class="sxs-lookup"><span data-stu-id="14a83-134">An item identifier is not returned in the response.</span></span><br/><br/><span data-ttu-id="14a83-135">**注**: 会議出席依頼は、 [SavedItemFolderId](saveditemfolderid.md)プロパティによって指定されたフォルダーには保存されません。</span><span class="sxs-lookup"><span data-stu-id="14a83-135">**NOTE**: Meeting requests are not saved to the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) property.</span></span> <span data-ttu-id="14a83-136">予定表の場合、 **SavedItemFolderId**プロパティで指定できるのは、予定表アイテムの保存場所のみです。</span><span class="sxs-lookup"><span data-stu-id="14a83-136">For calendaring, only the save location for calendar items can be specified by the **SavedItemFolderId** property.</span></span> <span data-ttu-id="14a83-137">会議出席依頼アイテムが保存される場所を制御することはできません。</span><span class="sxs-lookup"><span data-stu-id="14a83-137">You cannot control where a meeting request item is saved.</span></span> <span data-ttu-id="14a83-138">関連付けられた予定表アイテムのみがコピーされ、 **SavedItemFolderId**プロパティによって識別されるフォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="14a83-138">Only the associated calendar items are copied and saved into the folder that is identified by the **SavedItemFolderId** property.</span></span>           |
   
#### <a name="sendmeetinginvitations-attribute"></a><span data-ttu-id="14a83-139">Send会議の招待の属性</span><span class="sxs-lookup"><span data-stu-id="14a83-139">SendMeetingInvitations Attribute</span></span>

|<span data-ttu-id="14a83-140">値</span><span class="sxs-lookup"><span data-stu-id="14a83-140">Value</span></span>|<span data-ttu-id="14a83-141">説明</span><span class="sxs-lookup"><span data-stu-id="14a83-141">Description</span></span>|
|:-----|:-----|
|<span data-ttu-id="14a83-142">SendToNone</span><span class="sxs-lookup"><span data-stu-id="14a83-142">SendToNone</span></span>  <br/> |<span data-ttu-id="14a83-143">アイテムが会議出席依頼の場合、予定表アイテムとして保存されますが、送信されません。</span><span class="sxs-lookup"><span data-stu-id="14a83-143">If the item is a meeting request, it is saved as a calendar item but not sent.</span></span>  <br/> |
|<span data-ttu-id="14a83-144">SendOnlyToAll</span><span class="sxs-lookup"><span data-stu-id="14a83-144">SendOnlyToAll</span></span>  <br/> |<span data-ttu-id="14a83-145">会議出席依頼はすべての出席者に送信されますが、[送信済みアイテム] フォルダーには保存されません。</span><span class="sxs-lookup"><span data-stu-id="14a83-145">The meeting request is sent to all attendees but is not saved in the Sent Items folder.</span></span>  <br/> |
|<span data-ttu-id="14a83-146">SendToAllAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="14a83-146">SendToAllAndSaveCopy</span></span>  <br/> |<span data-ttu-id="14a83-147">会議出席依頼はすべての出席者に送信され、 [SavedItemFolderId](saveditemfolderid.md)要素によって識別されるフォルダーにコピーが保存されます。</span><span class="sxs-lookup"><span data-stu-id="14a83-147">The meeting request is sent to all attendees and a copy is saved in the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="14a83-148">子要素</span><span class="sxs-lookup"><span data-stu-id="14a83-148">Child elements</span></span>

|<span data-ttu-id="14a83-149">要素</span><span class="sxs-lookup"><span data-stu-id="14a83-149">Element</span></span>|<span data-ttu-id="14a83-150">説明</span><span class="sxs-lookup"><span data-stu-id="14a83-150">Description</span></span>|
|:-----|:-----|
|[<span data-ttu-id="14a83-151">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="14a83-151">SavedItemFolderId</span></span>](saveditemfolderid.md) <br/> |<span data-ttu-id="14a83-152">新しいアイテムを作成できるターゲットフォルダーを指定します。</span><span class="sxs-lookup"><span data-stu-id="14a83-152">Identifies the target folder where a new item can be created.</span></span> <span data-ttu-id="14a83-153">**MessageDisposition**属性が sendonly に設定されている場合は、作成されたメッセージのみが送信されます。</span><span class="sxs-lookup"><span data-stu-id="14a83-153">If the **MessageDisposition** attribute is set to SendOnly, a created message will only be sent.</span></span> <span data-ttu-id="14a83-154">このメッセージは、 [SavedItemFolderId](saveditemfolderid.md)要素によって識別されるフォルダーには配置されません。</span><span class="sxs-lookup"><span data-stu-id="14a83-154">The message will not be put in the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="14a83-155">アイテム (非 Emptyarrayofallitemstype)</span><span class="sxs-lookup"><span data-stu-id="14a83-155">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="14a83-156">[SavedItemFolderId](saveditemfolderid.md)要素によって識別されるフォルダー内に作成するアイテムの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="14a83-156">Contains an array of items to create in the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="14a83-157">親要素</span><span class="sxs-lookup"><span data-stu-id="14a83-157">Parent elements</span></span>

<span data-ttu-id="14a83-158">なし。</span><span class="sxs-lookup"><span data-stu-id="14a83-158">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="14a83-159">注釈</span><span class="sxs-lookup"><span data-stu-id="14a83-159">Remarks</span></span>

<span data-ttu-id="14a83-160">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="14a83-160">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="14a83-161">要素の情報</span><span class="sxs-lookup"><span data-stu-id="14a83-161">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="14a83-162">Namespace</span><span class="sxs-lookup"><span data-stu-id="14a83-162">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="14a83-163">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="14a83-163">Schema Name</span></span>  <br/> |<span data-ttu-id="14a83-164">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="14a83-164">Messages schema</span></span>  <br/> |
|<span data-ttu-id="14a83-165">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="14a83-165">Validation File</span></span>  <br/> |<span data-ttu-id="14a83-166">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="14a83-166">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="14a83-167">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="14a83-167">Can be Empty</span></span>  <br/> |<span data-ttu-id="14a83-168">正しくない</span><span class="sxs-lookup"><span data-stu-id="14a83-168">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="14a83-169">関連項目</span><span class="sxs-lookup"><span data-stu-id="14a83-169">See also</span></span>

- [<span data-ttu-id="14a83-170">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="14a83-170">CreateItemResponse</span></span>](createitemresponse.md)  
- [<span data-ttu-id="14a83-171">CreateItem 操作</span><span class="sxs-lookup"><span data-stu-id="14a83-171">CreateItem operation</span></span>](createitem-operation.md)
- [<span data-ttu-id="14a83-172">電子メールメッセージの作成</span><span class="sxs-lookup"><span data-stu-id="14a83-172">Creating E-mail Messages</span></span>](https://msdn.microsoft.com/library/05bfb83c-2866-427d-a9fe-14ba3cb02793%28Office.15%29.aspx) 
- [<span data-ttu-id="14a83-173">連絡先の作成 (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="14a83-173">Creating Contacts (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)  
- [<span data-ttu-id="14a83-174">タスクの作成</span><span class="sxs-lookup"><span data-stu-id="14a83-174">Creating Tasks</span></span>](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx) 
- [<span data-ttu-id="14a83-175">予定の作成</span><span class="sxs-lookup"><span data-stu-id="14a83-175">Creating Appointments</span></span>](https://msdn.microsoft.com/library/2385391e-c9e7-4d45-b803-c4ff94d5c94e%28Office.15%29.aspx)

