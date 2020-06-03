---
title: ExceptionFieldURI
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExceptionFieldURI
api_type:
- schema
ms.assetid: 7afda93a-0f8c-4c9e-8e09-f1b0bfc928bf
description: ExceptionFieldURI 要素は、要求の特定のエラーを識別します。 この要素は、MessageXml ノードでエラー応答の一部としてのみ使用されます。
ms.openlocfilehash: a47d44098f85d8bacb1e7a2c48a33e478e56c7ac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44454345"
---
# <a name="exceptionfielduri"></a><span data-ttu-id="602aa-104">ExceptionFieldURI</span><span class="sxs-lookup"><span data-stu-id="602aa-104">ExceptionFieldURI</span></span>

<span data-ttu-id="602aa-105">**ExceptionFieldURI**要素は、要求の特定のエラーを識別します。</span><span class="sxs-lookup"><span data-stu-id="602aa-105">The **ExceptionFieldURI** element identifies particular errors in a request.</span></span> <span data-ttu-id="602aa-106">この要素は、 [MessageXml](messagexml.md)ノードでエラー応答の一部としてのみ使用されます。</span><span class="sxs-lookup"><span data-stu-id="602aa-106">This element is only used as part of an error response in the [MessageXml](messagexml.md) node.</span></span> 
  
```xml
<ExceptionFieldURI FieldURI="" />
```

 <span data-ttu-id="602aa-107">**ExceptionPropertyURIType プロパティ**</span><span class="sxs-lookup"><span data-stu-id="602aa-107">**ExceptionPropertyURIType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="602aa-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="602aa-108">Attributes and elements</span></span>

<span data-ttu-id="602aa-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="602aa-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="602aa-110">属性</span><span class="sxs-lookup"><span data-stu-id="602aa-110">Attributes</span></span>

|<span data-ttu-id="602aa-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="602aa-111">**Attribute**</span></span>|<span data-ttu-id="602aa-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="602aa-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="602aa-113">**FieldURI**</span><span class="sxs-lookup"><span data-stu-id="602aa-113">**FieldURI**</span></span> <br/> |<span data-ttu-id="602aa-114">定期的なアイテムの発生のプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="602aa-114">Identifies a property of an occurrence of a recurring item.</span></span> <span data-ttu-id="602aa-115">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="602aa-115">This attribute is required.</span></span>  <br/> |
   
#### <a name="fielduri-attribute"></a><span data-ttu-id="602aa-116">FieldURI 属性</span><span class="sxs-lookup"><span data-stu-id="602aa-116">FieldURI Attribute</span></span>

|<span data-ttu-id="602aa-117">**値**</span><span class="sxs-lookup"><span data-stu-id="602aa-117">**Value**</span></span>|<span data-ttu-id="602aa-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="602aa-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="602aa-119">添付ファイル: 名前</span><span class="sxs-lookup"><span data-stu-id="602aa-119">attachment:Name</span></span>  <br/> |<span data-ttu-id="602aa-120">エラーが含まれる添付ファイルの名前を識別します。</span><span class="sxs-lookup"><span data-stu-id="602aa-120">Identifies the attachment name as containing an error.</span></span>  <br/> |
|<span data-ttu-id="602aa-121">添付ファイル: ContentType</span><span class="sxs-lookup"><span data-stu-id="602aa-121">attachment:ContentType</span></span>  <br/> |<span data-ttu-id="602aa-122">エラーが含まれるコンテンツタイプを識別します。</span><span class="sxs-lookup"><span data-stu-id="602aa-122">Identifies the content type as containing an error.</span></span>  <br/> |
|<span data-ttu-id="602aa-123">添付ファイル: コンテンツ</span><span class="sxs-lookup"><span data-stu-id="602aa-123">attachment:Content</span></span>  <br/> |<span data-ttu-id="602aa-124">エラーを含むコンテンツを識別します。</span><span class="sxs-lookup"><span data-stu-id="602aa-124">Identifies the content as containing an error.</span></span>  <br/> |
|<span data-ttu-id="602aa-125">定期的な予定: 月</span><span class="sxs-lookup"><span data-stu-id="602aa-125">recurrence:Month</span></span>  <br/> |<span data-ttu-id="602aa-126">エラーを含む month フィールドを識別します。</span><span class="sxs-lookup"><span data-stu-id="602aa-126">Identifies the month field as containing an error.</span></span>  <br/> |
|<span data-ttu-id="602aa-127">定期的なアイテム: DayOfWeekIndex</span><span class="sxs-lookup"><span data-stu-id="602aa-127">recurrence:DayOfWeekIndex</span></span>  <br/> |<span data-ttu-id="602aa-128">エラーが含まれる曜日インデックスを識別します。</span><span class="sxs-lookup"><span data-stu-id="602aa-128">Identifies the day of week index as containing an error.</span></span>  <br/> |
|<span data-ttu-id="602aa-129">定期的なアイテム: DaysOfWeek</span><span class="sxs-lookup"><span data-stu-id="602aa-129">recurrence:DaysOfWeek</span></span>  <br/> |<span data-ttu-id="602aa-130">エラーを含む DaysOfWeek プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="602aa-130">Identifies the DaysOfWeek property as containing an error.</span></span>  <br/> |
|<span data-ttu-id="602aa-131">定期的なアイテム: DayOfMonth</span><span class="sxs-lookup"><span data-stu-id="602aa-131">recurrence:DayOfMonth</span></span>  <br/> |<span data-ttu-id="602aa-132">エラーを含む DayOfMonth を識別します。</span><span class="sxs-lookup"><span data-stu-id="602aa-132">Identifies the DayOfMonth as containing an error.</span></span>  <br/> |
|<span data-ttu-id="602aa-133">繰り返し: 間隔</span><span class="sxs-lookup"><span data-stu-id="602aa-133">recurrence:Interval</span></span>  <br/> |<span data-ttu-id="602aa-134">エラーを含む間隔を識別します。</span><span class="sxs-lookup"><span data-stu-id="602aa-134">Identifies the interval as containing an error.</span></span>  <br/> |
|<span data-ttu-id="602aa-135">繰り返し: NumberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="602aa-135">recurrence:NumberOfOccurrences</span></span>  <br/> |<span data-ttu-id="602aa-136">エラーを含むオカレンスの数を識別します。</span><span class="sxs-lookup"><span data-stu-id="602aa-136">Identifies the number of occurrences as containing an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="602aa-137">子要素</span><span class="sxs-lookup"><span data-stu-id="602aa-137">Child elements</span></span>

<span data-ttu-id="602aa-138">なし。</span><span class="sxs-lookup"><span data-stu-id="602aa-138">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="602aa-139">親要素</span><span class="sxs-lookup"><span data-stu-id="602aa-139">Parent elements</span></span>

|<span data-ttu-id="602aa-140">**要素**</span><span class="sxs-lookup"><span data-stu-id="602aa-140">**Element**</span></span>|<span data-ttu-id="602aa-141">**説明**</span><span class="sxs-lookup"><span data-stu-id="602aa-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="602aa-142">MessageXml</span><span class="sxs-lookup"><span data-stu-id="602aa-142">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="602aa-143">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="602aa-143">Provides additional error response information.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="602aa-144">注釈</span><span class="sxs-lookup"><span data-stu-id="602aa-144">Remarks</span></span>

<span data-ttu-id="602aa-145">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="602aa-145">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="602aa-146">要素の情報</span><span class="sxs-lookup"><span data-stu-id="602aa-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="602aa-147">Namespace</span><span class="sxs-lookup"><span data-stu-id="602aa-147">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="602aa-148">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="602aa-148">Schema Name</span></span>  <br/> |<span data-ttu-id="602aa-149">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="602aa-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="602aa-150">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="602aa-150">Validation File</span></span>  <br/> |<span data-ttu-id="602aa-151">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="602aa-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="602aa-152">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="602aa-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="602aa-153">正しくない</span><span class="sxs-lookup"><span data-stu-id="602aa-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="602aa-154">関連項目</span><span class="sxs-lookup"><span data-stu-id="602aa-154">See also</span></span>



- [<span data-ttu-id="602aa-155">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="602aa-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

