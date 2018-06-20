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
description: 予定表ビューの要素は、カレンダーに表示される、一連の予定表のアイテムを返すよう FindItem 操作を定義します。
ms.openlocfilehash: 79b5ad268a8013092c1122c99bdcd10d876abf2c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759601"
---
# <a name="calendarview"></a><span data-ttu-id="981ca-103">CalendarView</span><span class="sxs-lookup"><span data-stu-id="981ca-103">CalendarView</span></span>

<span data-ttu-id="981ca-104">**予定表ビュー**の要素は、カレンダーに表示される、一連の予定表のアイテムを返すよう、 [FindItem 操作](finditem-operation.md)を定義します。</span><span class="sxs-lookup"><span data-stu-id="981ca-104">The **CalendarView** element defines a [FindItem operation](finditem-operation.md) as returning calendar items in a set as they appear in a calendar.</span></span> 
  
[<span data-ttu-id="981ca-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="981ca-105">FindItem</span></span>](finditem.md)
  
[<span data-ttu-id="981ca-106">予定表ビュー</span><span class="sxs-lookup"><span data-stu-id="981ca-106">CalendarView</span></span>](calendarview.md)
  
```XML
<CalendarView MaxEntriesReturned="" StartDate="" EndDate="" />
```

<span data-ttu-id="981ca-107">**予定表ビュー**</span><span class="sxs-lookup"><span data-stu-id="981ca-107">**CalendarView**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="981ca-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="981ca-108">Attributes and elements</span></span>

<span data-ttu-id="981ca-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="981ca-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="981ca-110">属性</span><span class="sxs-lookup"><span data-stu-id="981ca-110">Attributes</span></span>

|<span data-ttu-id="981ca-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="981ca-111">**Attribute**</span></span>|<span data-ttu-id="981ca-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="981ca-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="981ca-113">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="981ca-113">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="981ca-114">FindItem 応答で返す結果の最大数をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="981ca-114">Describes the maximum number of results to return in the FindItem response.</span></span>  <br/> |
|<span data-ttu-id="981ca-115">**開始日**</span><span class="sxs-lookup"><span data-stu-id="981ca-115">**StartDate**</span></span> <br/> |<span data-ttu-id="981ca-116">予定表アイテムに対してクエリを実行する期間の開始を識別します。</span><span class="sxs-lookup"><span data-stu-id="981ca-116">Identifies the start of a time span queried for calendar items.</span></span> <span data-ttu-id="981ca-117">終了時刻は**開始日**は返されません。 前にあるすべての予定表アイテム。</span><span class="sxs-lookup"><span data-stu-id="981ca-117">All calendar items that have an end time that is before **StartDate** will not be returned.</span></span> <span data-ttu-id="981ca-118">2006 のように、世界協定時刻 (UTC) 形式で**開始日**の値を指定することができます-01-02T12:00:00Z、2006年のように、ローカル時刻とタイム ゾーンのオフセットが指定されている形式で、または -01-02T04:00:00-08時 00分です。</span><span class="sxs-lookup"><span data-stu-id="981ca-118">The value of **StartDate** can be specified in coordinated universal time (UTC) format, as in 2006-01-02T12:00:00Z, or in a format where local time and time zone offset is specified, as in 2006-01-02T04:00:00-08:00.</span></span>  <br/><br/><span data-ttu-id="981ca-119">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="981ca-119">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="981ca-120">**終了日**</span><span class="sxs-lookup"><span data-stu-id="981ca-120">**EndDate**</span></span> <br/> |<span data-ttu-id="981ca-121">予定表アイテムに対してクエリを実行時間の範囲の末尾を識別します。</span><span class="sxs-lookup"><span data-stu-id="981ca-121">Identifies the end of a time span queried for calendar items.</span></span> <span data-ttu-id="981ca-122">開始時刻または**終了日**の後にあるすべての予定表アイテムは返されません。</span><span class="sxs-lookup"><span data-stu-id="981ca-122">All calendar items that have a start time that is on or after **EndDate** will not be returned.</span></span> <span data-ttu-id="981ca-123">2006 のように、UTC 形式で**終了日**の値を指定することができます-02-02T12:00:00Z、2006年のように、ローカル時刻とタイム ゾーンのオフセットが指定されている形式で、または -02-02T04:00:00-08時 00分です。</span><span class="sxs-lookup"><span data-stu-id="981ca-123">The value of **EndDate** can be specified in UTC format, as in 2006-02-02T12:00:00Z, or in a format where local time and time zone offset is specified, as in 2006-02-02T04:00:00-08:00.</span></span>  <br/><br/><span data-ttu-id="981ca-124">**終了日**が**開始日**は以上にする必要があります。それ以外の場合、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="981ca-124">**EndDate** must be greater than or equal to **StartDate**; otherwise an error is returned.</span></span> <span data-ttu-id="981ca-125">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="981ca-125">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="981ca-126">子要素</span><span class="sxs-lookup"><span data-stu-id="981ca-126">Child elements</span></span>

<span data-ttu-id="981ca-127">なし。</span><span class="sxs-lookup"><span data-stu-id="981ca-127">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="981ca-128">親要素</span><span class="sxs-lookup"><span data-stu-id="981ca-128">Parent elements</span></span>

|<span data-ttu-id="981ca-129">**要素**</span><span class="sxs-lookup"><span data-stu-id="981ca-129">**Element**</span></span>|<span data-ttu-id="981ca-130">**説明**</span><span class="sxs-lookup"><span data-stu-id="981ca-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="981ca-131">FindItem</span><span class="sxs-lookup"><span data-stu-id="981ca-131">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="981ca-132">メールボックス内のアイテムを検索するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="981ca-132">Defines a request to find items in a mailbox.</span></span><br/><br/> <span data-ttu-id="981ca-133">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="981ca-133">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="981ca-134">備考</span><span class="sxs-lookup"><span data-stu-id="981ca-134">Remarks</span></span>

<span data-ttu-id="981ca-135">FindItem 要求で、**予定表ビュー**の要素を指定すると、Web サービスは、1 つの予定表アイテムと出現する**開始日**と**終了日**に指定した範囲内での定期的な予定表アイテムの一覧を返します。</span><span class="sxs-lookup"><span data-stu-id="981ca-135">If the **CalendarView** element is specified in a FindItem request, the Web service returns a list of single calendar items and occurrences of recurring calendar items within the range specified by **StartDate** and **EndDate**.</span></span>
  
<span data-ttu-id="981ca-136">FindItem 要求で、**予定表ビュー**の要素を指定しない場合、Web サービスは、1 つの予定表アイテムと定期的なマスターの予定表アイテムの一覧を返します。</span><span class="sxs-lookup"><span data-stu-id="981ca-136">If the **CalendarView** element is not specified in a FindItem request, the Web service returns a list of single calendar items and recurring master calendar items.</span></span> <span data-ttu-id="981ca-137">定期的な予定表アイテムの予定表アイテムは展開されません。</span><span class="sxs-lookup"><span data-stu-id="981ca-137">Calendar occurrences of a recurring calendar item are not expanded.</span></span> 
  
<span data-ttu-id="981ca-138">予定表ビューのクエリを作成する必要がありますのみ予定表クエリを高速化をサポートするために次のプロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="981ca-138">CalendarView queries should only make use of the following properties since they support faster calendar queries.</span></span>
  
### <a name="recurrence-blob-properties"></a><span data-ttu-id="981ca-139">定期的なアイテムの blob のプロパティ</span><span class="sxs-lookup"><span data-stu-id="981ca-139">Recurrence blob properties</span></span>
  
- <span data-ttu-id="981ca-140">MapiStartTime</span><span class="sxs-lookup"><span data-stu-id="981ca-140">MapiStartTime</span></span>
    
- <span data-ttu-id="981ca-141">MapiEndTime</span><span class="sxs-lookup"><span data-stu-id="981ca-141">MapiEndTime</span></span>
    
- <span data-ttu-id="981ca-142">SubjectPrefixInternal</span><span class="sxs-lookup"><span data-stu-id="981ca-142">SubjectPrefixInternal</span></span>
    
- <span data-ttu-id="981ca-143">NormalizedSubjectInternal</span><span class="sxs-lookup"><span data-stu-id="981ca-143">NormalizedSubjectInternal</span></span>
    
- <span data-ttu-id="981ca-144">MapiSubject</span><span class="sxs-lookup"><span data-stu-id="981ca-144">MapiSubject</span></span>
    
- <span data-ttu-id="981ca-145">場所</span><span class="sxs-lookup"><span data-stu-id="981ca-145">Location</span></span>
    
- <span data-ttu-id="981ca-146">AppointmentColor</span><span class="sxs-lookup"><span data-stu-id="981ca-146">AppointmentColor</span></span>
    
- <span data-ttu-id="981ca-147">MapiIsAllDayEvent</span><span class="sxs-lookup"><span data-stu-id="981ca-147">MapiIsAllDayEvent</span></span>
    
- <span data-ttu-id="981ca-148">MapiHasAttachment</span><span class="sxs-lookup"><span data-stu-id="981ca-148">MapiHasAttachment</span></span>
    
- <span data-ttu-id="981ca-149">FreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="981ca-149">FreeBusyStatus</span></span>
    
- <span data-ttu-id="981ca-150">ReminderIsSetInternal</span><span class="sxs-lookup"><span data-stu-id="981ca-150">ReminderIsSetInternal</span></span>
    
- <span data-ttu-id="981ca-151">ReminderMinutesBeforeStartInternal</span><span class="sxs-lookup"><span data-stu-id="981ca-151">ReminderMinutesBeforeStartInternal</span></span>
    
- <span data-ttu-id="981ca-152">AppointmentState</span><span class="sxs-lookup"><span data-stu-id="981ca-152">AppointmentState</span></span>
    
- <span data-ttu-id="981ca-153">AllAttachmentsHidden</span><span class="sxs-lookup"><span data-stu-id="981ca-153">AllAttachmentsHidden</span></span>
    
- <span data-ttu-id="981ca-154">ChangeHighlight</span><span class="sxs-lookup"><span data-stu-id="981ca-154">ChangeHighlight</span></span>
    
### <a name="calculated-from-the-primary-recurrence-blob-or-master"></a><span data-ttu-id="981ca-155">主なパターン blob またはマスターからの計算</span><span class="sxs-lookup"><span data-stu-id="981ca-155">Calculated from the primary recurrence blob or master</span></span>
  
- <span data-ttu-id="981ca-156">ItemId</span><span class="sxs-lookup"><span data-stu-id="981ca-156">ItemId</span></span>
    
- <span data-ttu-id="981ca-157">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="981ca-157">IsRecurring</span></span>
    
- <span data-ttu-id="981ca-158">IsException</span><span class="sxs-lookup"><span data-stu-id="981ca-158">IsException</span></span>
    
- <span data-ttu-id="981ca-159">AppointmentRecurring</span><span class="sxs-lookup"><span data-stu-id="981ca-159">AppointmentRecurring</span></span>
    
- <span data-ttu-id="981ca-160">MapiStartTime</span><span class="sxs-lookup"><span data-stu-id="981ca-160">MapiStartTime</span></span>
    
- <span data-ttu-id="981ca-161">MapiPRStartDate</span><span class="sxs-lookup"><span data-stu-id="981ca-161">MapiPRStartDate</span></span>
    
- <span data-ttu-id="981ca-162">MapiEndTime</span><span class="sxs-lookup"><span data-stu-id="981ca-162">MapiEndTime</span></span>
    
- <span data-ttu-id="981ca-163">MapiPREndDate</span><span class="sxs-lookup"><span data-stu-id="981ca-163">MapiPREndDate</span></span>
    
- <span data-ttu-id="981ca-164">CalendarItemType</span><span class="sxs-lookup"><span data-stu-id="981ca-164">CalendarItemType</span></span>
    
- <span data-ttu-id="981ca-165">GlobalObjectId</span><span class="sxs-lookup"><span data-stu-id="981ca-165">GlobalObjectId</span></span>
    
- <span data-ttu-id="981ca-166">TimeZoneDefinitionStart</span><span class="sxs-lookup"><span data-stu-id="981ca-166">TimeZoneDefinitionStart</span></span>
    
- <span data-ttu-id="981ca-167">TimeZoneDefinitionEnd</span><span class="sxs-lookup"><span data-stu-id="981ca-167">TimeZoneDefinitionEnd</span></span>
    
### <a name="master-calendar-item-properties"></a><span data-ttu-id="981ca-168">マスターの予定表アイテムのプロパティ</span><span class="sxs-lookup"><span data-stu-id="981ca-168">Master calendar item properties</span></span>
  
- <span data-ttu-id="981ca-169">EntryId</span><span class="sxs-lookup"><span data-stu-id="981ca-169">EntryId</span></span>
    
- <span data-ttu-id="981ca-170">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="981ca-170">ChangeKey</span></span>
    
- <span data-ttu-id="981ca-171">ItemClass</span><span class="sxs-lookup"><span data-stu-id="981ca-171">ItemClass</span></span>
    
- <span data-ttu-id="981ca-172">SentRepresentingEmailAddress</span><span class="sxs-lookup"><span data-stu-id="981ca-172">SentRepresentingEmailAddress</span></span>
    
- <span data-ttu-id="981ca-173">SentRepresentingDisplayName</span><span class="sxs-lookup"><span data-stu-id="981ca-173">SentRepresentingDisplayName</span></span>
    
- <span data-ttu-id="981ca-174">SentRepresentingEntryId</span><span class="sxs-lookup"><span data-stu-id="981ca-174">SentRepresentingEntryId</span></span>
    
- <span data-ttu-id="981ca-175">AppointmentRecurrenceBlob</span><span class="sxs-lookup"><span data-stu-id="981ca-175">AppointmentRecurrenceBlob</span></span>
    
- <span data-ttu-id="981ca-176">TimeZone</span><span class="sxs-lookup"><span data-stu-id="981ca-176">TimeZone</span></span>
    
- <span data-ttu-id="981ca-177">TimeZoneBlob</span><span class="sxs-lookup"><span data-stu-id="981ca-177">TimeZoneBlob</span></span>
    
- <span data-ttu-id="981ca-178">TimeZoneDefinitionRecurring</span><span class="sxs-lookup"><span data-stu-id="981ca-178">TimeZoneDefinitionRecurring</span></span>
    
- <span data-ttu-id="981ca-179">CleanGlobalObjectId</span><span class="sxs-lookup"><span data-stu-id="981ca-179">CleanGlobalObjectId</span></span>
    
- <span data-ttu-id="981ca-180">AppointmentRecurring</span><span class="sxs-lookup"><span data-stu-id="981ca-180">AppointmentRecurring</span></span>
    
- <span data-ttu-id="981ca-181">IsException</span><span class="sxs-lookup"><span data-stu-id="981ca-181">IsException</span></span>
    
- <span data-ttu-id="981ca-182">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="981ca-182">IsRecurring</span></span>
    
- <span data-ttu-id="981ca-183">MapiSensitivity</span><span class="sxs-lookup"><span data-stu-id="981ca-183">MapiSensitivity</span></span>
    
- <span data-ttu-id="981ca-184">ContainerClass</span><span class="sxs-lookup"><span data-stu-id="981ca-184">ContainerClass</span></span>
    
- <span data-ttu-id="981ca-185">MapiPRStartDate</span><span class="sxs-lookup"><span data-stu-id="981ca-185">MapiPRStartDate</span></span>
    
- <span data-ttu-id="981ca-186">MapiPREndDate</span><span class="sxs-lookup"><span data-stu-id="981ca-186">MapiPREndDate</span></span>
    
- <span data-ttu-id="981ca-187">カテゴリ</span><span class="sxs-lookup"><span data-stu-id="981ca-187">Categories</span></span>
    
<span data-ttu-id="981ca-188">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="981ca-188">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="981ca-189">例</span><span class="sxs-lookup"><span data-stu-id="981ca-189">Example</span></span>

<span data-ttu-id="981ca-190">FindItem 要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="981ca-190">The following example shows a FindItem request.</span></span> <span data-ttu-id="981ca-191">要求が成功するには、2006年で開始される予定表アイテムを含む応答が返されます-05-18T00:00:00-08時 00分後、2006 年以前に終了したのか -05-19T00:00:00-08時 00分です。</span><span class="sxs-lookup"><span data-stu-id="981ca-191">A successful request returns a response that includes calendar items that started at 2006-05-18T00:00:00-08:00 or after and ended before 2006-05-19T00:00:00-08:00.</span></span>
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="element-information"></a><span data-ttu-id="981ca-192">要素情報</span><span class="sxs-lookup"><span data-stu-id="981ca-192">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="981ca-193">名前空間</span><span class="sxs-lookup"><span data-stu-id="981ca-193">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="981ca-194">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="981ca-194">Schema Name</span></span>  <br/> |<span data-ttu-id="981ca-195">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="981ca-195">Messages schema</span></span>  <br/> |
|<span data-ttu-id="981ca-196">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="981ca-196">Validation File</span></span>  <br/> |<span data-ttu-id="981ca-197">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="981ca-197">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="981ca-198">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="981ca-198">Can be Empty</span></span>  <br/> |<span data-ttu-id="981ca-199">False</span><span class="sxs-lookup"><span data-stu-id="981ca-199">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="981ca-200">関連項目</span><span class="sxs-lookup"><span data-stu-id="981ca-200">See also</span></span>

- <span data-ttu-id="981ca-201">
  [FindItem 操作](finditem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="981ca-201">[FindItem operation](finditem-operation.md)</span></span>
- [<span data-ttu-id="981ca-202">項目を検索します。</span><span class="sxs-lookup"><span data-stu-id="981ca-202">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

