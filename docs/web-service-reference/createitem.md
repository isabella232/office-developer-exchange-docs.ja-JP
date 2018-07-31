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
description: CreateItem 要素は、Exchange ストア内のアイテムを作成する要求を定義します。
ms.openlocfilehash: 9453323bff07749f5852dae75284c61c0895adb6
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353127"
---
# <a name="createitem"></a><span data-ttu-id="01ceb-103">CreateItem</span><span class="sxs-lookup"><span data-stu-id="01ceb-103">CreateItem</span></span>

<span data-ttu-id="01ceb-104">**CreateItem**要素は、Exchange ストア内のアイテムを作成する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="01ceb-104">The **CreateItem** element defines a request to create an item in the Exchange store.</span></span> 
  
```xml
<CreateItem MessageDisposition="" SendMeetingInvitations="">
   <SavedItemFolderId/>
   <Items/>
</CreateItem>
```

<span data-ttu-id="01ceb-105">**CreateItemType**</span><span class="sxs-lookup"><span data-stu-id="01ceb-105">**CreateItemType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="01ceb-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="01ceb-106">Attributes and elements</span></span>

<span data-ttu-id="01ceb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="01ceb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="01ceb-108">属性</span><span class="sxs-lookup"><span data-stu-id="01ceb-108">Attributes</span></span>

|<span data-ttu-id="01ceb-109">属性</span><span class="sxs-lookup"><span data-stu-id="01ceb-109">Attribute</span></span>|<span data-ttu-id="01ceb-110">説明</span><span class="sxs-lookup"><span data-stu-id="01ceb-110">Description</span></span>|
|:-----|:-----|
|<span data-ttu-id="01ceb-111">**MessageDisposition**</span><span class="sxs-lookup"><span data-stu-id="01ceb-111">**MessageDisposition**</span></span> <br/> |<span data-ttu-id="01ceb-112">作成後のアイテムの処理方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="01ceb-112">Describes how the item will be handled after it is created.</span></span> <span data-ttu-id="01ceb-113">属性は、電子メール メッセージに必要です。</span><span class="sxs-lookup"><span data-stu-id="01ceb-113">The attribute is required for e-mail messages.</span></span> <span data-ttu-id="01ceb-114">この属性は、電子メール メッセージに該当する場合のみです。</span><span class="sxs-lookup"><span data-stu-id="01ceb-114">This attribute is only applicable to e-mail messages.</span></span>  <br/> |
|<span data-ttu-id="01ceb-115">**SendMeetingInvitations**</span><span class="sxs-lookup"><span data-stu-id="01ceb-115">**SendMeetingInvitations**</span></span> <br/> |<span data-ttu-id="01ceb-116">作成後に会議出席依頼を処理する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="01ceb-116">Describes how meeting requests are handled after they are created.</span></span> <span data-ttu-id="01ceb-117">この属性は、予定表アイテムの必要があります。</span><span class="sxs-lookup"><span data-stu-id="01ceb-117">This attribute is required for calendar items.</span></span>  <br/> |
   
#### <a name="messagedisposition-attribute"></a><span data-ttu-id="01ceb-118">MessageDisposition 属性</span><span class="sxs-lookup"><span data-stu-id="01ceb-118">MessageDisposition Attribute</span></span>

|<span data-ttu-id="01ceb-119">値</span><span class="sxs-lookup"><span data-stu-id="01ceb-119">Value</span></span>|<span data-ttu-id="01ceb-120">説明</span><span class="sxs-lookup"><span data-stu-id="01ceb-120">Description</span></span>|
|:-----|:-----|
|<span data-ttu-id="01ceb-121">SaveOnly</span><span class="sxs-lookup"><span data-stu-id="01ceb-121">SaveOnly</span></span>  <br/> |<span data-ttu-id="01ceb-122">メッセージ アイテムは、 [SavedItemFolderId](saveditemfolderid.md)要素で指定されているフォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="01ceb-122">The message item is saved in the folder that is specified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span> <span data-ttu-id="01ceb-123">[SendItem 操作](senditem-operation.md)を使用してメッセージを後で送信することができます。</span><span class="sxs-lookup"><span data-stu-id="01ceb-123">Messages can be sent later by using the [SendItem operation](senditem-operation.md).</span></span> <span data-ttu-id="01ceb-124">アイテム識別子は、応答で返されます。</span><span class="sxs-lookup"><span data-stu-id="01ceb-124">An item identifier is returned in the response.</span></span> <span data-ttu-id="01ceb-125">メッセージ アイテム以外の項目の種類の項目の識別子は返されません。</span><span class="sxs-lookup"><span data-stu-id="01ceb-125">Item identifiers are not returned for any item types except for message items.</span></span> <span data-ttu-id="01ceb-126">これには、応答オブジェクトが含まれます。</span><span class="sxs-lookup"><span data-stu-id="01ceb-126">This includes response objects.</span></span>  <br/> |
|<span data-ttu-id="01ceb-127">SendOnly</span><span class="sxs-lookup"><span data-stu-id="01ceb-127">SendOnly</span></span>  <br/> |<span data-ttu-id="01ceb-128">アイテムを送信しますが、送信済みアイテム フォルダーにコピーは保存されません。</span><span class="sxs-lookup"><span data-stu-id="01ceb-128">The item is sent but no copy is saved in the Sent Items folder.</span></span> <span data-ttu-id="01ceb-129">アイテム識別子は、応答で返されません。</span><span class="sxs-lookup"><span data-stu-id="01ceb-129">An item identifier is not returned in the response.</span></span><br/><br/><span data-ttu-id="01ceb-130">**注**: **createitem メソッド**がデリゲートのアクセスをサポートしていませんこのオプションを使用してインストール先のフォルダーを指定することはできませんので、SendOnly オプションを使用するとします。</span><span class="sxs-lookup"><span data-stu-id="01ceb-130">**NOTE**: **CreateItem** does not support delegate access when the SendOnly option is used because a destination folder cannot be specified with this option.</span></span> <span data-ttu-id="01ceb-131">回避するに項目を作成し、項目の識別子を取得する、SendItem 操作を使用して、アイテムを送信するには。</span><span class="sxs-lookup"><span data-stu-id="01ceb-131">The workaround is to create the item, get the item identifier, and then use the SendItem operation to send the item.</span></span>           |
|<span data-ttu-id="01ceb-132">SendAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="01ceb-132">SendAndSaveCopy</span></span>  <br/> |<span data-ttu-id="01ceb-133">アイテムが送信され、 [SavedItemFolderId](saveditemfolderid.md)要素で指定されているフォルダーにコピーが保存されます。</span><span class="sxs-lookup"><span data-stu-id="01ceb-133">The item is sent and a copy is saved in the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span> <span data-ttu-id="01ceb-134">アイテム識別子は、応答で返されません。</span><span class="sxs-lookup"><span data-stu-id="01ceb-134">An item identifier is not returned in the response.</span></span><br/><br/><span data-ttu-id="01ceb-135">**注**: 会議出席依頼は、 [SavedItemFolderId](saveditemfolderid.md)プロパティで指定されたフォルダーには保存されません。</span><span class="sxs-lookup"><span data-stu-id="01ceb-135">**NOTE**: Meeting requests are not saved to the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) property.</span></span> <span data-ttu-id="01ceb-136">予定表の作成、保存だけの**SavedItemFolderId**プロパティによって予定表アイテムの場所を指定することができます。</span><span class="sxs-lookup"><span data-stu-id="01ceb-136">For calendaring, only the save location for calendar items can be specified by the **SavedItemFolderId** property.</span></span> <span data-ttu-id="01ceb-137">会議出席依頼アイテムの保存場所を制御することはできません。</span><span class="sxs-lookup"><span data-stu-id="01ceb-137">You cannot control where a meeting request item is saved.</span></span> <span data-ttu-id="01ceb-138">関連付けられている予定表アイテムのみがコピーされ、 **SavedItemFolderId**プロパティで指定されたフォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="01ceb-138">Only the associated calendar items are copied and saved into the folder that is identified by the **SavedItemFolderId** property.</span></span>           |
   
#### <a name="sendmeetinginvitations-attribute"></a><span data-ttu-id="01ceb-139">SendMeetingInvitations 属性</span><span class="sxs-lookup"><span data-stu-id="01ceb-139">SendMeetingInvitations Attribute</span></span>

|<span data-ttu-id="01ceb-140">値</span><span class="sxs-lookup"><span data-stu-id="01ceb-140">Value</span></span>|<span data-ttu-id="01ceb-141">説明</span><span class="sxs-lookup"><span data-stu-id="01ceb-141">Description</span></span>|
|:-----|:-----|
|<span data-ttu-id="01ceb-142">SendToNone</span><span class="sxs-lookup"><span data-stu-id="01ceb-142">SendToNone</span></span>  <br/> |<span data-ttu-id="01ceb-143">アイテムが会議出席依頼の場合は、これは予定表のアイテムとして保存しますが、送信されません。</span><span class="sxs-lookup"><span data-stu-id="01ceb-143">If the item is a meeting request, it is saved as a calendar item but not sent.</span></span>  <br/> |
|<span data-ttu-id="01ceb-144">SendOnlyToAll</span><span class="sxs-lookup"><span data-stu-id="01ceb-144">SendOnlyToAll</span></span>  <br/> |<span data-ttu-id="01ceb-145">会議出席依頼は、すべての出席者に送信されますが、送信済みアイテム フォルダーには保存されません。</span><span class="sxs-lookup"><span data-stu-id="01ceb-145">The meeting request is sent to all attendees but is not saved in the Sent Items folder.</span></span>  <br/> |
|<span data-ttu-id="01ceb-146">SendToAllAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="01ceb-146">SendToAllAndSaveCopy</span></span>  <br/> |<span data-ttu-id="01ceb-147">すべての出席者に会議出席依頼が送信され、 [SavedItemFolderId](saveditemfolderid.md)要素で指定されているフォルダーにコピーが保存されます。</span><span class="sxs-lookup"><span data-stu-id="01ceb-147">The meeting request is sent to all attendees and a copy is saved in the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="01ceb-148">子要素</span><span class="sxs-lookup"><span data-stu-id="01ceb-148">Child elements</span></span>

|<span data-ttu-id="01ceb-149">要素</span><span class="sxs-lookup"><span data-stu-id="01ceb-149">Element</span></span>|<span data-ttu-id="01ceb-150">説明</span><span class="sxs-lookup"><span data-stu-id="01ceb-150">Description</span></span>|
|:-----|:-----|
|[<span data-ttu-id="01ceb-151">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="01ceb-151">SavedItemFolderId</span></span>](saveditemfolderid.md) <br/> |<span data-ttu-id="01ceb-152">新しいアイテムを作成することができますターゲット フォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="01ceb-152">Identifies the target folder where a new item can be created.</span></span> <span data-ttu-id="01ceb-153">**MessageDisposition**属性は、SendOnly に設定されている場合は、作成したメッセージのみ送信されます。</span><span class="sxs-lookup"><span data-stu-id="01ceb-153">If the **MessageDisposition** attribute is set to SendOnly, a created message will only be sent.</span></span> <span data-ttu-id="01ceb-154">[SavedItemFolderId](saveditemfolderid.md)要素で指定されたフォルダーにメッセージは送信されません。</span><span class="sxs-lookup"><span data-stu-id="01ceb-154">The message will not be put in the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="01ceb-155">Items (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="01ceb-155">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="01ceb-156">[SavedItemFolderId](saveditemfolderid.md)要素で指定されたフォルダーに作成する項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="01ceb-156">Contains an array of items to create in the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="01ceb-157">親要素</span><span class="sxs-lookup"><span data-stu-id="01ceb-157">Parent elements</span></span>

<span data-ttu-id="01ceb-158">なし。</span><span class="sxs-lookup"><span data-stu-id="01ceb-158">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="01ceb-159">注釈</span><span class="sxs-lookup"><span data-stu-id="01ceb-159">Remarks</span></span>

<span data-ttu-id="01ceb-160">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="01ceb-160">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="01ceb-161">要素情報</span><span class="sxs-lookup"><span data-stu-id="01ceb-161">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="01ceb-162">名前空間</span><span class="sxs-lookup"><span data-stu-id="01ceb-162">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="01ceb-163">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="01ceb-163">Schema Name</span></span>  <br/> |<span data-ttu-id="01ceb-164">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="01ceb-164">Messages schema</span></span>  <br/> |
|<span data-ttu-id="01ceb-165">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="01ceb-165">Validation File</span></span>  <br/> |<span data-ttu-id="01ceb-166">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="01ceb-166">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="01ceb-167">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="01ceb-167">Can be Empty</span></span>  <br/> |<span data-ttu-id="01ceb-168">False</span><span class="sxs-lookup"><span data-stu-id="01ceb-168">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="01ceb-169">関連項目</span><span class="sxs-lookup"><span data-stu-id="01ceb-169">See also</span></span>

- [<span data-ttu-id="01ceb-170">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="01ceb-170">CreateItemResponse</span></span>](createitemresponse.md)  
- <span data-ttu-id="01ceb-171">
  [CreateItem 操作](createitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="01ceb-171">[CreateItem operation](createitem-operation.md)</span></span>
- [<span data-ttu-id="01ceb-172">電子メール メッセージの作成</span><span class="sxs-lookup"><span data-stu-id="01ceb-172">Creating E-mail Messages</span></span>](http://msdn.microsoft.com/library/05bfb83c-2866-427d-a9fe-14ba3cb02793%28Office.15%29.aspx) 
- [<span data-ttu-id="01ceb-173">連絡先 (Exchange Web サービス) を作成します。</span><span class="sxs-lookup"><span data-stu-id="01ceb-173">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)  
- [<span data-ttu-id="01ceb-174">タスクを作成します。</span><span class="sxs-lookup"><span data-stu-id="01ceb-174">Creating Tasks</span></span>](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx) 
- [<span data-ttu-id="01ceb-175">予定の作成</span><span class="sxs-lookup"><span data-stu-id="01ceb-175">Creating Appointments</span></span>](http://msdn.microsoft.com/library/2385391e-c9e7-4d45-b803-c4ff94d5c94e%28Office.15%29.aspx)

