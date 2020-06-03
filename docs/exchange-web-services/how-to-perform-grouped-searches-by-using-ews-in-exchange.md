---
title: Exchange で EWS を使用して、グループ化された検索を実行する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 55de92eb-8e8b-4156-8ad9-dd3828024242
description: EWS マネージ API または Exchange を対象とする EWS アプリケーションで、グループ化された検索を実行する方法を説明します。
ms.openlocfilehash: 65c6f75ea6b8ab848a263349dcceceead52fa210
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527932"
---
# <a name="perform-grouped-searches-by-using-ews-in-exchange"></a><span data-ttu-id="17934-103">Exchange で EWS を使用して、グループ化された検索を実行する</span><span class="sxs-lookup"><span data-stu-id="17934-103">Perform grouped searches by using EWS in Exchange</span></span>

<span data-ttu-id="17934-104">EWS マネージ API または Exchange を対象とする EWS アプリケーションで、グループ化された検索を実行する方法を説明します。</span><span class="sxs-lookup"><span data-stu-id="17934-104">Find out how to perform grouped searches in your EWS Managed API or EWS application that targets Exchange.</span></span>
  
<span data-ttu-id="17934-p101">グループ化された検索は、検索結果を整理する方法を管理できるという点が便利です。検索結果を整理することにより、管理可能な方法で、アプリケーションが結果を処理したり結果をエンド ユーザーに表示したりすることが簡単にできるようになります。</span><span class="sxs-lookup"><span data-stu-id="17934-p101">Grouped searches are useful in that they gives you control over how search results are organized. Organized search results can make it easier for your application to process results or display them to an end user in a manageable way.</span></span>
  
<span data-ttu-id="17934-p102">特定のフィールドの同じ値を持つ結果セット内のすべてのアイテムをグループに配置してグループ化します。たとえば、送信者ごとに結果をグループ化でき、同じ人のすべてのアイテムは別のグループに入れられ、各グループ内のアイテムはビューで指定した順序に従って並べ替えられます。グループ自体は、選択したフィールドに基づく集約値で並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="17934-p102">Grouping works by putting all items within the result set that have the same value of a specific field into a group. For example, you can group your results by the sender, and all items from the same person will be in a separate group, and the items within each group will be sorted according to the order you specify on the view. The groups themselves are sorted by an aggregate value based on a field you choose.</span></span>
  
<span data-ttu-id="17934-110">**表 1. 検索結果を整理するための EWS マネージ API のメソッドと EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="17934-110">**Table 1. EWS Managed API methods and EWS operations for organizing search results**</span></span>

|<span data-ttu-id="17934-111">**目的…**</span><span class="sxs-lookup"><span data-stu-id="17934-111">**If you want to…**</span></span>|<span data-ttu-id="17934-112">**EWS マネージ API で使用するもの**</span><span class="sxs-lookup"><span data-stu-id="17934-112">**In the EWS Managed API, use…**</span></span>|<span data-ttu-id="17934-113">**EWS で使用するもの**</span><span class="sxs-lookup"><span data-stu-id="17934-113">**In EWS, use…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="17934-114">結果内の特定のプロパティが同じ値のアイテムをグループに分類する</span><span class="sxs-lookup"><span data-stu-id="17934-114">Organize items with the same value in a specific property in your results into groups</span></span>  <br/> |[<span data-ttu-id="17934-115">Grouping.GroupOn</span><span class="sxs-lookup"><span data-stu-id="17934-115">Grouping.GroupOn</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.groupon%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="17934-116">[GroupBy](https://msdn.microsoft.com/library/9728619b-4674-4b9d-9f6c-e75c6165966c%28Office.15%29.aspx) 要素の子としての [FieldURI](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) 要素</span><span class="sxs-lookup"><span data-stu-id="17934-116">[FieldURI](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) element as a child of the [GroupBy](https://msdn.microsoft.com/library/9728619b-4674-4b9d-9f6c-e75c6165966c%28Office.15%29.aspx) element</span></span>  <br/> |
|<span data-ttu-id="17934-117">特定のプロパティの値によって各グループ内でアイテムを並べ替える</span><span class="sxs-lookup"><span data-stu-id="17934-117">Sort items within each group by the value in a specific property</span></span>  <br/> |[<span data-ttu-id="17934-118">ItemView.OrderBy</span><span class="sxs-lookup"><span data-stu-id="17934-118">ItemView.OrderBy</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview.orderby%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="17934-119">[SortOrder](https://msdn.microsoft.com/library/c2413f0b-8c03-46ae-9990-13338b3c53a6%28Office.15%29.aspx) 要素</span><span class="sxs-lookup"><span data-stu-id="17934-119">[SortOrder](https://msdn.microsoft.com/library/c2413f0b-8c03-46ae-9990-13338b3c53a6%28Office.15%29.aspx) element</span></span>  <br/> |
|<span data-ttu-id="17934-120">グループを並べ替える</span><span class="sxs-lookup"><span data-stu-id="17934-120">Sort the groups</span></span>  <br/> |[<span data-ttu-id="17934-121">Grouping.AggregateOn</span><span class="sxs-lookup"><span data-stu-id="17934-121">Grouping.AggregateOn</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.aggregateon%28v=exchg.80%29.aspx) <br/><br/> [<span data-ttu-id="17934-122">Grouping.AggregateType</span><span class="sxs-lookup"><span data-stu-id="17934-122">Grouping.AggregateType</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.aggregatetype%28v=exchg.80%29.aspx) <br/><br/> [<span data-ttu-id="17934-123">Grouping.SortDirection</span><span class="sxs-lookup"><span data-stu-id="17934-123">Grouping.SortDirection</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.sortdirection%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="17934-124">[AggregateOn](https://msdn.microsoft.com/library/9b0a03f2-3282-46e1-b1a0-cbb9a0fbe9bb%28Office.15%29.aspx) 要素の子としての **FieldURI** 要素</span><span class="sxs-lookup"><span data-stu-id="17934-124">**FieldURI** element as a child of the [AggregateOn](https://msdn.microsoft.com/library/9b0a03f2-3282-46e1-b1a0-cbb9a0fbe9bb%28Office.15%29.aspx) element</span></span><br/><br/> <span data-ttu-id="17934-125">**AggregateOn** 要素の **Aggregate** 属性</span><span class="sxs-lookup"><span data-stu-id="17934-125">**Aggregate** attribute on the **AggregateOn** element</span></span><br/><br/><span data-ttu-id="17934-126">**GroupBy** 要素の **Order** 属性</span><span class="sxs-lookup"><span data-stu-id="17934-126">**Order** attribute on the **GroupBy** element</span></span>  <br/> |
   
<span data-ttu-id="17934-127">それぞれ順を追って説明します。</span><span class="sxs-lookup"><span data-stu-id="17934-127">Let's take it step by step.</span></span>
  
## <a name="group-results-by-a-specific-property"></a><span data-ttu-id="17934-128">特定のプロパティによる結果のグループ化</span><span class="sxs-lookup"><span data-stu-id="17934-128">Group results by a specific property</span></span>
<span data-ttu-id="17934-129"><a name="bk_GroupResults"> </a></span><span class="sxs-lookup"><span data-stu-id="17934-129"><a name="bk_GroupResults"> </a></span></span>

<span data-ttu-id="17934-130">グループ化を使用する最初の手順は、グループ化するための、Exchange ストア内のアイテムのプロパティまたは属性を選択することです。</span><span class="sxs-lookup"><span data-stu-id="17934-130">The first step to using grouping is to select a property, or attribute on the items in the Exchange store, to group by.</span></span> <span data-ttu-id="17934-131">EWS マネージ API はこれらを対応するクラスのクラス プロパティとして公開するのに対し、EWS は XML 要素として公開します。</span><span class="sxs-lookup"><span data-stu-id="17934-131">The EWS Managed API exposes these as class properties on the corresponding classes, while EWS exposes them as XML elements.</span></span> <span data-ttu-id="17934-132">カスタム プロパティまたは拡張プロパティなど、任意のプロパティを選択することができますが、選択するプロパティの値に基づいてアイテムがグループ化される方法について理解しておくと役に立ちます。</span><span class="sxs-lookup"><span data-stu-id="17934-132">You can choose any property, including custom or extended properties, but it is helpful to understand how items are grouped based on the value of the property you choose.</span></span> 

<span data-ttu-id="17934-133">グループ化するために選択されたプロパティに同じ値を持つすべてのアイテムは、グループにまとめられます。</span><span class="sxs-lookup"><span data-stu-id="17934-133">All items that have the same value in the property you choose to group by will be grouped together.</span></span> <span data-ttu-id="17934-134">これは当然のことのようですが、重要な点です。</span><span class="sxs-lookup"><span data-stu-id="17934-134">This might seem obvious, but it is an important detail.</span></span> <span data-ttu-id="17934-135">EWS マネージ API の [Item.DateTimeReceived](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.datetimereceived%28v=exchg.80%29.aspx)、または EWS の [DateTimeReceived](https://msdn.microsoft.com/library/8f489bd4-2434-4d0a-91fe-1b5ba7eb5765%28Office.15%29.aspx) 要素など、日付/時刻プロパティでグループ化するとどうなるかを考えてみましょう。</span><span class="sxs-lookup"><span data-stu-id="17934-135">Consider what happens if you group by a date/time property, such as [Item.DateTimeReceived](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.datetimereceived%28v=exchg.80%29.aspx) in the EWS Managed API, or the [DateTimeReceived](https://msdn.microsoft.com/library/8f489bd4-2434-4d0a-91fe-1b5ba7eb5765%28Office.15%29.aspx) element in EWS.</span></span> <span data-ttu-id="17934-136">それぞれ同じ日のアイテムを含むグループになるよう、結果をグループ分けする場合があります。</span><span class="sxs-lookup"><span data-stu-id="17934-136">The intent might be to organize the results into groups, with each group containing items from the same day.</span></span> <span data-ttu-id="17934-137">ただし、グループ化では値全体が対象になります。これには時間が含まれます。</span><span class="sxs-lookup"><span data-stu-id="17934-137">However, grouping looks at the entire value, which includes the time.</span></span> 

<span data-ttu-id="17934-138">最終的には、同時に (秒単位で正確に) 受け取られたアイテムが独自のグループに入るようにグループ化されます。</span><span class="sxs-lookup"><span data-stu-id="17934-138">The end result is that the items will be grouped so that items received at the same time, down to the second, are in their own groups.</span></span> <span data-ttu-id="17934-139">ほとんどの場合、各グループでアイテムの数が少ない多数のグループに並べ替えられることになります。</span><span class="sxs-lookup"><span data-stu-id="17934-139">The results will most likely be sorted into a large number of groups with a small number of items in each group.</span></span> 
  
<span data-ttu-id="17934-140">グループの数が少なくかつ各グループでアイテムの数が多い結果セットを取得するには、値の数が少ない可能性の高いプロパティ (EWS マネージ API の [EmailMessage.From](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.from%28v=exchg.80%29.aspx) または [Item.Categories](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.categories%28v=exchg.80%29.aspx)、または EWS の [From](https://msdn.microsoft.com/library/5a52d644-3677-4049-874c-12bd5c3080dc%28Office.15%29.aspx) または [Categories](https://msdn.microsoft.com/library/d84d4927-b524-4e62-bf3d-1f12fec8c21a%28Office.15%29.aspx) など) を選択します。</span><span class="sxs-lookup"><span data-stu-id="17934-140">To get a results set with a smaller number of groups and a larger number of items in each group, choose a property that is likely to have a smaller number of values, such as [EmailMessage.From](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.from%28v=exchg.80%29.aspx) or [Item.Categories](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.categories%28v=exchg.80%29.aspx) in the EWS Managed API, or [From](https://msdn.microsoft.com/library/5a52d644-3677-4049-874c-12bd5c3080dc%28Office.15%29.aspx) or [Categories](https://msdn.microsoft.com/library/d84d4927-b524-4e62-bf3d-1f12fec8c21a%28Office.15%29.aspx) in EWS.</span></span> <span data-ttu-id="17934-141">次の図は、受信トレイ内に表示されるメールの一覧を示します。</span><span class="sxs-lookup"><span data-stu-id="17934-141">The following figure shows a list of emails that appear in an Inbox.</span></span> 
  
<span data-ttu-id="17934-142">**図 1. 受信トレイ内のメッセージ**</span><span class="sxs-lookup"><span data-stu-id="17934-142">**Figure 1. Messages in an Inbox**</span></span>

![ユーザーの [受信トレイ] のメッセージのサンプル リスト。](media/Ex15_GroupedSearch_MsgList.png)
  
<span data-ttu-id="17934-144">**EmailMessage.From** プロパティで図 1 のアイテムをグループ化すると、2 つのグループに分けられます。1 つは Hope Gross から送信されたメッセージで、もう 1 つは Sadie Daniels から送信されたメッセージです。</span><span class="sxs-lookup"><span data-stu-id="17934-144">If you group the items in Figure 1 by the **EmailMessage.From** property, the result will be two groups, one for messages sent by Hope Gross, and one for messages sent by Sadie Daniels.</span></span> 
  
<span data-ttu-id="17934-145">**図 2. From プロパティに基づいてグループ分けされたメッセージ**</span><span class="sxs-lookup"><span data-stu-id="17934-145">**Figure 2. Messages separated into groups based on the From property**</span></span>

![From プロパティで 2 つのリストに分類されたメッセージを表示したイメージ。](media/Ex15_GroupedSearch_SeparateGroups.png)
  
## <a name="sort-the-items-within-groups"></a><span data-ttu-id="17934-147">グループ内でアイテムを並べ替える</span><span class="sxs-lookup"><span data-stu-id="17934-147">Sort the items within groups</span></span>
<span data-ttu-id="17934-148"><a name="bk_SortItems"> </a></span><span class="sxs-lookup"><span data-stu-id="17934-148"><a name="bk_SortItems"> </a></span></span>

<span data-ttu-id="17934-149">EWS マネージ API の [ItemView.OrderBy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview.orderby%28v=exchg.80%29.aspx) プロパティ、または EWS の [SortOrder](https://msdn.microsoft.com/library/c2413f0b-8c03-46ae-9990-13338b3c53a6%28Office.15%29.aspx) 要素を使用して、各グループ内でアイテムを並べ替える方法を制御することができます。</span><span class="sxs-lookup"><span data-stu-id="17934-149">You can control how items are sorted within each group by using the [ItemView.OrderBy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview.orderby%28v=exchg.80%29.aspx) property in the EWS Managed API, or the [SortOrder](https://msdn.microsoft.com/library/c2413f0b-8c03-46ae-9990-13338b3c53a6%28Office.15%29.aspx) element in EWS.</span></span> <span data-ttu-id="17934-150">同じ順序を各グループに適用します。</span><span class="sxs-lookup"><span data-stu-id="17934-150">The same ordering applies to each group.</span></span> <span data-ttu-id="17934-151">たとえば、**Item.DateTimeReceived** プロパティで図 1 のアイテムを降順に並べ替えると、Hope Gross から受信した最新のアイテムが Hope Gross グループの一番上になります。また、Sadie Daniels から受信した最新のアイテムは Sadie Daniels グループの一番上になります。</span><span class="sxs-lookup"><span data-stu-id="17934-151">For example, if you sort the items from Figure 1 by the **Item.DateTimeReceived** property, in descending order, the item most recently received from Hope Gross will be first in the Hope Gross group, and the item most recently received from Sadie Daniels will be first in the Sadie Daniels group.</span></span> <span data-ttu-id="17934-152">便利なことに、図 2 のグループは既にこの方法で並べ替えられています。</span><span class="sxs-lookup"><span data-stu-id="17934-152">Conveniently, the groups in Figure 2 are already sorted this way.</span></span> 
  
## <a name="sort-the-groups"></a><span data-ttu-id="17934-153">グループを並べ替える</span><span class="sxs-lookup"><span data-stu-id="17934-153">Sort the groups</span></span>
<span data-ttu-id="17934-154"><a name="bk_SortGroups"> </a></span><span class="sxs-lookup"><span data-stu-id="17934-154"><a name="bk_SortGroups"> </a></span></span>

<span data-ttu-id="17934-155">これでグループが確定したので、最後の手順でグループ自体を並べ替えます。</span><span class="sxs-lookup"><span data-stu-id="17934-155">Now that you have your groups settled, the final step is sorting the groups themselves.</span></span> <span data-ttu-id="17934-156">グループ自体に特定の値がないため、グループ化のプロセスでグループごとに並べ替えの値を割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="17934-156">Because the groups themselves have no specific values, the grouping process has to assign a sort value to each group.</span></span> <span data-ttu-id="17934-157">これを行うには、EWS マネージ API の [Grouping.AggregateOn](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.aggregateon%28v=exchg.80%29.aspx) プロパティ、または EWS の [AggregateOn](https://msdn.microsoft.com/library/9b0a03f2-3282-46e1-b1a0-cbb9a0fbe9bb%28Office.15%29.aspx) 要素の子としての [FieldURI](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) 要素で指定して、各グループ内で特定のプロパティの値を集約します。</span><span class="sxs-lookup"><span data-stu-id="17934-157">This is done by aggregation of the values of a specific property within each group, specified by the [Grouping.AggregateOn](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.aggregateon%28v=exchg.80%29.aspx) property in the EWS Managed API, or the [FieldURI](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) element as a child of the [AggregateOn](https://msdn.microsoft.com/library/9b0a03f2-3282-46e1-b1a0-cbb9a0fbe9bb%28Office.15%29.aspx) element in EWS.</span></span> <span data-ttu-id="17934-158">EWS マネージ API の [Grouping.AggregateType](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.aggregatetype%28v=exchg.80%29.aspx) プロパティ (または EWS の **AggregateOn** 要素の **Aggregate** 属性) は、グループの並べ替え対象の値 (最大値または最小値のいずれか) として割り当てる各グループ内のアイテムの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="17934-158">The [Grouping.AggregateType](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.aggregatetype%28v=exchg.80%29.aspx) property in the EWS Managed API (or the **Aggregate** attribute on the **AggregateOn** element in EWS) specifies which value from the items within each group is assigned to the sort value for the group — either the largest value or the smallest value.</span></span> <span data-ttu-id="17934-159">最後に、並べ替えの順序 (降順または昇順) を、EWS マネージ API の [Grouping.SortDirection](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.sortdirection%28v=exchg.80%29.aspx) プロパティまたは EWS の [GroupBy](https://msdn.microsoft.com/library/9728619b-4674-4b9d-9f6c-e75c6165966c%28Office.15%29.aspx) 要素の **Order** 属性で指定します。</span><span class="sxs-lookup"><span data-stu-id="17934-159">Finally, the sort order (descending or ascending) is specified by the [Grouping.SortDirection](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.sortdirection%28v=exchg.80%29.aspx) property in the EWS Managed API, or the **Order** attribute on the [GroupBy](https://msdn.microsoft.com/library/9728619b-4674-4b9d-9f6c-e75c6165966c%28Office.15%29.aspx) element in EWS.</span></span> 
  
<span data-ttu-id="17934-160">たとえば、図 2 のグループを **Item.DateTimeReceived** プロパティで集約し、最小値を使用して降順で並べ替えると、アイテムは図 3 に示す順序で返されます。</span><span class="sxs-lookup"><span data-stu-id="17934-160">For example, if the groups from Figure 2 are sorted by aggregating on the **Item.DateTimeReceived** property, using the smallest value, and sorting in descending order, the items are returned in the order in shown Figure 3.</span></span> 
  
<span data-ttu-id="17934-161">**図 3. DateTimeReceived プロパティによって並べ替えられたグループでのグループ化された検索結果**</span><span class="sxs-lookup"><span data-stu-id="17934-161">**Figure 3. Grouped search results with the groups sorted by the DateTimeReceived property**</span></span>

![From プロパティでグループ化された、並べ替えられたメッセージのリストを表示しているイメージ。グループは最小の受信日時で並び替えられています。](media/Ex15_GroupedSearch_Results.png)
  
<span data-ttu-id="17934-163">次のセクションでは、コードでグループ化と並べ替えをまとめてプルする方法を説明します。</span><span class="sxs-lookup"><span data-stu-id="17934-163">The next sections show you how you might pull grouping and sorting together in code.</span></span>
  
## <a name="example-perform-a-grouped-search-by-using-the-ews-managed-api"></a><span data-ttu-id="17934-164">例: EWS マネージ API を使用して、グループ化された検索を実行する</span><span class="sxs-lookup"><span data-stu-id="17934-164">Example: Perform a grouped search by using the EWS Managed API</span></span>
<span data-ttu-id="17934-165"><a name="bk_GroupSearchEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="17934-165"><a name="bk_GroupSearchEWSMA"> </a></span></span>

<span data-ttu-id="17934-166">次の EWS マネージ API メソッドではグループ化を使用できます。</span><span class="sxs-lookup"><span data-stu-id="17934-166">The following EWS Managed API methods can use grouping:</span></span>
  
- [<span data-ttu-id="17934-167">ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="17934-167">ExchangeService.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="17934-168">Folder.FindItems</span><span class="sxs-lookup"><span data-stu-id="17934-168">Folder.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
<span data-ttu-id="17934-169">次の例では **ExchangeService.FindItems** メソッドを使用しますが、同じルールと概念が **Folder.FindItems** メソッドにも適用されます。</span><span class="sxs-lookup"><span data-stu-id="17934-169">The following example uses the **ExchangeService.FindItems** method; however, the same rules and concepts apply to the **Folder.FindItems** method.</span></span> <span data-ttu-id="17934-170">この例では、**GroupItemsByFrom** と呼ばれるメソッドが定義されます。</span><span class="sxs-lookup"><span data-stu-id="17934-170">In this example, a method called **GroupItemsByFrom** is defined.</span></span> <span data-ttu-id="17934-171">パラメーターとして、[ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトと [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) オブジェクトを使用します。</span><span class="sxs-lookup"><span data-stu-id="17934-171">It takes an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and a [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) object as parameters.</span></span> <span data-ttu-id="17934-172">**EmailMessage.From** プロパティでグループ化し **Item.DateTimeReceived** プロパティで降順に並べ替えた、フォルダー内の最初の 50 アイテムを要求します。</span><span class="sxs-lookup"><span data-stu-id="17934-172">It requests the first 50 items in the folder, grouped by the **EmailMessage.From** property, sorted by the **Item.DateTimeReceived** property in descending order.</span></span> <span data-ttu-id="17934-173">グループ自体は、グループのアイテムの **Item.DateTimeReceived** プロパティの最小値によって降順で並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="17934-173">The groups themselves are sorted by the smallest **Item.DateTimeReceived** property value on their items, in descending order.</span></span> 
  
<span data-ttu-id="17934-174">この例では、**ExchangeService** オブジェクトは [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) プロパティと [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) プロパティの有効な値で初期化されているものとします。</span><span class="sxs-lookup"><span data-stu-id="17934-174">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
```cs
static void GroupItemsByFrom(ExchangeService service, WellKnownFolderName folder)
{
    // Limit the result set to 50 items.
    ItemView view = new ItemView(50);
    view.PropertySet = new PropertySet(ItemSchema.Subject,
                                       ItemSchema.DateTimeReceived,
                                       EmailMessageSchema.From,
                                       ItemSchema.Categories);
    // Item searches do not support Deep traversal.
    view.Traversal = ItemTraversal.Shallow;
    // Specify the sorting done within the groups.
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    // Configure grouping.
    Grouping groupByFrom = new Grouping();
    groupByFrom.GroupOn = EmailMessageSchema.From;
    groupByFrom.AggregateOn = ItemSchema.DateTimeReceived;
    groupByFrom.AggregateType = AggregateType.Minimum;
    groupByFrom.SortDirection = SortDirection.Descending;
    try
    {
        GroupedFindItemsResults<Item> results = service.FindItems(folder,
            view, groupByFrom);
        foreach (ItemGroup<Item> group in results.ItemGroups)
        {
            Console.WriteLine("Group: {0}", group.GroupIndex);
            foreach (Item item in group.Items)
            {
                if (item is EmailMessage)
                {
                    EmailMessage message = item as EmailMessage;
                    Console.WriteLine("From: {0}", message.From);
                    Console.WriteLine("Subject: {0}", message.Subject);
                    Console.WriteLine("Id: {0}\n", message.Id.ToString());
                }
            }
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while enumerating results: {0}", ex.Message);
    }
}
```

## <a name="example-perform-a-grouped-search-by-using-ews"></a><span data-ttu-id="17934-175">例: EWS を使用して、グループ化された検索を実行する</span><span class="sxs-lookup"><span data-stu-id="17934-175">Example: Perform a grouped search by using EWS</span></span>
<span data-ttu-id="17934-176"><a name="bk_GroupSearchEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="17934-176"><a name="bk_GroupSearchEWS"> </a></span></span>

<span data-ttu-id="17934-177">次の要求例では、**From** 要素でグループ化し **DateTimeReceived** 要素で降順に並べ替えた、フォルダー内の最初の 50 アイテムに対する [FindItem 操作](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)要求を示します。</span><span class="sxs-lookup"><span data-stu-id="17934-177">The following request example shows a [FindItem operation](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) request for the first 50 items in the folder, grouped by the **From** element, sorted by the **DateTimeReceived** element in descending order.</span></span> <span data-ttu-id="17934-178">グループ自体は、グループのアイテムの **DateTimeReceived** 要素の最小値によって降順で並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="17934-178">The groups themselves are sorted by the smallest **DateTimeReceived** element value on their items, in descending order.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Eastern Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="item:DateTimeReceived" />
          <t:FieldURI FieldURI="message:From" />
          <t:FieldURI FieldURI="item:Categories" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="50" Offset="0" BasePoint="Beginning" />
      <m:GroupBy Order="Descending">
        <t:FieldURI FieldURI="message:From" />
        <t:AggregateOn Aggregate="Minimum">
          <t:FieldURI FieldURI="item:DateTimeReceived" />
        </t:AggregateOn>
      </m:GroupBy>
      <m:SortOrder>
        <t:FieldOrder Order="Descending">
          <t:FieldURI FieldURI="item:DateTimeReceived" />
        </t:FieldOrder>
      </m:SortOrder>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="17934-179">サーバーは次の応答を返します。</span><span class="sxs-lookup"><span data-stu-id="17934-179">The server returns the following response.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
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
          <m:RootFolder IndexedPagingOffset="10" TotalItemsInView="8" IncludesLastItemInRange="true">
            <t:Groups>
              <t:GroupedItems>
                <t:GroupIndex>0</t:GroupIndex>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>Planning resources</t:Subject>
                    <t:DateTimeReceived>2013-12-10T17:41:05Z</t:DateTimeReceived>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=8D84A3F4CBB34D48838A3AECF99795C0-SADIE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>Timeline</t:Subject>
                    <t:DateTimeReceived>2013-12-10T17:40:37Z</t:DateTimeReceived>
                    <t:Categories>
                      <t:String>Project</t:String>
                    </t:Categories>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=8D84A3F4CBB34D48838A3AECF99795C0-SADIE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>For your perusal</t:Subject>
                    <t:DateTimeReceived>2013-11-20T21:51:16Z</t:DateTimeReceived>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=8D84A3F4CBB34D48838A3AECF99795C0-SADIE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>meeting notes</t:Subject>
                    <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                    <t:Categories>
                      <t:String>Blue category</t:String>
                    </t:Categories>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=8D84A3F4CBB34D48838A3AECF99795C0-SADIE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>Meeting notes</t:Subject>
                    <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=8D84A3F4CBB34D48838A3AECF99795C0-SADIE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                </t:Items>
              </t:GroupedItems>
              <t:GroupedItems>
                <t:GroupIndex>1</t:GroupIndex>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>Query</t:Subject>
                    <t:DateTimeReceived>2013-12-10T17:43:15Z</t:DateTimeReceived>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Hope Gross</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=9B55E4100C064D9D8C5F72FF36802ED3-HOPE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>Update</t:Subject>
                    <t:DateTimeReceived>2013-12-10T17:42:33Z</t:DateTimeReceived>
                    <t:Categories>
                      <t:String>Project</t:String>
                      <t:String>Blue category</t:String>
                    </t:Categories>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Hope Gross</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=9B55E4100C064D9D8C5F72FF36802ED3-HOPE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>This cat is hilarious!</t:Subject>
                    <t:DateTimeReceived>2013-10-15T20:22:12Z</t:DateTimeReceived>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Hope Gross</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=9B55E4100C064D9D8C5F72FF36802ED3-HOPE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                </t:Items>
              </t:GroupedItems>
            </t:Groups>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="version-differences"></a><span data-ttu-id="17934-180">バージョンの相違点</span><span class="sxs-lookup"><span data-stu-id="17934-180">Version differences</span></span>
<span data-ttu-id="17934-181"><a name="bk_VersionDiffs"> </a></span><span class="sxs-lookup"><span data-stu-id="17934-181"><a name="bk_VersionDiffs"> </a></span></span>

<span data-ttu-id="17934-182">メジャー バージョン 15 以降のビルド 15.0.775.38 以前のバージョンの Exchange では、SOAP 応答で [GroupedItems](https://msdn.microsoft.com/library/53170df4-4272-4b37-b23f-cd8e2d4a7396%28Office.15%29.aspx) 要素の代わりに **Group** 要素 (型 **GroupedItemsType**) が返されます。</span><span class="sxs-lookup"><span data-stu-id="17934-182">Versions of Exchange starting with major version 15 and ending with build 15.0.775.38 return **Group** elements (of type **GroupedItemsType**) in place of [GroupedItems](https://msdn.microsoft.com/library/53170df4-4272-4b37-b23f-cd8e2d4a7396%28Office.15%29.aspx) elements in the SOAP response.</span></span> <span data-ttu-id="17934-183">EWS マネージ API を使用している場合、これは [GroupedFindItemsResults.ItemGroups](https://msdn.microsoft.com/library/office/dd633961%28v=exchg.80%29.aspx) コレクションに含まれるオブジェクトが 0 になる原因になります。</span><span class="sxs-lookup"><span data-stu-id="17934-183">If you are using the EWS Managed API, this will cause the [GroupedFindItemsResults.ItemGroups](https://msdn.microsoft.com/library/office/dd633961%28v=exchg.80%29.aspx) collection to contain 0 objects.</span></span> <span data-ttu-id="17934-184">EWS を使用している場合は、**Group** 要素は **GroupedItems** 要素として処理される必要があります。</span><span class="sxs-lookup"><span data-stu-id="17934-184">If you are using EWS, **Group** elements should be handled as **GroupedItems** elements.</span></span> 
  
<span data-ttu-id="17934-185">メジャー バージョン 15 以降のバージョンの Exchange では、SOAP 応答で **true** に設定された **xsi:nil** 属性を持つ追加の **Group** 要素または **GroupedItems** 要素が返されます。</span><span class="sxs-lookup"><span data-stu-id="17934-185">Versions of Exchange starting with major version 15 return extra **Group** or **GroupedItems** elements with the **xsi:nil** attribute set to **true** in the SOAP response.</span></span> <span data-ttu-id="17934-186">EWS マネージ API を使用している場合、これらの追加の要素は [ServiceXmlDeserializationException](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.servicexmldeserializationexception%28v=exchg.80%29.aspx) がスローされる原因となります。</span><span class="sxs-lookup"><span data-stu-id="17934-186">If you are using the EWS Managed API, these extra elements will cause a [ServiceXmlDeserializationException](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.servicexmldeserializationexception%28v=exchg.80%29.aspx) to be thrown.</span></span> <span data-ttu-id="17934-187">EWS を使用している場合は、これらの余分な要素は無視します。</span><span class="sxs-lookup"><span data-stu-id="17934-187">If you are using EWS, these extra elements should be ignored.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="17934-188">関連項目</span><span class="sxs-lookup"><span data-stu-id="17934-188">See also</span></span>

- [<span data-ttu-id="17934-189">Exchange の検索と EWS</span><span class="sxs-lookup"><span data-stu-id="17934-189">Search and EWS in Exchange</span></span>](search-and-ews-in-exchange.md)    
- [<span data-ttu-id="17934-190">ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="17934-190">ExchangeService.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="17934-191">Folder.FindItems</span><span class="sxs-lookup"><span data-stu-id="17934-191">Folder.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)   
- [<span data-ttu-id="17934-192">クラスのグループ化</span><span class="sxs-lookup"><span data-stu-id="17934-192">Grouping class</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="17934-193">FindItem 操作</span><span class="sxs-lookup"><span data-stu-id="17934-193">FindItem operation</span></span>](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    

