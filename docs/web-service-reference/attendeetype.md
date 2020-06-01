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
description: AttendeeType 要素は、Email (EmailAddressType) 要素で識別される出席者の種類を表します。 この要素は、会議提案の要求で使用されます。
ms.openlocfilehash: 104b9f38cc891310ecb47c0b47837a912ced6ab7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462298"
---
# <a name="attendeetype"></a><span data-ttu-id="16f77-104">AttendeeType</span><span class="sxs-lookup"><span data-stu-id="16f77-104">AttendeeType</span></span>

<span data-ttu-id="16f77-105">**AttendeeType**要素は、 [Email (emailaddresstype)](email-emailaddresstype.md)要素で識別される出席者の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="16f77-105">The **AttendeeType** element represents the type of attendee that is identified in the [Email (EmailAddressType)](email-emailaddresstype.md) element.</span></span> <span data-ttu-id="16f77-106">この要素は、会議提案の要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="16f77-106">This element is used in requests for meeting suggestions.</span></span> 
  
- [<span data-ttu-id="16f77-107">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="16f77-107">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
- [<span data-ttu-id="16f77-108">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="16f77-108">MailboxDataArray</span></span>](mailboxdataarray.md)
  
- [<span data-ttu-id="16f77-109">MailboxData</span><span class="sxs-lookup"><span data-stu-id="16f77-109">MailboxData</span></span>](mailboxdata.md)
  
- [<span data-ttu-id="16f77-110">AttendeeType</span><span class="sxs-lookup"><span data-stu-id="16f77-110">AttendeeType</span></span>](attendeetype.md)
  
```xml
<AttendeeType>Organizer or Required or Optional or Room or Resource</AttendeeType>
```

 <span data-ttu-id="16f77-111">**MeetingAttendeeType**</span><span class="sxs-lookup"><span data-stu-id="16f77-111">**MeetingAttendeeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="16f77-112">属性と要素</span><span class="sxs-lookup"><span data-stu-id="16f77-112">Attributes and elements</span></span>

<span data-ttu-id="16f77-113">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="16f77-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="16f77-114">属性</span><span class="sxs-lookup"><span data-stu-id="16f77-114">Attributes</span></span>

<span data-ttu-id="16f77-115">なし。</span><span class="sxs-lookup"><span data-stu-id="16f77-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="16f77-116">子要素</span><span class="sxs-lookup"><span data-stu-id="16f77-116">Child elements</span></span>

<span data-ttu-id="16f77-117">なし。</span><span class="sxs-lookup"><span data-stu-id="16f77-117">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="16f77-118">親要素</span><span class="sxs-lookup"><span data-stu-id="16f77-118">Parent elements</span></span>

|<span data-ttu-id="16f77-119">**要素**</span><span class="sxs-lookup"><span data-stu-id="16f77-119">**Element**</span></span>|<span data-ttu-id="16f77-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="16f77-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="16f77-121">MailboxData</span><span class="sxs-lookup"><span data-stu-id="16f77-121">MailboxData</span></span>](mailboxdata.md) <br/> |<span data-ttu-id="16f77-122">個々のメールボックスユーザー、およびメールボックスユーザーに関して返されるデータの種類のオプションを表します。</span><span class="sxs-lookup"><span data-stu-id="16f77-122">Represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span>  <br/> <span data-ttu-id="16f77-123">この要素の XPath を次に示します。</span><span class="sxs-lookup"><span data-stu-id="16f77-123">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]/MailboxData` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="16f77-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="16f77-124">Text value</span></span>

<span data-ttu-id="16f77-125">この要素にはテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="16f77-125">A text value is required for this element.</span></span> <span data-ttu-id="16f77-126">次の表に、この要素で使用できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="16f77-126">The following table lists the possible values for this element.</span></span>
  
|<span data-ttu-id="16f77-127">**値**</span><span class="sxs-lookup"><span data-stu-id="16f77-127">**Value**</span></span>|<span data-ttu-id="16f77-128">**説明**</span><span class="sxs-lookup"><span data-stu-id="16f77-128">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="16f77-129">開催者</span><span class="sxs-lookup"><span data-stu-id="16f77-129">Organizer</span></span>  <br/> |<span data-ttu-id="16f77-130">予定表アイテムを作成したメールボックスユーザーと出席者。</span><span class="sxs-lookup"><span data-stu-id="16f77-130">The mailbox user and attendee who created the calendar item.</span></span>  <br/> |
|<span data-ttu-id="16f77-131">必須</span><span class="sxs-lookup"><span data-stu-id="16f77-131">Required</span></span>  <br/> |<span data-ttu-id="16f77-132">会議の必須出席者であるメールボックスユーザー。</span><span class="sxs-lookup"><span data-stu-id="16f77-132">A mailbox user who is a required attendee to the meeting.</span></span>  <br/> |
|<span data-ttu-id="16f77-133">オプション</span><span class="sxs-lookup"><span data-stu-id="16f77-133">Optional</span></span>  <br/> |<span data-ttu-id="16f77-134">会議の任意出席者であるメールボックスユーザー。</span><span class="sxs-lookup"><span data-stu-id="16f77-134">A mailbox user who is an optional attendee to the meeting.</span></span>  <br/> |
|<span data-ttu-id="16f77-135">Room</span><span class="sxs-lookup"><span data-stu-id="16f77-135">Room</span></span>  <br/> |<span data-ttu-id="16f77-136">会議に使用される会議室リソースを表すメールボックスエンティティ。</span><span class="sxs-lookup"><span data-stu-id="16f77-136">A mailbox entity that represents a room resource used for the meeting.</span></span>  <br/> |
|<span data-ttu-id="16f77-137">関連情報</span><span class="sxs-lookup"><span data-stu-id="16f77-137">Resource</span></span>  <br/> |<span data-ttu-id="16f77-138">会議で使用するようにスケジュールされている、テレビやプロジェクターなどのリソース。</span><span class="sxs-lookup"><span data-stu-id="16f77-138">A resource such as a TV or projector that is scheduled for use in the meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="16f77-139">注釈</span><span class="sxs-lookup"><span data-stu-id="16f77-139">Remarks</span></span>

<span data-ttu-id="16f77-140">この要素は、 [MailboxData](mailboxdata.md)要素の必須の子要素です。</span><span class="sxs-lookup"><span data-stu-id="16f77-140">This element is a required child element of the [MailboxData](mailboxdata.md) element.</span></span> <span data-ttu-id="16f77-141">この要素は、 [MailboxData](mailboxdata.md)要素内で1回だけ発生します。</span><span class="sxs-lookup"><span data-stu-id="16f77-141">This element can only occur once in the [MailboxData](mailboxdata.md) element.</span></span> <span data-ttu-id="16f77-142">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの/EWS/ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="16f77-142">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="16f77-143">AttendeeType スキーマの種類は、予定表アイテムへの出席者を表すために使用されます。</span><span class="sxs-lookup"><span data-stu-id="16f77-143">The AttendeeType schema type is used to represent attendees to a calendar item.</span></span> <span data-ttu-id="16f77-144">この要素は、AttendeeType スキーマ型の要素と混同しないでください。</span><span class="sxs-lookup"><span data-stu-id="16f77-144">Do not confuse this element with elements of the AttendeeType schema type.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="16f77-145">要素の情報</span><span class="sxs-lookup"><span data-stu-id="16f77-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="16f77-146">Namespace</span><span class="sxs-lookup"><span data-stu-id="16f77-146">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="16f77-147">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="16f77-147">Schema Name</span></span>  <br/> |<span data-ttu-id="16f77-148">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="16f77-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="16f77-149">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="16f77-149">Validation File</span></span>  <br/> |<span data-ttu-id="16f77-150">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="16f77-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="16f77-151">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="16f77-151">Can be Empty</span></span>  <br/> |<span data-ttu-id="16f77-152">正しくない</span><span class="sxs-lookup"><span data-stu-id="16f77-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="16f77-153">関連項目</span><span class="sxs-lookup"><span data-stu-id="16f77-153">See also</span></span>

- [<span data-ttu-id="16f77-154">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="16f77-154">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="16f77-155">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="16f77-155">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="16f77-156">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="16f77-156">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

