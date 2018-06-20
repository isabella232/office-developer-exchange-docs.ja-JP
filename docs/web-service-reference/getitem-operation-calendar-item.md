---
title: GetItem 操作 (予定表アイテム)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItem
api_type:
- schema
ms.assetid: a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8
description: GetItem 操作は、Exchange ストアから、予定表のアイテムを取得します。
ms.openlocfilehash: 69bce0f0cc7b5c986f9bf4767c3cd429a309e50d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760762"
---
# <a name="getitem-operation-calendar-item"></a><span data-ttu-id="14cfb-103">GetItem 操作 (予定表アイテム)</span><span class="sxs-lookup"><span data-stu-id="14cfb-103">GetItem operation (calendar item)</span></span>

<span data-ttu-id="14cfb-104">GetItem 操作は、Exchange ストアから、予定表のアイテムを取得します。</span><span class="sxs-lookup"><span data-stu-id="14cfb-104">The GetItem operation gets calendar items from the Exchange store.</span></span>
  
## <a name="getitem-request-example"></a><span data-ttu-id="14cfb-105">GetItem 要求の例</span><span class="sxs-lookup"><span data-stu-id="14cfb-105">GetItem request example</span></span>

### <a name="description"></a><span data-ttu-id="14cfb-106">説明</span><span class="sxs-lookup"><span data-stu-id="14cfb-106">Description</span></span>

<span data-ttu-id="14cfb-107">GetItem 要求の次の例では、id および項目の件名を取得する要求を作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="14cfb-107">The following example of a GetItem request shows how to form a request to get the identity and subject of an item.</span></span>
  
### <a name="code"></a><span data-ttu-id="14cfb-108">コード</span><span class="sxs-lookup"><span data-stu-id="14cfb-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject"/>
        </t:AdditionalProperties>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="AsdD89=" ChangeKey="Jajs3=="/>
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="14cfb-109">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="14cfb-109">Request elements</span></span>

<span data-ttu-id="14cfb-110">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="14cfb-110">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="14cfb-111">GetItem</span><span class="sxs-lookup"><span data-stu-id="14cfb-111">GetItem</span></span>](getitem.md)
    
- [<span data-ttu-id="14cfb-112">ItemShape</span><span class="sxs-lookup"><span data-stu-id="14cfb-112">ItemShape</span></span>](itemshape.md)
    
- [<span data-ttu-id="14cfb-113">BaseShape</span><span class="sxs-lookup"><span data-stu-id="14cfb-113">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="14cfb-114">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="14cfb-114">AdditionalProperties</span></span>](additionalproperties.md)
    
- [<span data-ttu-id="14cfb-115">FieldURI</span><span class="sxs-lookup"><span data-stu-id="14cfb-115">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="14cfb-116">Itemid</span><span class="sxs-lookup"><span data-stu-id="14cfb-116">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="14cfb-117">ItemId</span><span class="sxs-lookup"><span data-stu-id="14cfb-117">ItemId</span></span>](itemid.md)
    
> [!NOTE]
> <span data-ttu-id="14cfb-118">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="14cfb-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="14cfb-119">GetItem 操作の要求メッセージには、他のオプションを検索するには、スキーマの階層構造を表示します。</span><span class="sxs-lookup"><span data-stu-id="14cfb-119">To find other options for the request message of the GetItem operation, explore the schema hierarchy.</span></span> <span data-ttu-id="14cfb-120">[GetItem](getitem.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="14cfb-120">Start at the [GetItem](getitem.md) element.</span></span> 
  
## <a name="successful-getitem-response"></a><span data-ttu-id="14cfb-121">GetItem 応答の成功</span><span class="sxs-lookup"><span data-stu-id="14cfb-121">Successful GetItem Response</span></span>

### <a name="description"></a><span data-ttu-id="14cfb-122">説明</span><span class="sxs-lookup"><span data-stu-id="14cfb-122">Description</span></span>

<span data-ttu-id="14cfb-123">GetItem 要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="14cfb-123">The following example shows a successful response to the GetItem request.</span></span> <span data-ttu-id="14cfb-124">この応答を作成する要求は、IdOnly baseshape を使用します。</span><span class="sxs-lookup"><span data-stu-id="14cfb-124">The request that created this response used the IdOnly baseshape.</span></span> <span data-ttu-id="14cfb-125">この例では、応答は、アイテムの ID だけを返します。</span><span class="sxs-lookup"><span data-stu-id="14cfb-125">In this example, the response returns only the ID of the item.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="14cfb-126">品目 ID と変更キーは、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="14cfb-126">The item ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="14cfb-127">コード</span><span class="sxs-lookup"><span data-stu-id="14cfb-127">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                   xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                   xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="ASUAd" ChangeKey="otlIqB=="/>
            </t:CalendarItem>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </GetItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="description"></a><span data-ttu-id="14cfb-128">説明</span><span class="sxs-lookup"><span data-stu-id="14cfb-128">Description</span></span>

<span data-ttu-id="14cfb-129">GetItem 要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="14cfb-129">The following example shows a successful response to the GetItem request.</span></span> <span data-ttu-id="14cfb-130">この応答を作成する要求は、既定の baseshape を使用します。</span><span class="sxs-lookup"><span data-stu-id="14cfb-130">The request that created this response used the Default baseshape.</span></span> <span data-ttu-id="14cfb-131">この例では、応答は、予定表アイテムの既定の図形を返します。</span><span class="sxs-lookup"><span data-stu-id="14cfb-131">In this example, the response returns the Default shape for a calendar item.</span></span>
  
> [!NOTE]
> <span data-ttu-id="14cfb-132">品目 ID と変更キーは、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="14cfb-132">The item ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="14cfb-133">コード</span><span class="sxs-lookup"><span data-stu-id="14cfb-133">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                     xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                     xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="ASUAdTB" ChangeKey="otlIqBwrt=="/>
              <t:ResponseObjects>
                <t:ForwardItem/>
              </t:ResponseObjects>
              <t:Start>2006-06-16T00:30:00Z</t:Start>
              <t:End>2006-06-16T01:00:00Z</t:End>
              <t:LegacyFreeBusyStatus>Busy</t:LegacyFreeBusyStatus>
              <t:CalendarItemType>Single</t:CalendarItemType>
              <t:Organizer>
                <t:Mailbox>
                  <t:Name>Bob</t:Name>
                  <t:EmailAddress>someone@example.com</t:EmailAddress>
                  <t:RoutingType>SMTP</t:RoutingType>
                </t:Mailbox>
              </t:Organizer>
            </t:CalendarItem>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </GetItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="description"></a><span data-ttu-id="14cfb-134">説明</span><span class="sxs-lookup"><span data-stu-id="14cfb-134">Description</span></span>

<span data-ttu-id="14cfb-135">GetItem 要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="14cfb-135">The following example shows a successful response to the GetItem request.</span></span> <span data-ttu-id="14cfb-136">この応答を作成する要求は、AllProperties baseshape を使用します。</span><span class="sxs-lookup"><span data-stu-id="14cfb-136">The request that created this response used the AllProperties baseshape.</span></span> <span data-ttu-id="14cfb-137">この例では、応答は、予定表アイテムの [AllProperties] 図形を返します。</span><span class="sxs-lookup"><span data-stu-id="14cfb-137">In this example, the response returns the AllProperties shape for a calendar item.</span></span>
  
### <a name="code"></a><span data-ttu-id="14cfb-138">コード</span><span class="sxs-lookup"><span data-stu-id="14cfb-138">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                     xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                     xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="ASUAdT" ChangeKey="otlIqB=="/>
              <t:ParentFolderId Id="ASUAdT=="/>
              <t:ItemClass>IPM.Appointment</t:ItemClass>
              <t:Sensitivity>Normal</t:Sensitivity>
              <t:Body BodyType="Text"/>
              <t:DateTimeReceived>2006-06-16T00:12:41Z</t:DateTimeReceived>
              <t:Size>374</t:Size>
              <t:Importance>Normal</t:Importance>
              <t:IsSubmitted>false</t:IsSubmitted>
              <t:IsDraft>false</t:IsDraft>
              <t:IsFromMe>false</t:IsFromMe>
              <t:IsResend>false</t:IsResend>
              <t:IsUnmodified>false</t:IsUnmodified>
              <t:DateTimeSent>2006-06-16T00:12:41Z</t:DateTimeSent>
              <t:DateTimeCreated>2006-06-16T00:12:41Z</t:DateTimeCreated>
              <t:ResponseObjects>
                <t:ForwardItem/>
              </t:ResponseObjects>
              <t:ReminderDueBy>2006-06-16T00:30:00Z</t:ReminderDueBy>
              <t:ReminderIsSet>true</t:ReminderIsSet>
              <t:ReminderMinutesBeforeStart>15</t:ReminderMinutesBeforeStart>
              <t:DisplayCc/>
              <t:DisplayTo/>
              <t:HasAttachments>false</t:HasAttachments>
              <t:Culture>en-US</t:Culture>
              <t:Start>2006-06-16T00:30:00Z</t:Start>
              <t:End>2006-06-16T01:00:00Z</t:End>
              <t:IsAllDayEvent>false</t:IsAllDayEvent>
              <t:LegacyFreeBusyStatus>Busy</t:LegacyFreeBusyStatus>
              <t:IsMeeting>false</t:IsMeeting>
              <t:IsCancelled>false</t:IsCancelled>
              <t:IsRecurring>false</t:IsRecurring>
              <t:MeetingRequestWasSent>false</t:MeetingRequestWasSent>
              <t:CalendarItemType>Single</t:CalendarItemType>
              <t:MyResponseType>Organizer</t:MyResponseType>
              <t:Organizer>
                <t:Mailbox>
                  <t:Name>Bob</t:Name>
                  <t:EmailAddress>someone@example.com</t:EmailAddress>
                  <t:RoutingType>SMTP</t:RoutingType>
                </t:Mailbox>
              </t:Organizer>
              <t:ConflictingMeetingCount>2</t:ConflictingMeetingCount>
              <t:AdjacentMeetingCount>0</t:AdjacentMeetingCount>
              <t:ConflictingMeetings>
                <t:CalendarItem>
                  <t:ItemId Id="ASUAdTB" ChangeKey="otlIqBwr=="/>
                  <t:Subject/>
                  <t:Start>2006-06-16T00:30:00Z</t:Start>
                  <t:End>2006-06-16T01:00:00Z</t:End>
                  <t:LegacyFreeBusyStatus>Busy</t:LegacyFreeBusyStatus>
                  <t:Location/>
                </t:CalendarItem>
                <t:CalendarItem>
                  <t:ItemId Id="ASUAd" ChangeKey="otlIqBw=="/>
                  <t:Subject/>
                  <t:Start>2006-06-16T00:30:00Z</t:Start>
                  <t:End>2006-06-16T01:00:00Z</t:End>
                  <t:LegacyFreeBusyStatus>Busy</t:LegacyFreeBusyStatus>
                  <t:Location/>
                </t:CalendarItem>
              </t:ConflictingMeetings>
              <t:Duration>PT30M</t:Duration>
              <t:TimeZone>Pacific Standard Time</t:TimeZone>
              <t:AppointmentSequenceNumber>0</t:AppointmentSequenceNumber>
              <t:AppointmentState>0</t:AppointmentState>
            </t:CalendarItem>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </GetItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="14cfb-139">コメント</span><span class="sxs-lookup"><span data-stu-id="14cfb-139">Comments</span></span>

<span data-ttu-id="14cfb-140">GetItem 操作の応答メッセージには、他のオプションを検索するには、スキーマの階層構造を表示します。</span><span class="sxs-lookup"><span data-stu-id="14cfb-140">To find other options for the response message of the GetItem operation, explore the schema hierarchy.</span></span> <span data-ttu-id="14cfb-141">[GetItemResponse](getitemresponse.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="14cfb-141">Start at the [GetItemResponse](getitemresponse.md) element.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="14cfb-142">正常な応答の要素</span><span class="sxs-lookup"><span data-stu-id="14cfb-142">Successful response elements</span></span>

<span data-ttu-id="14cfb-143">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="14cfb-143">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="14cfb-144">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="14cfb-144">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="14cfb-145">GetItemResponse</span><span class="sxs-lookup"><span data-stu-id="14cfb-145">GetItemResponse</span></span>](getitemresponse.md)
    
- [<span data-ttu-id="14cfb-146">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="14cfb-146">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="14cfb-147">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="14cfb-147">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
    
- [<span data-ttu-id="14cfb-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="14cfb-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="14cfb-149">Items</span><span class="sxs-lookup"><span data-stu-id="14cfb-149">Items</span></span>](items.md)
    
- [<span data-ttu-id="14cfb-150">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="14cfb-150">CalendarItem</span></span>](calendaritem.md)
    
- [<span data-ttu-id="14cfb-151">ItemId</span><span class="sxs-lookup"><span data-stu-id="14cfb-151">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="14cfb-152">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="14cfb-152">ParentFolderId</span></span>](parentfolderid.md)
    
- [<span data-ttu-id="14cfb-153">ItemClass</span><span class="sxs-lookup"><span data-stu-id="14cfb-153">ItemClass</span></span>](itemclass.md)
    
- [<span data-ttu-id="14cfb-154">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="14cfb-154">Sensitivity</span></span>](sensitivity.md)
    
- [<span data-ttu-id="14cfb-155">Body/本文</span><span class="sxs-lookup"><span data-stu-id="14cfb-155">Body</span></span>](body.md)
    
- [<span data-ttu-id="14cfb-156">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="14cfb-156">DateTimeReceived</span></span>](datetimereceived.md)
    
- [<span data-ttu-id="14cfb-157">Size</span><span class="sxs-lookup"><span data-stu-id="14cfb-157">Size</span></span>](size.md)
    
- [<span data-ttu-id="14cfb-158">Importance</span><span class="sxs-lookup"><span data-stu-id="14cfb-158">Importance</span></span>](importance.md)
    
- [<span data-ttu-id="14cfb-159">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="14cfb-159">IsSubmitted</span></span>](issubmitted.md)
    
- [<span data-ttu-id="14cfb-160">IsDraft</span><span class="sxs-lookup"><span data-stu-id="14cfb-160">IsDraft</span></span>](isdraft.md)
    
- [<span data-ttu-id="14cfb-161">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="14cfb-161">IsFromMe</span></span>](isfromme.md)
    
- [<span data-ttu-id="14cfb-162">IsResend</span><span class="sxs-lookup"><span data-stu-id="14cfb-162">IsResend</span></span>](isresend.md)
    
- [<span data-ttu-id="14cfb-163">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="14cfb-163">IsUnmodified</span></span>](isunmodified.md)
    
- [<span data-ttu-id="14cfb-164">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="14cfb-164">DateTimeSent</span></span>](datetimesent.md)
    
- [<span data-ttu-id="14cfb-165">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="14cfb-165">DateTimeCreated</span></span>](datetimecreated.md)
    
- [<span data-ttu-id="14cfb-166">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="14cfb-166">ResponseObjects</span></span>](responseobjects.md)
    
- [<span data-ttu-id="14cfb-167">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="14cfb-167">ForwardItem</span></span>](forwarditem.md)
    
- [<span data-ttu-id="14cfb-168">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="14cfb-168">ReminderDueBy</span></span>](reminderdueby.md)
    
- [<span data-ttu-id="14cfb-169">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="14cfb-169">ReminderIsSet</span></span>](reminderisset.md)
    
- [<span data-ttu-id="14cfb-170">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="14cfb-170">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md)
    
- [<span data-ttu-id="14cfb-171">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="14cfb-171">DisplayCc</span></span>](displaycc.md)
    
- [<span data-ttu-id="14cfb-172">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="14cfb-172">DisplayTo</span></span>](displayto.md)
    
- [<span data-ttu-id="14cfb-173">添付ファイル付き</span><span class="sxs-lookup"><span data-stu-id="14cfb-173">HasAttachments</span></span>](hasattachments.md)
    
- [<span data-ttu-id="14cfb-174">カルチャ</span><span class="sxs-lookup"><span data-stu-id="14cfb-174">Culture</span></span>](culture.md)
    
- [<span data-ttu-id="14cfb-175">Start</span><span class="sxs-lookup"><span data-stu-id="14cfb-175">Start</span></span>](start.md)
    
- [<span data-ttu-id="14cfb-176">終わり</span><span class="sxs-lookup"><span data-stu-id="14cfb-176">End </span></span>](end-ex15websvcsotherref.md)
    
- [<span data-ttu-id="14cfb-177">IsAllDayEvent</span><span class="sxs-lookup"><span data-stu-id="14cfb-177">IsAllDayEvent</span></span>](isalldayevent.md)
    
- [<span data-ttu-id="14cfb-178">LegacyFreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="14cfb-178">LegacyFreeBusyStatus</span></span>](legacyfreebusystatus.md)
    
- [<span data-ttu-id="14cfb-179">IsMeeting</span><span class="sxs-lookup"><span data-stu-id="14cfb-179">IsMeeting</span></span>](ismeeting.md)
    
- [<span data-ttu-id="14cfb-180">IsCancelled</span><span class="sxs-lookup"><span data-stu-id="14cfb-180">IsCancelled</span></span>](iscancelled.md)
    
- [<span data-ttu-id="14cfb-181">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="14cfb-181">IsRecurring</span></span>](isrecurring.md)
    
- [<span data-ttu-id="14cfb-182">MeetingRequestWasSent</span><span class="sxs-lookup"><span data-stu-id="14cfb-182">MeetingRequestWasSent</span></span>](meetingrequestwassent.md)
    
- [<span data-ttu-id="14cfb-183">CalendarItemType</span><span class="sxs-lookup"><span data-stu-id="14cfb-183">CalendarItemType</span></span>](calendaritemtype.md)
    
- [<span data-ttu-id="14cfb-184">MyResponseType</span><span class="sxs-lookup"><span data-stu-id="14cfb-184">MyResponseType</span></span>](myresponsetype.md)
    
- [<span data-ttu-id="14cfb-185">Organizer</span><span class="sxs-lookup"><span data-stu-id="14cfb-185">Organizer</span></span>](organizer.md)
    
- [<span data-ttu-id="14cfb-186">メールボックス</span><span class="sxs-lookup"><span data-stu-id="14cfb-186">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="14cfb-187">名 (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="14cfb-187">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="14cfb-188">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="14cfb-188">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="14cfb-189">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="14cfb-189">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="14cfb-190">ConflictingMeetingCount</span><span class="sxs-lookup"><span data-stu-id="14cfb-190">ConflictingMeetingCount</span></span>](conflictingmeetingcount.md)
    
- [<span data-ttu-id="14cfb-191">AdjacentMeetingCount</span><span class="sxs-lookup"><span data-stu-id="14cfb-191">AdjacentMeetingCount</span></span>](adjacentmeetingcount.md)
    
- [<span data-ttu-id="14cfb-192">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="14cfb-192">ConflictingMeetings</span></span>](conflictingmeetings.md)
    
- [<span data-ttu-id="14cfb-193">場所</span><span class="sxs-lookup"><span data-stu-id="14cfb-193">Location</span></span>](location.md)
    
- [<span data-ttu-id="14cfb-194">期間 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="14cfb-194">Duration (Items)</span></span>](duration-items.md)
    
- [<span data-ttu-id="14cfb-195">タイムゾーン (アイテム)</span><span class="sxs-lookup"><span data-stu-id="14cfb-195">TimeZone (Item)</span></span>](timezone-item.md)
    
- [<span data-ttu-id="14cfb-196">AppointmentSequenceNumber</span><span class="sxs-lookup"><span data-stu-id="14cfb-196">AppointmentSequenceNumber</span></span>](appointmentsequencenumber.md)
    
- [<span data-ttu-id="14cfb-197">AppointmentState</span><span class="sxs-lookup"><span data-stu-id="14cfb-197">AppointmentState</span></span>](appointmentstate.md)
    
## <a name="see-also"></a><span data-ttu-id="14cfb-198">関連項目</span><span class="sxs-lookup"><span data-stu-id="14cfb-198">See also</span></span>



<span data-ttu-id="14cfb-199">
  [GetItem 操作](getitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="14cfb-199">[GetItem operation](getitem-operation.md)</span></span>

