---
title: AttendeeType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttendeeType
api_type:
- schema
ms.assetid: 048043a8-dbad-45a0-97c8-4cad63d8898b
description: AttendeeType 要素は、電子メール (EmailAddressType) の要素で指定されている参加者の種類を表します。 この要素は、推奨事項を満たすため、要求で使用されます。
ms.openlocfilehash: a08532ed78296102ee252c1e0c40beee7ca8ea5d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759462"
---
# <a name="attendeetype"></a><span data-ttu-id="98d1b-104">AttendeeType</span><span class="sxs-lookup"><span data-stu-id="98d1b-104">AttendeeType</span></span>

<span data-ttu-id="98d1b-105">**AttendeeType**要素は、[電子メール (EmailAddressType)](email-emailaddresstype.md)の要素で指定されている参加者の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="98d1b-105">The **AttendeeType** element represents the type of attendee that is identified in the [Email (EmailAddressType)](email-emailaddresstype.md) element.</span></span> <span data-ttu-id="98d1b-106">この要素は、推奨事項を満たすため、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="98d1b-106">This element is used in requests for meeting suggestions.</span></span> 
  
- [<span data-ttu-id="98d1b-107">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="98d1b-107">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
- [<span data-ttu-id="98d1b-108">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="98d1b-108">MailboxDataArray</span></span>](mailboxdataarray.md)
  
- [<span data-ttu-id="98d1b-109">MailboxData</span><span class="sxs-lookup"><span data-stu-id="98d1b-109">MailboxData</span></span>](mailboxdata.md)
  
- [<span data-ttu-id="98d1b-110">AttendeeType</span><span class="sxs-lookup"><span data-stu-id="98d1b-110">AttendeeType</span></span>](attendeetype.md)
  
```xml
<AttendeeType>Organizer or Required or Optional or Room or Resource</AttendeeType>
```

 <span data-ttu-id="98d1b-111">**MeetingAttendeeType**</span><span class="sxs-lookup"><span data-stu-id="98d1b-111">**MeetingAttendeeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="98d1b-112">属性および要素</span><span class="sxs-lookup"><span data-stu-id="98d1b-112">Attributes and elements</span></span>

<span data-ttu-id="98d1b-113">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="98d1b-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="98d1b-114">属性</span><span class="sxs-lookup"><span data-stu-id="98d1b-114">Attributes</span></span>

<span data-ttu-id="98d1b-115">なし。</span><span class="sxs-lookup"><span data-stu-id="98d1b-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="98d1b-116">子要素</span><span class="sxs-lookup"><span data-stu-id="98d1b-116">Child elements</span></span>

<span data-ttu-id="98d1b-117">なし。</span><span class="sxs-lookup"><span data-stu-id="98d1b-117">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="98d1b-118">親要素</span><span class="sxs-lookup"><span data-stu-id="98d1b-118">Parent elements</span></span>

|<span data-ttu-id="98d1b-119">**要素**</span><span class="sxs-lookup"><span data-stu-id="98d1b-119">**Element**</span></span>|<span data-ttu-id="98d1b-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="98d1b-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="98d1b-121">MailboxData</span><span class="sxs-lookup"><span data-stu-id="98d1b-121">MailboxData</span></span>](mailboxdata.md) <br/> |<span data-ttu-id="98d1b-122">個々 のメールボックス ユーザーのメールボックスのユーザーに返されるデータの種類のオプションを表します。</span><span class="sxs-lookup"><span data-stu-id="98d1b-122">Represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span>  <br/> <span data-ttu-id="98d1b-123">以下は、この要素の XPath です。</span><span class="sxs-lookup"><span data-stu-id="98d1b-123">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]/MailboxData` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="98d1b-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="98d1b-124">Text value</span></span>

<span data-ttu-id="98d1b-125">テキスト値は、この要素の必要があります。</span><span class="sxs-lookup"><span data-stu-id="98d1b-125">A text value is required for this element.</span></span> <span data-ttu-id="98d1b-126">次の表は、この要素の有効な値を一覧します。</span><span class="sxs-lookup"><span data-stu-id="98d1b-126">The following table lists the possible values for this element.</span></span>
  
|<span data-ttu-id="98d1b-127">**値**</span><span class="sxs-lookup"><span data-stu-id="98d1b-127">**Value**</span></span>|<span data-ttu-id="98d1b-128">**説明**</span><span class="sxs-lookup"><span data-stu-id="98d1b-128">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="98d1b-129">Organizer</span><span class="sxs-lookup"><span data-stu-id="98d1b-129">Organizer</span></span>  <br/> |<span data-ttu-id="98d1b-130">メールボックス ユーザーと出席者の予定表アイテムを作成しました。</span><span class="sxs-lookup"><span data-stu-id="98d1b-130">The mailbox user and attendee who created the calendar item.</span></span>  <br/> |
|<span data-ttu-id="98d1b-131">必須</span><span class="sxs-lookup"><span data-stu-id="98d1b-131">Required</span></span>  <br/> |<span data-ttu-id="98d1b-132">必須の出席者、会議には、メールボックス ・ ユーザーです。</span><span class="sxs-lookup"><span data-stu-id="98d1b-132">A mailbox user who is a required attendee to the meeting.</span></span>  <br/> |
|<span data-ttu-id="98d1b-133">省略可能</span><span class="sxs-lookup"><span data-stu-id="98d1b-133">Optional</span></span>  <br/> |<span data-ttu-id="98d1b-134">任意の出席者、会議には、メールボックス ・ ユーザーです。</span><span class="sxs-lookup"><span data-stu-id="98d1b-134">A mailbox user who is an optional attendee to the meeting.</span></span>  <br/> |
|<span data-ttu-id="98d1b-135">ルーム</span><span class="sxs-lookup"><span data-stu-id="98d1b-135">Room</span></span>  <br/> |<span data-ttu-id="98d1b-136">メールボックスを表すエンティティ部屋リソースが、会議に使用します。</span><span class="sxs-lookup"><span data-stu-id="98d1b-136">A mailbox entity that represents a room resource used for the meeting.</span></span>  <br/> |
|<span data-ttu-id="98d1b-137">リソース</span><span class="sxs-lookup"><span data-stu-id="98d1b-137">Resource</span></span>  <br/> |<span data-ttu-id="98d1b-138">テレビ会議で使用するためにスケジュールされている最初のプロジェクターなどのリソースです。</span><span class="sxs-lookup"><span data-stu-id="98d1b-138">A resource such as a TV or projector that is scheduled for use in the meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="98d1b-139">備考</span><span class="sxs-lookup"><span data-stu-id="98d1b-139">Remarks</span></span>

<span data-ttu-id="98d1b-140">この要素は、 [MailboxData](mailboxdata.md)要素の必須の子要素です。</span><span class="sxs-lookup"><span data-stu-id="98d1b-140">This element is a required child element of the [MailboxData](mailboxdata.md) element.</span></span> <span data-ttu-id="98d1b-141">この要素はことができます[MailboxData](mailboxdata.md)要素内で 1 回のみ発生します。</span><span class="sxs-lookup"><span data-stu-id="98d1b-141">This element can only occur once in the [MailboxData](mailboxdata.md) element.</span></span> <span data-ttu-id="98d1b-142">この要素を記述するスキーマは、インストールされているクライアント アクセス サーバーの役割を持つ MicrosoftExchange Server 2007 を実行しているコンピューターの/EWS/ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="98d1b-142">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="98d1b-143">AttendeeType スキーマの種類が使用され、出席者の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="98d1b-143">The AttendeeType schema type is used to represent attendees to a calendar item.</span></span> <span data-ttu-id="98d1b-144">AttendeeType スキーマの種類の要素にこの要素を混同しないでください。</span><span class="sxs-lookup"><span data-stu-id="98d1b-144">Do not confuse this element with elements of the AttendeeType schema type.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="98d1b-145">要素情報</span><span class="sxs-lookup"><span data-stu-id="98d1b-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="98d1b-146">名前空間</span><span class="sxs-lookup"><span data-stu-id="98d1b-146">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="98d1b-147">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="98d1b-147">Schema Name</span></span>  <br/> |<span data-ttu-id="98d1b-148">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="98d1b-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="98d1b-149">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="98d1b-149">Validation File</span></span>  <br/> |<span data-ttu-id="98d1b-150">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="98d1b-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="98d1b-151">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="98d1b-151">Can be Empty</span></span>  <br/> |<span data-ttu-id="98d1b-152">False</span><span class="sxs-lookup"><span data-stu-id="98d1b-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="98d1b-153">関連項目</span><span class="sxs-lookup"><span data-stu-id="98d1b-153">See also</span></span>

- [<span data-ttu-id="98d1b-154">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="98d1b-154">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="98d1b-155">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="98d1b-155">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="98d1b-156">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="98d1b-156">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

