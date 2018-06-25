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
description: MailboxData 要素は、個々 のメールボックス ユーザーとメールボックスのユーザーに返されるデータの種類のオプションを表します。
ms.openlocfilehash: df60294e7d83b1459e5cca7d75c2b6b4bb9d931d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832281"
---
# <a name="mailboxdata"></a><span data-ttu-id="90f7d-103">MailboxData</span><span class="sxs-lookup"><span data-stu-id="90f7d-103">MailboxData</span></span>

<span data-ttu-id="90f7d-104">**MailboxData**要素は、個々 のメールボックス ユーザーとメールボックスのユーザーに返されるデータの種類のオプションを表します。</span><span class="sxs-lookup"><span data-stu-id="90f7d-104">The **MailboxData** element represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span> 
  
- [<span data-ttu-id="90f7d-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="90f7d-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
- [<span data-ttu-id="90f7d-106">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="90f7d-106">MailboxDataArray</span></span>](mailboxdataarray.md)
  
- [<span data-ttu-id="90f7d-107">MailboxData</span><span class="sxs-lookup"><span data-stu-id="90f7d-107">MailboxData</span></span>](mailboxdata.md)
  
```xml
<MailboxData>
   <Email>...</Email>
   <AttendeeType>...</AttendeeType>
   <ExcludeConflicts>...</ExcludeConflicts>
<MailboxData>
```

<span data-ttu-id="90f7d-108">**MailboxData**</span><span class="sxs-lookup"><span data-stu-id="90f7d-108">**MailboxData**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="90f7d-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="90f7d-109">Attributes and elements</span></span>

<span data-ttu-id="90f7d-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="90f7d-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="90f7d-111">属性</span><span class="sxs-lookup"><span data-stu-id="90f7d-111">Attributes</span></span>

<span data-ttu-id="90f7d-112">なし。</span><span class="sxs-lookup"><span data-stu-id="90f7d-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="90f7d-113">子要素</span><span class="sxs-lookup"><span data-stu-id="90f7d-113">Child elements</span></span>

|<span data-ttu-id="90f7d-114">**要素**</span><span class="sxs-lookup"><span data-stu-id="90f7d-114">**Element**</span></span>|<span data-ttu-id="90f7d-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="90f7d-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="90f7d-116">電子メール (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="90f7d-116">Email (EmailAddressType)</span></span>](email-emailaddresstype.md) <br/> |<span data-ttu-id="90f7d-117">GetUserAvailability クエリのメールボックスのユーザーを表します。</span><span class="sxs-lookup"><span data-stu-id="90f7d-117">Represents the mailbox user for a GetUserAvailability query.</span></span>  <br/> |
|[<span data-ttu-id="90f7d-118">AttendeeType</span><span class="sxs-lookup"><span data-stu-id="90f7d-118">AttendeeType</span></span>](attendeetype.md) <br/> |<span data-ttu-id="90f7d-119">出席者の[電子メール (EmailAddressType)](email-emailaddresstype.md)の要素で特定の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="90f7d-119">Represents the type of attendee identified in the [Email (EmailAddressType)](email-emailaddresstype.md) element.</span></span> <span data-ttu-id="90f7d-120">会議の提案の要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="90f7d-120">This is used in requests for meeting suggestions.</span></span>  <br/> |
|[<span data-ttu-id="90f7d-121">ExcludeConflicts</span><span class="sxs-lookup"><span data-stu-id="90f7d-121">ExcludeConflicts</span></span>](excludeconflicts.md) <br/> |<span data-ttu-id="90f7d-122">候補を返すかどうかを指定、出席者の間で競合するカレンダーの時間の時間です。</span><span class="sxs-lookup"><span data-stu-id="90f7d-122">Specifies whether to return suggested times for calendar times that conflict among the attendees.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="90f7d-123">親要素</span><span class="sxs-lookup"><span data-stu-id="90f7d-123">Parent elements</span></span>

|<span data-ttu-id="90f7d-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="90f7d-124">**Element**</span></span>|<span data-ttu-id="90f7d-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="90f7d-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="90f7d-126">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="90f7d-126">MailboxDataArray</span></span>](mailboxdataarray.md) <br/> |<span data-ttu-id="90f7d-127">利用可能時間情報のクエリを実行するメールボックスの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="90f7d-127">Contains a list of mailboxes to query for availability information.</span></span>  <br/> <span data-ttu-id="90f7d-128">以下は、この要素の XPath です。</span><span class="sxs-lookup"><span data-stu-id="90f7d-128">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="90f7d-129">備考</span><span class="sxs-lookup"><span data-stu-id="90f7d-129">Remarks</span></span>

<span data-ttu-id="90f7d-130">クライアント アプリケーションは、多くの**MailboxData**要素を 1 つ定義できます。</span><span class="sxs-lookup"><span data-stu-id="90f7d-130">A client application can define one to many **MailboxData** elements.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="90f7d-131">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="90f7d-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="example"></a><span data-ttu-id="90f7d-132">例</span><span class="sxs-lookup"><span data-stu-id="90f7d-132">Example</span></span>

```xml
<MailboxDataArray>
  <MailboxData xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a><span data-ttu-id="90f7d-133">要素情報</span><span class="sxs-lookup"><span data-stu-id="90f7d-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="90f7d-134">名前空間</span><span class="sxs-lookup"><span data-stu-id="90f7d-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="90f7d-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="90f7d-135">Schema Name</span></span>  <br/> |<span data-ttu-id="90f7d-136">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="90f7d-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="90f7d-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="90f7d-137">Validation File</span></span>  <br/> |<span data-ttu-id="90f7d-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="90f7d-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="90f7d-139">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="90f7d-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="90f7d-140">False</span><span class="sxs-lookup"><span data-stu-id="90f7d-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="90f7d-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="90f7d-141">See also</span></span>

- [<span data-ttu-id="90f7d-142">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="90f7d-142">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="90f7d-143">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="90f7d-143">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="90f7d-144">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="90f7d-144">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

