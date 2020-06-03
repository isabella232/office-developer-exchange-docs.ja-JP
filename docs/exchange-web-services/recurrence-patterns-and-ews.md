---
title: 定期的なパターンと EWS
manager: luken
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: fd9ef706-1e01-49fa-af6f-2f6d3e173c16
description: Exchange の定期的なパターンと定期的なアイテムについて説明します。
ms.openlocfilehash: 681dfee7e0a66a483b8638810da5e4e0ac0f05ac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459329"
---
# <a name="recurrence-patterns-and-ews"></a><span data-ttu-id="c3cb4-103">定期的なパターンと EWS</span><span class="sxs-lookup"><span data-stu-id="c3cb4-103">Recurrence patterns and EWS</span></span>

<span data-ttu-id="c3cb4-104">Exchange の定期的なパターンと定期的なアイテムについて説明します。</span><span class="sxs-lookup"><span data-stu-id="c3cb4-104">Learn about recurrence patterns and recurring series in Exchange.</span></span>
  
<span data-ttu-id="c3cb4-p101">定期的なアイテムは、定義済みのパターンに従って繰り返す予定または会議です。定期的なアイテムは、特定のアイテム数にすることも、無制限で繰り返すこともできます。さらに、定期的なアイテムには、アイテムの残りのパターンに従わない例外もあります。また、パターンから削除されたアイテムを持つこともできます。EWS マネージ API と EWS を使用すると、定期的なアイテムと、それらの関連付けられた予定表アイテムを操作できます。</span><span class="sxs-lookup"><span data-stu-id="c3cb4-p101">A recurring series is an appointment or meeting that repeats according to a defined pattern. A recurring series can either have a specific number of occurrences or can repeat indefinitely. Additionally, a recurring series can have exceptions that don't follow the pattern of the rest of the occurrences, and can have occurrences that have been deleted from the pattern. You can use the EWS Managed API and EWS to work with recurring series and their associated calendar items.</span></span>
  
## <a name="recurring-calendar-items"></a><span data-ttu-id="c3cb4-109">定期的な予定表アイテム</span><span class="sxs-lookup"><span data-stu-id="c3cb4-109">Recurring calendar items</span></span>

<span data-ttu-id="c3cb4-110">すべての予定表アイテムは、次に示す 4 つのカテゴリのいずれか 1 つに分類されます。</span><span class="sxs-lookup"><span data-stu-id="c3cb4-110">All calendar items fall into one of the following four categories:</span></span>
  
- <span data-ttu-id="c3cb4-111">非定期的な予定表アイテム</span><span class="sxs-lookup"><span data-stu-id="c3cb4-111">Non-recurring calendar items</span></span>
    
- <span data-ttu-id="c3cb4-112">定期的マスター</span><span class="sxs-lookup"><span data-stu-id="c3cb4-112">Recurring masters</span></span>
    
- <span data-ttu-id="c3cb4-113">定期的なアイテム内のアイテム</span><span class="sxs-lookup"><span data-stu-id="c3cb4-113">Occurrences in a series</span></span>
    
- <span data-ttu-id="c3cb4-114">定期的なアイテム内の変更されたアイテム (例外)</span><span class="sxs-lookup"><span data-stu-id="c3cb4-114">Modified occurrences in a series, known as exceptions</span></span>
    
<span data-ttu-id="c3cb4-115">この記事では、定期的なアイテムの一部である予定表アイテムの 3 つの種類について説明します。</span><span class="sxs-lookup"><span data-stu-id="c3cb4-115">In this article, we'll look at the three types of calendar items that are part of a recurring series.</span></span>
  
<span data-ttu-id="c3cb4-p102">これは、定期的なアイテム を Exchange Server 上に実装する方法を理解するために役立ちます。定期的なアイテム内の各アイテムに、個別に異なるアイテムを作成するかわりに、サーバーは予定表で、定期的マスターと呼ばれる実際のアイテムを 1 つだけ作成します。定期的マスターの書式は非定期的な予定とよく似ていますが、定期的なパターンの情報が追加されています。サーバーは予定の情報に関するクライアントの要求に応じて、定期的なパターンを基に展開と呼ばれるプロセスを使用してアイテムを生成します。これらの生成されたアイテムは、永続的にサーバーで保存されるわけではありません。これを理解することは重要です。予定表アイテムを検索する方法が、受け取る情報と、展開を行うかどうかを決定するからです。</span><span class="sxs-lookup"><span data-stu-id="c3cb4-p102">It's helpful to understand how recurring series are implemented on the Exchange server. Instead of creating a separate distinct item for each occurrence in a recurring series, the server creates only one actual item in the calendar, known as the recurring master. The format of a recurring master is very similar to a non-recurring appointment, with the addition of recurrence pattern information. The server then generates occurrences based on the recurrence pattern in response to client requests for appointment information, using a process called expansion. These generated occurrences are not permanently stored on the server. This is important to understand because the way that you search for calendar items determines what information you receive and whether expansion occurs.</span></span>
  
## <a name="recurrence-patterns"></a><span data-ttu-id="c3cb4-122">定期的なパターン</span><span class="sxs-lookup"><span data-stu-id="c3cb4-122">Recurrence patterns</span></span>

<span data-ttu-id="c3cb4-p103">展開を可能にする重要な定期的なアイテムは、定期的なパターンです。定期的なパターンは、定期的マスターにあります。定期的なパターンは、定期的マスターの日付および時間に基づいたアイテムの計算に関する条件のセットを記述します。</span><span class="sxs-lookup"><span data-stu-id="c3cb4-p103">The key piece to a recurring series that makes expansion possible is the recurrence pattern. The recurrence pattern is found on the recurring master, and describes a set of criteria for calculating occurrences based on the date and time of the recurring master.</span></span>
  
<span data-ttu-id="c3cb4-125">**表 1. 使用可能な定期的なパターン**</span><span class="sxs-lookup"><span data-stu-id="c3cb4-125">**Table 1. Available recurrence patterns**</span></span>

|<span data-ttu-id="c3cb4-126">**EWS マネージ API のクラス**</span><span class="sxs-lookup"><span data-stu-id="c3cb4-126">**EWS Managed API class**</span></span>|<span data-ttu-id="c3cb4-127">**EWS の要素**</span><span class="sxs-lookup"><span data-stu-id="c3cb4-127">**EWS element**</span></span>|<span data-ttu-id="c3cb4-128">**例**</span><span class="sxs-lookup"><span data-stu-id="c3cb4-128">**Examples**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="c3cb4-129">Recurrence.DailyPattern</span><span class="sxs-lookup"><span data-stu-id="c3cb4-129">Recurrence.DailyPattern</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.dailypattern%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="c3cb4-130">DailyRecurrence</span><span class="sxs-lookup"><span data-stu-id="c3cb4-130">DailyRecurrence</span></span>](https://msdn.microsoft.com/library/0aaf265d-b723-49c6-8e9c-9ba60141e9ab%28Office.15%29.aspx) <br/> |<span data-ttu-id="c3cb4-131">毎日繰り返します。</span><span class="sxs-lookup"><span data-stu-id="c3cb4-131">Repeat every day.</span></span>  <br/> <span data-ttu-id="c3cb4-132">隔日で繰り返します。</span><span class="sxs-lookup"><span data-stu-id="c3cb4-132">Repeat every other day.</span></span>  <br/> |
|[<span data-ttu-id="c3cb4-133">Recurrence.MonthlyPattern</span><span class="sxs-lookup"><span data-stu-id="c3cb4-133">Recurrence.MonthlyPattern</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.monthlypattern%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="c3cb4-134">AbsoluteMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="c3cb4-134">AbsoluteMonthlyRecurrence</span></span>](https://msdn.microsoft.com/library/178fa0ae-9dfc-417f-933c-d657d31c2161%28Office.15%29.aspx) <br/> |<span data-ttu-id="c3cb4-135">毎月 10 日に繰り返します。</span><span class="sxs-lookup"><span data-stu-id="c3cb4-135">Repeat every month on the tenth day of the month.</span></span>  <br/> <span data-ttu-id="c3cb4-136">隔月の 21 日に繰り返します。</span><span class="sxs-lookup"><span data-stu-id="c3cb4-136">Repeat every other month on the twenty-first day of the month.</span></span>  <br/> |
|[<span data-ttu-id="c3cb4-137">Recurrence.RelativeMonthlyPattern</span><span class="sxs-lookup"><span data-stu-id="c3cb4-137">Recurrence.RelativeMonthlyPattern</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.relativemonthlypattern%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="c3cb4-138">RelativeMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="c3cb4-138">RelativeMonthlyRecurrence</span></span>](https://msdn.microsoft.com/library/a76595db-7460-44ac-ac2a-53241caa33a7%28Office.15%29.aspx) <br/> |<span data-ttu-id="c3cb4-139">毎月第 2 火曜日に繰り返します。</span><span class="sxs-lookup"><span data-stu-id="c3cb4-139">Repeat on the second Tuesday of every month.</span></span>  <br/> <span data-ttu-id="c3cb4-140">3 か月ごとの第 3 木曜日に繰り返します。</span><span class="sxs-lookup"><span data-stu-id="c3cb4-140">Repeat on the third Thursday of the month every three months.</span></span>  <br/> |
|[<span data-ttu-id="c3cb4-141">Recurrence.RelativeYearlyPattern</span><span class="sxs-lookup"><span data-stu-id="c3cb4-141">Recurrence.RelativeYearlyPattern</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.relativeyearlypattern%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="c3cb4-142">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="c3cb4-142">RelativeYearlyRecurrence</span></span>](https://msdn.microsoft.com/library/25b67876-9979-4a30-a637-357ea10a93b8%28Office.15%29.aspx) <br/> |<span data-ttu-id="c3cb4-143">毎年 8 月の第 1 月曜日に繰り返します。</span><span class="sxs-lookup"><span data-stu-id="c3cb4-143">Repeat on the first Monday of August every year.</span></span>  <br/> |
|[<span data-ttu-id="c3cb4-144">Recurrence.WeeklyPattern</span><span class="sxs-lookup"><span data-stu-id="c3cb4-144">Recurrence.WeeklyPattern</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.weeklypattern%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="c3cb4-145">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="c3cb4-145">WeeklyRecurrence</span></span>](https://msdn.microsoft.com/library/69c41dd5-597c-45bc-be3f-e2f2b5615aa3%28Office.15%29.aspx) <br/> |<span data-ttu-id="c3cb4-146">毎週月曜日に繰り返します。</span><span class="sxs-lookup"><span data-stu-id="c3cb4-146">Repeat every Monday.</span></span>  <br/> <span data-ttu-id="c3cb4-147">隔週の火曜日と木曜日に繰り返します。</span><span class="sxs-lookup"><span data-stu-id="c3cb4-147">Repeat every Tuesday and Thursday every other week.</span></span>  <br/> |
|[<span data-ttu-id="c3cb4-148">Recurrence.YearlyPattern</span><span class="sxs-lookup"><span data-stu-id="c3cb4-148">Recurrence.YearlyPattern</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.yearlypattern%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="c3cb4-149">AbsoluteYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="c3cb4-149">AbsoluteYearlyRecurrence</span></span>](https://msdn.microsoft.com/library/96f53e2c-3893-4f6e-a78a-ac179f45c5db%28Office.15%29.aspx) <br/> |<span data-ttu-id="c3cb4-150">毎年 9 月 1 日に繰り返します。</span><span class="sxs-lookup"><span data-stu-id="c3cb4-150">Repeat on September 1st every year.</span></span>  <br/> |
   
<span data-ttu-id="c3cb4-p104">定期的なパターンについての別の重要な情報は、定期的なアイテムが終了するのはいつかということです。これは、アイテムのセット数、終了日、または終了日なしとして表すことができます。</span><span class="sxs-lookup"><span data-stu-id="c3cb4-p104">The other important piece of information for a recurrence pattern is when the recurrence ends. This can be expressed as either a set number of occurrences, as an end date, or as having no end.</span></span>
  
<span data-ttu-id="c3cb4-153">**表 2. 定期的なアイテムの終了オプション**</span><span class="sxs-lookup"><span data-stu-id="c3cb4-153">**Table 2. Options for the end of a recurring series**</span></span>

|<span data-ttu-id="c3cb4-154">**EWS マネージ API メソッド/プロパティ**</span><span class="sxs-lookup"><span data-stu-id="c3cb4-154">**EWS Managed API method/property**</span></span>|<span data-ttu-id="c3cb4-155">**EWS の要素**</span><span class="sxs-lookup"><span data-stu-id="c3cb4-155">**EWS element**</span></span>|<span data-ttu-id="c3cb4-156">**説明**</span><span class="sxs-lookup"><span data-stu-id="c3cb4-156">**Description**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="c3cb4-157">Recurrence.NumberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="c3cb4-157">Recurrence.NumberOfOccurrences</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.numberofoccurrences%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="c3cb4-158">NumberedRecurrence</span><span class="sxs-lookup"><span data-stu-id="c3cb4-158">NumberedRecurrence</span></span>](https://msdn.microsoft.com/library/53746909-ef21-4764-8715-a7769b943cca%28Office.15%29.aspx) <br/> |<span data-ttu-id="c3cb4-159">このプロパティまたは要素の値は、アイテムの数を指定します。</span><span class="sxs-lookup"><span data-stu-id="c3cb4-159">The value of this property or element specifies the number of occurrences.</span></span>  <br/> |
|[<span data-ttu-id="c3cb4-160">Recurrence.EndDate</span><span class="sxs-lookup"><span data-stu-id="c3cb4-160">Recurrence.EndDate</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.enddate%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="c3cb4-161">EndDateRecurrence</span><span class="sxs-lookup"><span data-stu-id="c3cb4-161">EndDateRecurrence</span></span>](https://msdn.microsoft.com/library/a5ee2504-db84-49ee-870c-cca9269f2e26%28Office.15%29.aspx) <br/> |<span data-ttu-id="c3cb4-162">定期的なアイテムの最後のアイテムは、このプロパティまたは要素で指定された日付の当日またはそれ以前になります。</span><span class="sxs-lookup"><span data-stu-id="c3cb4-162">The last occurrence in the series falls on or before the date specified by this property or element.</span></span>  <br/> |
|[<span data-ttu-id="c3cb4-163">Recurrence.HasEnd</span><span class="sxs-lookup"><span data-stu-id="c3cb4-163">Recurrence.HasEnd</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.hasend%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="c3cb4-164">Recurrence.NeverEnds</span><span class="sxs-lookup"><span data-stu-id="c3cb4-164">Recurrence.NeverEnds</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.neverends%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="c3cb4-165">NoEndRecurrence</span><span class="sxs-lookup"><span data-stu-id="c3cb4-165">NoEndRecurrence</span></span>](https://msdn.microsoft.com/library/ab2ebd9c-388e-45f1-abf9-56e293ef123b%28Office.15%29.aspx) <br/> |<span data-ttu-id="c3cb4-166">定期的なアイテムには終わりがありません。</span><span class="sxs-lookup"><span data-stu-id="c3cb4-166">The series has no end.</span></span>  <br/> |
   
## <a name="expanded-vs-non-expanded-views"></a><span data-ttu-id="c3cb4-167">展開ビューと非展開ビュー</span><span class="sxs-lookup"><span data-stu-id="c3cb4-167">Expanded vs. non-expanded views</span></span>

<span data-ttu-id="c3cb4-p105">EWS マネージ API で **FindAppointments** メソッド (または EWS で **CalendarView** 要素を設定した **FindItem** 操作) を使用して、展開プロセスを呼び出します。これは結果セットからの定期的マスターの予定を非表示にし、その代わりに、その定期的なアイテムの展開ビューを表示します。予定表ビューのパラメーターに入る定期的マスターのアイテムと例外は、結果セットに含まれます。これとは逆に、EWS マネージ API で **FindItems** メソッド (または EWS で **IndexedPageItemView** または **FractionalPageItemView** 要素を設定した **FindItem** 操作) を使用しても、展開プロセスは呼び出されません。また、アイテムと例外も含まれません。2 つのメソッドを比較した例を紹介します。</span><span class="sxs-lookup"><span data-stu-id="c3cb4-p105">Using the **FindAppointments** method in the EWS Managed API (or the **FindItem** operation with a **CalendarView** element in EWS) invokes the expansion process. This hides recurring master appointments from the result set, and instead presents an expanded view of that recurring series. Occurrences of and exceptions to the recurring master that fall within the parameters of the calendar view are included in the result set. Conversely, using the **FindItems** method in the EWS Managed API (or the **FindItem** operation with a **IndexedPageItemView** or **FractionalPageItemView** element in EWS), does not invoke the expansion process, and occurrences and exceptions are not included. Let's look at an example comparing the two methods.</span></span> 
  
<span data-ttu-id="c3cb4-173">**表 3. 予定を検索するメソッドと操作**</span><span class="sxs-lookup"><span data-stu-id="c3cb4-173">**Table 3. Methods and operations for finding appointments**</span></span>

|<span data-ttu-id="c3cb4-174">**EWS マネージ API メソッド**</span><span class="sxs-lookup"><span data-stu-id="c3cb4-174">**EWS Managed API method**</span></span>|<span data-ttu-id="c3cb4-175">**EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="c3cb4-175">**EWS operation**</span></span>|<span data-ttu-id="c3cb4-176">**定期的なアイテムの展開**</span><span class="sxs-lookup"><span data-stu-id="c3cb4-176">**Expands series?**</span></span>|<span data-ttu-id="c3cb4-177">**結果に含まれるアイテム**</span><span class="sxs-lookup"><span data-stu-id="c3cb4-177">**Items included in results**</span></span>|
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="c3cb4-178">ExchangeService.FindAppointments</span><span class="sxs-lookup"><span data-stu-id="c3cb4-178">ExchangeService.FindAppointments</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="c3cb4-179">[CalendarView](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) 要素を設定した [FindItem 操作](https://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="c3cb4-179">[FindItem operation](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) with a [CalendarView](https://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx) element</span></span>  <br/> |<span data-ttu-id="c3cb4-180">はい</span><span class="sxs-lookup"><span data-stu-id="c3cb4-180">Yes</span></span>  <br/> |<span data-ttu-id="c3cb4-181">非定期的な予定、定期的なアイテムの 1 つのアイテム、および定期的なアイテムに対する例外</span><span class="sxs-lookup"><span data-stu-id="c3cb4-181">Non-recurring appointments, single occurrences of recurring series, and exceptions to recurring series</span></span>  <br/> |
|[<span data-ttu-id="c3cb4-182">ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="c3cb4-182">ExchangeService.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="c3cb4-183">[IndexedPageItemView](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) 要素または [FractionalPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) 要素を設定した [FindItem 操作](https://msdn.microsoft.com/library/4111afec-35e7-4c6f-b291-9bbba603f633%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="c3cb4-183">[FindItem operation](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) with an [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) element or [FractionalPageItemView](https://msdn.microsoft.com/library/4111afec-35e7-4c6f-b291-9bbba603f633%28Office.15%29.aspx) element</span></span>  <br/> |<span data-ttu-id="c3cb4-184">いいえ</span><span class="sxs-lookup"><span data-stu-id="c3cb4-184">No</span></span>  <br/> |<span data-ttu-id="c3cb4-185">非定期的な予定と定期的マスターの予定</span><span class="sxs-lookup"><span data-stu-id="c3cb4-185">Non-recurring appointments and recurring master appointments</span></span>  <br/> |
   
<span data-ttu-id="c3cb4-p106">Sadie は最近、自分の息子を水泳チームに参加させました。チームは毎週水曜日の午前 8 時 30 分に練習を行います。7 月 2 日から練習が始まり、最後の練習は 8 月 6 日に行われます。練習を忘れてはいけないので、Sadie は自分の予定表に定期的な予定を追加して、忘れないようにしました。</span><span class="sxs-lookup"><span data-stu-id="c3cb4-p106">Sadie has just signed her son up for swim team. The team has practice every Wednesday morning at 8:30 AM, starting July 2, with the last practice being on August 6. Not wanting to forget about practice, Sadie adds a recurring appointment to her calendar to remind her.</span></span>
  
<span data-ttu-id="c3cb4-189">**表 4. Sadie の定期的な予定**</span><span class="sxs-lookup"><span data-stu-id="c3cb4-189">**Table 4. Sadie's recurring appointment**</span></span>

|<span data-ttu-id="c3cb4-190">**予定フィールド**</span><span class="sxs-lookup"><span data-stu-id="c3cb4-190">**Appointment field**</span></span>|<span data-ttu-id="c3cb4-191">**値**</span><span class="sxs-lookup"><span data-stu-id="c3cb4-191">**Value**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c3cb4-192">件名</span><span class="sxs-lookup"><span data-stu-id="c3cb4-192">Subject</span></span>  <br/> |<span data-ttu-id="c3cb4-193">水泳チームの練習</span><span class="sxs-lookup"><span data-stu-id="c3cb4-193">Swim Team Practice</span></span>  <br/> |
|<span data-ttu-id="c3cb4-194">開始</span><span class="sxs-lookup"><span data-stu-id="c3cb4-194">Start</span></span>  <br/> |<span data-ttu-id="c3cb4-195">2014 年 7 月 2 日午前 8 時 30 分</span><span class="sxs-lookup"><span data-stu-id="c3cb4-195">July 2, 2014 8:30 AM</span></span>  <br/> |
|<span data-ttu-id="c3cb4-196">終了</span><span class="sxs-lookup"><span data-stu-id="c3cb4-196">End</span></span>  <br/> |<span data-ttu-id="c3cb4-197">2014 年 7 月 2 日午前 10 時 00 分</span><span class="sxs-lookup"><span data-stu-id="c3cb4-197">July 2, 2014 10:00 AM</span></span>  <br/> |
|<span data-ttu-id="c3cb4-198">繰り返し</span><span class="sxs-lookup"><span data-stu-id="c3cb4-198">Recurs</span></span>  <br/> |<span data-ttu-id="c3cb4-199">毎週水曜日</span><span class="sxs-lookup"><span data-stu-id="c3cb4-199">Every Wednesday</span></span>  <br/> |
|<span data-ttu-id="c3cb4-200">最後のアイテム</span><span class="sxs-lookup"><span data-stu-id="c3cb4-200">Last occurrence</span></span>  <br/> |<span data-ttu-id="c3cb4-201">2014 年 8 月 6 日午前 8 時 30 分</span><span class="sxs-lookup"><span data-stu-id="c3cb4-201">August 6, 2014 8:30 AM</span></span>  <br/> |
   
<span data-ttu-id="c3cb4-p107">予定表を一瞥すると、チームは合計 6 回の練習を行うと示されています。しかし予定表には、6 つの個別の予定アイテムはありません。その代わりに、定期的なアイテムを代表する定期的マスターの予定が 1 つだけあります。</span><span class="sxs-lookup"><span data-stu-id="c3cb4-p107">A quick look at a calendar shows that the team will have a total of six practices. However, there aren't six distinct appointment items in the calendar. Instead, there is just one recurring master appointment representing the series.</span></span>
  
<span data-ttu-id="c3cb4-p108">ここで、Sadie の予定表の、7 月中に発生する予定を見つけることについて説明します。次のコード例では、Exchange マネージ API の **FindItems** メソッドを使用して、Sadie の予定表の非展開ビューを作成します。</span><span class="sxs-lookup"><span data-stu-id="c3cb4-p108">Now let's look at finding appointments on Sadie's calendar that occur within the month of July. The following code example uses the **FindItems** method in the Exchange Managed API to produce a non-expanded view of Sadie's calendar.</span></span> 
  
```cs
PropertySet propSet = new PropertySet(AppointmentSchema.Subject,
                                      AppointmentSchema.Location,
                                      AppointmentSchema.Start, 
                                      AppointmentSchema.End,
                                      AppointmentSchema.AppointmentType);
#region FindItems + ItemView method
ItemView itemView = new ItemView(100);
itemView.PropertySet = propSet;
List<SearchFilter> filterList = new List<SearchFilter>();
// Find appointments that start after midnight on July 1, 2014.
SearchFilter.IsGreaterThan startFilter = new SearchFilter.IsGreaterThan(AppointmentSchema.Start,
    new DateTime(2014, 7, 1));
// Find appointments that end before midnight on July 31, 2014
SearchFilter.IsLessThan endFilter = new SearchFilter.IsLessThan(AppointmentSchema.End,
    new DateTime(2014, 7, 31));
filterList.Add(startFilter);
filterList.Add(endFilter);
SearchFilter.SearchFilterCollection calendarFilter = new SearchFilter.SearchFilterCollection(LogicalOperator.And, filterList);
// This results in a call to EWS.
FindItemsResults<Item> results = service.FindItems(WellKnownFolderName.Calendar, calendarFilter, itemView);
foreach(Item appt in results.Items)
{
    Console.WriteLine(appt.Subject);
}
```

<span data-ttu-id="c3cb4-207">このコードの結果は、次に示す [IndexedPageItemView](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) 要素を設定した [FindItem 操作](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx)要求になります。</span><span class="sxs-lookup"><span data-stu-id="c3cb4-207">That code results in the following [FindItem operation](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) request with an [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) element.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="calendar:Location" />
          <t:FieldURI FieldURI="calendar:Start" />
          <t:FieldURI FieldURI="calendar:End" />
          <t:FieldURI FieldURI="calendar:CalendarItemType" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="100" Offset="0" BasePoint="Beginning" />
      <m:Restriction>
        <t:And>
          <t:IsGreaterThan>
            <t:FieldURI FieldURI="calendar:Start" />
            <t:FieldURIOrConstant>
              <t:Constant Value="2014-07-01T07:00:00.000Z" />
            </t:FieldURIOrConstant>
          </t:IsGreaterThan>
          <t:IsLessThan>
            <t:FieldURI FieldURI="calendar:End" />
            <t:FieldURIOrConstant>
              <t:Constant Value="2014-07-31T07:00:00.000Z" />
            </t:FieldURIOrConstant>
          </t:IsLessThan>
        </t:And>
      </m:Restriction>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="calendar" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="c3cb4-p109">サーバーの応答には、 [RecurringMaster](https://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) の **CalendarItemType** 要素の値を示す 1 つのアイテム (定期的マスター) のみが含まれます。 [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) 要素の値は読みやすいよう短縮されています。</span><span class="sxs-lookup"><span data-stu-id="c3cb4-p109">The server's response includes only a single item, the recurring master, indicated by the [CalendarItemType](https://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) element value of **RecurringMaster**. The value of the [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) element has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="939" MinorBuildNumber="16" Version="V2_11" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="1" TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Items>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA5..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-02T15:30:00Z</t:Start>
                <t:End>2014-07-02T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>RecurringMaster</t:CalendarItemType>
              </t:CalendarItem>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="c3cb4-p110">では、展開ビューと比較してみましょう。次のコード例では、EWS マネージ API の **FindAppointments** メソッドを使用して、Sadie の予定表の展開ビューを作成します。</span><span class="sxs-lookup"><span data-stu-id="c3cb4-p110">Now let's compare with an expanded view. The following code example uses the **FindAppointments** method in the EWS Managed API to create an expanded view of Sadie's calendar.</span></span> 
  
```cs
PropertySet propSet = new PropertySet(AppointmentSchema.Subject,
                                      AppointmentSchema.Location,
                                      AppointmentSchema.Start, 
                                      AppointmentSchema.End,
                                      AppointmentSchema.AppointmentType);
CalendarView calView = new CalendarView(new DateTime(2014, 7, 1),
    new DateTime(2014, 7, 31));
calView.PropertySet = propSet;
FindItemsResults<Appointment> results = service.FindAppointments(WellKnownFolderName.Calendar, calView);
foreach(Appointment appt in results.Items)
{
    Console.WriteLine(appt.Subject);
}
```

<span data-ttu-id="c3cb4-212">このコードの結果は、次に示す [CalendarView](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) 要素を設定した [FindItem 操作](https://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx)要求になります。</span><span class="sxs-lookup"><span data-stu-id="c3cb4-212">This code results in the following [FindItem operation](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) request with a [CalendarView](https://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx) element.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="calendar:Location" />
          <t:FieldURI FieldURI="calendar:Start" />
          <t:FieldURI FieldURI="calendar:End" />
          <t:FieldURI FieldURI="calendar:CalendarItemType" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:CalendarView StartDate="2014-07-01T07:00:00.000Z" EndDate="2014-07-31T07:00:00.000Z" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="calendar" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="c3cb4-p111">今度は、サーバーの応答に 5 つのアイテム (7 月の各水曜日につき 1 つ) が含まれます。これらのアイテムの [CalendarItemType](https://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) 要素は、すべて **Occurrence** の値を持っています。定期的マスターはこの応答に存在しない点に注意してください。 [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) 要素の値は、読みやすいよう短縮されています。</span><span class="sxs-lookup"><span data-stu-id="c3cb4-p111">This time, the server response includes five occurrences, one for each Wednesday in July. The [CalendarItemType](https://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) elements on these items all have a value of **Occurrence**. Note that the recurring master is not present in the response. The values of the [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="939" MinorBuildNumber="16" Version="V2_11" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder TotalItemsInView="5" IncludesLastItemInRange="true">
            <t:Items>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA6..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-02T15:30:00Z</t:Start>
                <t:End>2014-07-02T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA7..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-09T15:30:00Z</t:Start>
                <t:End>2014-07-09T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA8..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-16T15:30:00Z</t:Start>
                <t:End>2014-07-16T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA9..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-23T15:30:00Z</t:Start>
                <t:End>2014-07-23T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADAA..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-30T15:30:00Z</t:Start>
                <t:End>2014-07-30T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="c3cb4-p112">定期的マスター、アイテム、または例外があれば、いつでも[別の関連アイテムを取得](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)できます。アイテムまたは例外を指定すると定期的マスターを取得できます。この逆も可能です。</span><span class="sxs-lookup"><span data-stu-id="c3cb4-p112">After you have a recurring master, an occurrence, or an exception, you can always [retrieve the other related items](how-to-access-a-recurring-series-by-using-ews-in-exchange.md). Given an occurrence or exception, you can retrieve the recurring master, and vice versa.</span></span>
  
## <a name="working-with-recurring-calendar-items"></a><span data-ttu-id="c3cb4-219">定期的な予定表アイテムの操作</span><span class="sxs-lookup"><span data-stu-id="c3cb4-219">Working with recurring calendar items</span></span>

<span data-ttu-id="c3cb4-p113">非定期的な予定表アイテムを操作するために使用するメソッドおよび操作と同じものを、定期的なアイテムを操作するために使用します。相違点は、実行するアクションが定期的なアイテム全体に適用されるか、1 つのアイテムのみに適用されるかが、それらのメソッドまたは操作を呼び出すために使用するアイテムによって決まることです。[定期的マスターに実行したアクション](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)は、定期的なアイテム内のすべてのアイテムに適用されますが、[1 つのアイテムまたは例外に実行したアクション](how-to-update-a-recurring-series-by-using-ews.md)は、そのアイテムまたは例外にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="c3cb4-p113">You use all the same methods and operations to work with recurring series as you use to work with non-recurring calendar items. The difference is that, depending on the item you use to invoke those methods or operations, the actions you take can apply to the entire series, or just a single occurrence. [Actions taken on the recurring master](how-to-update-a-recurring-series-by-using-ews-in-exchange.md) will apply to all occurrences in the series, while [actions taken to a single occurrence or exception](how-to-update-a-recurring-series-by-using-ews.md) will only apply to that occurrence or exception.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="c3cb4-223">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="c3cb4-223">In this section</span></span>

- [<span data-ttu-id="c3cb4-224">Exchange の EWS を使用して定期的なアイテムにアクセスする</span><span class="sxs-lookup"><span data-stu-id="c3cb4-224">Access a recurring series by using EWS in Exchange</span></span>](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="c3cb4-225">Exchange の EWS を使用して定期的なアイテムを作成する</span><span class="sxs-lookup"><span data-stu-id="c3cb4-225">Create a recurring series by using EWS in Exchange</span></span>](how-to-create-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="c3cb4-226">Exchange の EWS を使用して定期的なアイテムを削除する</span><span class="sxs-lookup"><span data-stu-id="c3cb4-226">Delete appointments in a recurring series by using EWS in Exchange</span></span>](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="c3cb4-227">EWS を使用して定期的なアイテムを更新する</span><span class="sxs-lookup"><span data-stu-id="c3cb4-227">Update a recurring series by using EWS</span></span>](how-to-update-a-recurring-series-by-using-ews.md)
    
- [<span data-ttu-id="c3cb4-228">Exchange の EWS を使用して定期的なアイテムを更新する</span><span class="sxs-lookup"><span data-stu-id="c3cb4-228">Update a recurring series by using EWS in Exchange</span></span>](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="c3cb4-229">関連項目</span><span class="sxs-lookup"><span data-stu-id="c3cb4-229">See also</span></span>


- [<span data-ttu-id="c3cb4-230">Exchange の予定表と EWS</span><span class="sxs-lookup"><span data-stu-id="c3cb4-230">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    
- [<span data-ttu-id="c3cb4-231">Exchange 用の Web サービス クライアントの開発</span><span class="sxs-lookup"><span data-stu-id="c3cb4-231">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="c3cb4-232">Exchange の EWS を使用して予定と会議を取得する</span><span class="sxs-lookup"><span data-stu-id="c3cb4-232">Get appointments and meetings by using EWS in Exchange</span></span>](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    

