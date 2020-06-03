---
title: CalendarView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarView
api_type:
- schema
ms.assetid: a4a953b8-0710-416c-95ef-59e51eba9982
description: CalendarView 要素は、カレンダーに表示されているように、セット内の予定表アイテムを返す FindItem 操作を定義します。
ms.openlocfilehash: e547a4b2db5c09ebefd9a072da6cc4733818002e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462263"
---
# <a name="calendarview"></a><span data-ttu-id="ecac2-103">CalendarView</span><span class="sxs-lookup"><span data-stu-id="ecac2-103">CalendarView</span></span>

<span data-ttu-id="ecac2-104">**CalendarView**要素は、カレンダーに表示されているように、セット内の予定表アイテムを返す[FindItem 操作](finditem-operation.md)を定義します。</span><span class="sxs-lookup"><span data-stu-id="ecac2-104">The **CalendarView** element defines a [FindItem operation](finditem-operation.md) as returning calendar items in a set as they appear in a calendar.</span></span> 
  
[<span data-ttu-id="ecac2-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="ecac2-105">FindItem</span></span>](finditem.md)
  
[<span data-ttu-id="ecac2-106">CalendarView</span><span class="sxs-lookup"><span data-stu-id="ecac2-106">CalendarView</span></span>](calendarview.md)
  
```XML
<CalendarView MaxEntriesReturned="" StartDate="" EndDate="" />
```

<span data-ttu-id="ecac2-107">**CalendarView**</span><span class="sxs-lookup"><span data-stu-id="ecac2-107">**CalendarView**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="ecac2-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="ecac2-108">Attributes and elements</span></span>

<span data-ttu-id="ecac2-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ecac2-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ecac2-110">属性</span><span class="sxs-lookup"><span data-stu-id="ecac2-110">Attributes</span></span>

|<span data-ttu-id="ecac2-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="ecac2-111">**Attribute**</span></span>|<span data-ttu-id="ecac2-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="ecac2-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ecac2-113">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="ecac2-113">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="ecac2-114">FindItem 応答で返される結果の最大数を表します。</span><span class="sxs-lookup"><span data-stu-id="ecac2-114">Describes the maximum number of results to return in the FindItem response.</span></span>  <br/> |
|<span data-ttu-id="ecac2-115">**StartDate**</span><span class="sxs-lookup"><span data-stu-id="ecac2-115">**StartDate**</span></span> <br/> |<span data-ttu-id="ecac2-116">予定表アイテムを照会する期間の開始日を識別します。</span><span class="sxs-lookup"><span data-stu-id="ecac2-116">Identifies the start of a time span queried for calendar items.</span></span> <span data-ttu-id="ecac2-117">終了時刻**が開始日より前**のすべての予定表アイテムは返されません。</span><span class="sxs-lookup"><span data-stu-id="ecac2-117">All calendar items that have an end time that is before **StartDate** will not be returned.</span></span> <span data-ttu-id="ecac2-118">**StartDate**の値は協定世界時 (UTC) 形式で指定できます。2006年-01-02T12:00: 00z、または現地時刻とタイムゾーンオフセットが指定されている形式 (2006-01-02T12:00:00-08:00) で指定できます。</span><span class="sxs-lookup"><span data-stu-id="ecac2-118">The value of **StartDate** can be specified in coordinated universal time (UTC) format, as in 2006-01-02T12:00:00Z, or in a format where local time and time zone offset is specified, as in 2006-01-02T04:00:00-08:00.</span></span>  <br/><br/><span data-ttu-id="ecac2-119">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="ecac2-119">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="ecac2-120">**EndDate**</span><span class="sxs-lookup"><span data-stu-id="ecac2-120">**EndDate**</span></span> <br/> |<span data-ttu-id="ecac2-121">予定表アイテムを照会した期間の終わりを識別します。</span><span class="sxs-lookup"><span data-stu-id="ecac2-121">Identifies the end of a time span queried for calendar items.</span></span> <span data-ttu-id="ecac2-122">開始時刻が終了日になっている予定表**アイテムは、** すべて返されません。</span><span class="sxs-lookup"><span data-stu-id="ecac2-122">All calendar items that have a start time that is on or after **EndDate** will not be returned.</span></span> <span data-ttu-id="ecac2-123">**EndDate**の値は、2006年-02-02T12:00: 00z のように UTC 形式で指定することができます。また、2006-02-02T12:00:00-08:00 のように、現地時刻とタイムゾーンオフセットが指定されている形式で指定することもできます。</span><span class="sxs-lookup"><span data-stu-id="ecac2-123">The value of **EndDate** can be specified in UTC format, as in 2006-02-02T12:00:00Z, or in a format where local time and time zone offset is specified, as in 2006-02-02T04:00:00-08:00.</span></span>  <br/><br/><span data-ttu-id="ecac2-124">**EndDate**は**StartDate**以上である必要があります。それ以外の場合は、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="ecac2-124">**EndDate** must be greater than or equal to **StartDate**; otherwise an error is returned.</span></span> <span data-ttu-id="ecac2-125">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="ecac2-125">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ecac2-126">子要素</span><span class="sxs-lookup"><span data-stu-id="ecac2-126">Child elements</span></span>

<span data-ttu-id="ecac2-127">なし。</span><span class="sxs-lookup"><span data-stu-id="ecac2-127">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ecac2-128">親要素</span><span class="sxs-lookup"><span data-stu-id="ecac2-128">Parent elements</span></span>

|<span data-ttu-id="ecac2-129">**要素**</span><span class="sxs-lookup"><span data-stu-id="ecac2-129">**Element**</span></span>|<span data-ttu-id="ecac2-130">**説明**</span><span class="sxs-lookup"><span data-stu-id="ecac2-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ecac2-131">FindItem</span><span class="sxs-lookup"><span data-stu-id="ecac2-131">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="ecac2-132">メールボックス内のアイテムを検索するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="ecac2-132">Defines a request to find items in a mailbox.</span></span><br/><br/> <span data-ttu-id="ecac2-133">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ecac2-133">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ecac2-134">注釈</span><span class="sxs-lookup"><span data-stu-id="ecac2-134">Remarks</span></span>

<span data-ttu-id="ecac2-135">**CalendarView**要素が FindItem 要求で指定されている場合、Web サービスは、開始**日と終了**日で指定**された**範囲内の予定表アイテムの1つおよび定期的なアイテムのリストを返します。</span><span class="sxs-lookup"><span data-stu-id="ecac2-135">If the **CalendarView** element is specified in a FindItem request, the Web service returns a list of single calendar items and occurrences of recurring calendar items within the range specified by **StartDate** and **EndDate**.</span></span>
  
<span data-ttu-id="ecac2-136">**CalendarView**要素が FindItem 要求で指定されていない場合、Web サービスは、1つの予定表アイテムと定期的なマスター予定表アイテムの一覧を返します。</span><span class="sxs-lookup"><span data-stu-id="ecac2-136">If the **CalendarView** element is not specified in a FindItem request, the Web service returns a list of single calendar items and recurring master calendar items.</span></span> <span data-ttu-id="ecac2-137">定期的な予定表アイテムの予定表アイテムは展開されません。</span><span class="sxs-lookup"><span data-stu-id="ecac2-137">Calendar occurrences of a recurring calendar item are not expanded.</span></span> 
  
<span data-ttu-id="ecac2-138">CalendarView クエリでは、より高速な予定表クエリがサポートされているため、次のプロパティのみを使用してください。</span><span class="sxs-lookup"><span data-stu-id="ecac2-138">CalendarView queries should only make use of the following properties since they support faster calendar queries.</span></span>
  
### <a name="recurrence-blob-properties"></a><span data-ttu-id="ecac2-139">定期的な blob プロパティ</span><span class="sxs-lookup"><span data-stu-id="ecac2-139">Recurrence blob properties</span></span>
  
- <span data-ttu-id="ecac2-140">MapiStartTime</span><span class="sxs-lookup"><span data-stu-id="ecac2-140">MapiStartTime</span></span>
    
- <span data-ttu-id="ecac2-141">MapiEndTime</span><span class="sxs-lookup"><span data-stu-id="ecac2-141">MapiEndTime</span></span>
    
- <span data-ttu-id="ecac2-142">SubjectPrefixInternal</span><span class="sxs-lookup"><span data-stu-id="ecac2-142">SubjectPrefixInternal</span></span>
    
- <span data-ttu-id="ecac2-143">NormalizedSubjectInternal</span><span class="sxs-lookup"><span data-stu-id="ecac2-143">NormalizedSubjectInternal</span></span>
    
- <span data-ttu-id="ecac2-144">MapiSubject</span><span class="sxs-lookup"><span data-stu-id="ecac2-144">MapiSubject</span></span>
    
- <span data-ttu-id="ecac2-145">場所</span><span class="sxs-lookup"><span data-stu-id="ecac2-145">Location</span></span>
    
- <span data-ttu-id="ecac2-146">AppointmentColor</span><span class="sxs-lookup"><span data-stu-id="ecac2-146">AppointmentColor</span></span>
    
- <span data-ttu-id="ecac2-147">MapiIsAllDayEvent</span><span class="sxs-lookup"><span data-stu-id="ecac2-147">MapiIsAllDayEvent</span></span>
    
- <span data-ttu-id="ecac2-148">MapiHasAttachment</span><span class="sxs-lookup"><span data-stu-id="ecac2-148">MapiHasAttachment</span></span>
    
- <span data-ttu-id="ecac2-149">FreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="ecac2-149">FreeBusyStatus</span></span>
    
- <span data-ttu-id="ecac2-150">ReminderIsSetInternal</span><span class="sxs-lookup"><span data-stu-id="ecac2-150">ReminderIsSetInternal</span></span>
    
- <span data-ttu-id="ecac2-151">ReminderMinutesBeforeStartInternal</span><span class="sxs-lookup"><span data-stu-id="ecac2-151">ReminderMinutesBeforeStartInternal</span></span>
    
- <span data-ttu-id="ecac2-152">AppointmentState</span><span class="sxs-lookup"><span data-stu-id="ecac2-152">AppointmentState</span></span>
    
- <span data-ttu-id="ecac2-153">AllAttachmentsHidden</span><span class="sxs-lookup"><span data-stu-id="ecac2-153">AllAttachmentsHidden</span></span>
    
- <span data-ttu-id="ecac2-154">ChangeHighlight 表示</span><span class="sxs-lookup"><span data-stu-id="ecac2-154">ChangeHighlight</span></span>
    
### <a name="calculated-from-the-primary-recurrence-blob-or-master"></a><span data-ttu-id="ecac2-155">主要な定期的なアイテムの blob またはマスターから計算されます。</span><span class="sxs-lookup"><span data-stu-id="ecac2-155">Calculated from the primary recurrence blob or master</span></span>
  
- <span data-ttu-id="ecac2-156">ItemId</span><span class="sxs-lookup"><span data-stu-id="ecac2-156">ItemId</span></span>
    
- <span data-ttu-id="ecac2-157">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="ecac2-157">IsRecurring</span></span>
    
- <span data-ttu-id="ecac2-158">IsException</span><span class="sxs-lookup"><span data-stu-id="ecac2-158">IsException</span></span>
    
- <span data-ttu-id="ecac2-159">AppointmentRecurring</span><span class="sxs-lookup"><span data-stu-id="ecac2-159">AppointmentRecurring</span></span>
    
- <span data-ttu-id="ecac2-160">MapiStartTime</span><span class="sxs-lookup"><span data-stu-id="ecac2-160">MapiStartTime</span></span>
    
- <span data-ttu-id="ecac2-161">MapiPRStartDate</span><span class="sxs-lookup"><span data-stu-id="ecac2-161">MapiPRStartDate</span></span>
    
- <span data-ttu-id="ecac2-162">MapiEndTime</span><span class="sxs-lookup"><span data-stu-id="ecac2-162">MapiEndTime</span></span>
    
- <span data-ttu-id="ecac2-163">MapiPREndDate</span><span class="sxs-lookup"><span data-stu-id="ecac2-163">MapiPREndDate</span></span>
    
- <span data-ttu-id="ecac2-164">CalendarItemType</span><span class="sxs-lookup"><span data-stu-id="ecac2-164">CalendarItemType</span></span>
    
- <span data-ttu-id="ecac2-165">GlobalObjectId</span><span class="sxs-lookup"><span data-stu-id="ecac2-165">GlobalObjectId</span></span>
    
- <span data-ttu-id="ecac2-166">TimeZoneDefinitionStart</span><span class="sxs-lookup"><span data-stu-id="ecac2-166">TimeZoneDefinitionStart</span></span>
    
- <span data-ttu-id="ecac2-167">TimeZoneDefinitionEnd</span><span class="sxs-lookup"><span data-stu-id="ecac2-167">TimeZoneDefinitionEnd</span></span>
    
### <a name="master-calendar-item-properties"></a><span data-ttu-id="ecac2-168">マスター予定表アイテムのプロパティ</span><span class="sxs-lookup"><span data-stu-id="ecac2-168">Master calendar item properties</span></span>
  
- <span data-ttu-id="ecac2-169">EntryId</span><span class="sxs-lookup"><span data-stu-id="ecac2-169">EntryId</span></span>
    
- <span data-ttu-id="ecac2-170">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="ecac2-170">ChangeKey</span></span>
    
- <span data-ttu-id="ecac2-171">ItemClass</span><span class="sxs-lookup"><span data-stu-id="ecac2-171">ItemClass</span></span>
    
- <span data-ttu-id="ecac2-172">SentRepresentingEmailAddress</span><span class="sxs-lookup"><span data-stu-id="ecac2-172">SentRepresentingEmailAddress</span></span>
    
- <span data-ttu-id="ecac2-173">[文] 表示 Displayname</span><span class="sxs-lookup"><span data-stu-id="ecac2-173">SentRepresentingDisplayName</span></span>
    
- <span data-ttu-id="ecac2-174">[文]</span><span class="sxs-lookup"><span data-stu-id="ecac2-174">SentRepresentingEntryId</span></span>
    
- <span data-ttu-id="ecac2-175">AppointmentRecurrenceBlob</span><span class="sxs-lookup"><span data-stu-id="ecac2-175">AppointmentRecurrenceBlob</span></span>
    
- <span data-ttu-id="ecac2-176">TimeZone</span><span class="sxs-lookup"><span data-stu-id="ecac2-176">TimeZone</span></span>
    
- <span data-ttu-id="ecac2-177">TimeZoneBlob</span><span class="sxs-lookup"><span data-stu-id="ecac2-177">TimeZoneBlob</span></span>
    
- <span data-ttu-id="ecac2-178">TimeZoneDefinitionRecurring</span><span class="sxs-lookup"><span data-stu-id="ecac2-178">TimeZoneDefinitionRecurring</span></span>
    
- <span data-ttu-id="ecac2-179">CleanGlobalObjectId</span><span class="sxs-lookup"><span data-stu-id="ecac2-179">CleanGlobalObjectId</span></span>
    
- <span data-ttu-id="ecac2-180">AppointmentRecurring</span><span class="sxs-lookup"><span data-stu-id="ecac2-180">AppointmentRecurring</span></span>
    
- <span data-ttu-id="ecac2-181">IsException</span><span class="sxs-lookup"><span data-stu-id="ecac2-181">IsException</span></span>
    
- <span data-ttu-id="ecac2-182">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="ecac2-182">IsRecurring</span></span>
    
- <span data-ttu-id="ecac2-183">MapiSensitivity</span><span class="sxs-lookup"><span data-stu-id="ecac2-183">MapiSensitivity</span></span>
    
- <span data-ttu-id="ecac2-184">ContainerClass</span><span class="sxs-lookup"><span data-stu-id="ecac2-184">ContainerClass</span></span>
    
- <span data-ttu-id="ecac2-185">MapiPRStartDate</span><span class="sxs-lookup"><span data-stu-id="ecac2-185">MapiPRStartDate</span></span>
    
- <span data-ttu-id="ecac2-186">MapiPREndDate</span><span class="sxs-lookup"><span data-stu-id="ecac2-186">MapiPREndDate</span></span>
    
- <span data-ttu-id="ecac2-187">カテゴリ</span><span class="sxs-lookup"><span data-stu-id="ecac2-187">Categories</span></span>
    
<span data-ttu-id="ecac2-188">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ecac2-188">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="ecac2-189">例</span><span class="sxs-lookup"><span data-stu-id="ecac2-189">Example</span></span>

<span data-ttu-id="ecac2-190">次の例は、FindItem 要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="ecac2-190">The following example shows a FindItem request.</span></span> <span data-ttu-id="ecac2-191">成功した要求は、2006年-05-18T00:00:00-08:00 または after and 終了された予定表アイテムを含む応答を返します。これは2006年から 05-19T00:00:00-08:00 です。</span><span class="sxs-lookup"><span data-stu-id="ecac2-191">A successful request returns a response that includes calendar items that started at 2006-05-18T00:00:00-08:00 or after and ended before 2006-05-19T00:00:00-08:00.</span></span>
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="calendar:Start"/>
          <t:FieldURI FieldURI="calendar:End"/>
          <t:FieldURI FieldURI="item:Subject"/>
        </t:AdditionalProperties>
      </ItemShape>
      <CalendarView MaxEntriesReturned="2" StartDate="2006-05-18T00:00:00-08:00" EndDate="2006-05-19T00:00:00-08:00"/>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="calendar"/>
      </ParentFolderIds>
    </FindItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="ecac2-192">要素の情報</span><span class="sxs-lookup"><span data-stu-id="ecac2-192">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ecac2-193">Namespace</span><span class="sxs-lookup"><span data-stu-id="ecac2-193">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ecac2-194">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ecac2-194">Schema Name</span></span>  <br/> |<span data-ttu-id="ecac2-195">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="ecac2-195">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ecac2-196">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ecac2-196">Validation File</span></span>  <br/> |<span data-ttu-id="ecac2-197">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="ecac2-197">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ecac2-198">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ecac2-198">Can be Empty</span></span>  <br/> |<span data-ttu-id="ecac2-199">正しくない</span><span class="sxs-lookup"><span data-stu-id="ecac2-199">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ecac2-200">関連項目</span><span class="sxs-lookup"><span data-stu-id="ecac2-200">See also</span></span>

- [<span data-ttu-id="ecac2-201">FindItem 操作</span><span class="sxs-lookup"><span data-stu-id="ecac2-201">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="ecac2-202">アイテムの検索</span><span class="sxs-lookup"><span data-stu-id="ecac2-202">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

