---
title: MailboxData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailboxData
api_type:
- schema
ms.assetid: e9e3f50c-5a7b-49c7-a9ea-117959c08352
description: MailboxData 要素は、個々のメールボックスユーザー、およびメールボックスユーザーに関して返されるデータの種類のオプションを表します。
ms.openlocfilehash: bfcb8c01d40af81097c7d9868006fe9b7b5519d4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467250"
---
# <a name="mailboxdata"></a><span data-ttu-id="36083-103">MailboxData</span><span class="sxs-lookup"><span data-stu-id="36083-103">MailboxData</span></span>

<span data-ttu-id="36083-104">**MailboxData**要素は、個々のメールボックスユーザー、およびメールボックスユーザーに関して返されるデータの種類のオプションを表します。</span><span class="sxs-lookup"><span data-stu-id="36083-104">The **MailboxData** element represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span> 
  
- [<span data-ttu-id="36083-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="36083-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
- [<span data-ttu-id="36083-106">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="36083-106">MailboxDataArray</span></span>](mailboxdataarray.md)
  
- [<span data-ttu-id="36083-107">MailboxData</span><span class="sxs-lookup"><span data-stu-id="36083-107">MailboxData</span></span>](mailboxdata.md)
  
```xml
<MailboxData>
   <Email>...</Email>
   <AttendeeType>...</AttendeeType>
   <ExcludeConflicts>...</ExcludeConflicts>
<MailboxData>
```

<span data-ttu-id="36083-108">**MailboxData**</span><span class="sxs-lookup"><span data-stu-id="36083-108">**MailboxData**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="36083-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="36083-109">Attributes and elements</span></span>

<span data-ttu-id="36083-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="36083-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="36083-111">属性</span><span class="sxs-lookup"><span data-stu-id="36083-111">Attributes</span></span>

<span data-ttu-id="36083-112">なし。</span><span class="sxs-lookup"><span data-stu-id="36083-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="36083-113">子要素</span><span class="sxs-lookup"><span data-stu-id="36083-113">Child elements</span></span>

|<span data-ttu-id="36083-114">**Element**</span><span class="sxs-lookup"><span data-stu-id="36083-114">**Element**</span></span>|<span data-ttu-id="36083-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="36083-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="36083-116">電子メール (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="36083-116">Email (EmailAddressType)</span></span>](email-emailaddresstype.md) <br/> |<span data-ttu-id="36083-117">GetUserAvailability クエリのメールボックスユーザーを表します。</span><span class="sxs-lookup"><span data-stu-id="36083-117">Represents the mailbox user for a GetUserAvailability query.</span></span>  <br/> |
|[<span data-ttu-id="36083-118">AttendeeType</span><span class="sxs-lookup"><span data-stu-id="36083-118">AttendeeType</span></span>](attendeetype.md) <br/> |<span data-ttu-id="36083-119">[Email (EmailAddressType)](email-emailaddresstype.md)要素で識別された出席者の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="36083-119">Represents the type of attendee identified in the [Email (EmailAddressType)](email-emailaddresstype.md) element.</span></span> <span data-ttu-id="36083-120">これは、会議提案の要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="36083-120">This is used in requests for meeting suggestions.</span></span>  <br/> |
|[<span data-ttu-id="36083-121">ExcludeConflicts</span><span class="sxs-lookup"><span data-stu-id="36083-121">ExcludeConflicts</span></span>](excludeconflicts.md) <br/> |<span data-ttu-id="36083-122">出席者間での予定表の時間について、提案された時間を返すかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="36083-122">Specifies whether to return suggested times for calendar times that conflict among the attendees.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="36083-123">親要素</span><span class="sxs-lookup"><span data-stu-id="36083-123">Parent elements</span></span>

|<span data-ttu-id="36083-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="36083-124">**Element**</span></span>|<span data-ttu-id="36083-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="36083-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="36083-126">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="36083-126">MailboxDataArray</span></span>](mailboxdataarray.md) <br/> |<span data-ttu-id="36083-127">可用性情報を照会するメールボックスの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="36083-127">Contains a list of mailboxes to query for availability information.</span></span>  <br/> <span data-ttu-id="36083-128">この要素の XPath を次に示します。</span><span class="sxs-lookup"><span data-stu-id="36083-128">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="36083-129">注釈</span><span class="sxs-lookup"><span data-stu-id="36083-129">Remarks</span></span>

<span data-ttu-id="36083-130">クライアントアプリケーションでは、1対多の**MailboxData**要素を定義できます。</span><span class="sxs-lookup"><span data-stu-id="36083-130">A client application can define one to many **MailboxData** elements.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="36083-131">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="36083-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="example"></a><span data-ttu-id="36083-132">例</span><span class="sxs-lookup"><span data-stu-id="36083-132">Example</span></span>

```xml
<MailboxDataArray>
  <MailboxData xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
    <Email>
      <Name></Name>
      <Address>someone@ExServer.example.com</Address>
      <RoutingType>SMTP</RoutingType>
    </Email>
    <AttendeeType>Organizer</AttendeeType>
    <ExcludeConflicts>false</ExcludeConflicts>
  </MailboxData>
</MailboxDataArray>
```

## <a name="element-information"></a><span data-ttu-id="36083-133">要素の情報</span><span class="sxs-lookup"><span data-stu-id="36083-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="36083-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="36083-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="36083-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="36083-135">Schema Name</span></span>  <br/> |<span data-ttu-id="36083-136">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="36083-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="36083-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="36083-137">Validation File</span></span>  <br/> |<span data-ttu-id="36083-138">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="36083-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="36083-139">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="36083-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="36083-140">正しくない</span><span class="sxs-lookup"><span data-stu-id="36083-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="36083-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="36083-141">See also</span></span>

- [<span data-ttu-id="36083-142">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="36083-142">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="36083-143">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="36083-143">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="36083-144">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="36083-144">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

