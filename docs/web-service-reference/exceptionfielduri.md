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
description: ExceptionFieldURI 要素は、要求内の特定のエラーを識別します。 この要素を MessageXml ノードにエラー応答の一部としてのみ使用します。
ms.openlocfilehash: 79909405179cec0d0b86ad12bf52031e1daeb790
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760350"
---
# <a name="exceptionfielduri"></a><span data-ttu-id="761d5-104">ExceptionFieldURI</span><span class="sxs-lookup"><span data-stu-id="761d5-104">ExceptionFieldURI</span></span>

<span data-ttu-id="761d5-105">**ExceptionFieldURI**要素は、要求内の特定のエラーを識別します。</span><span class="sxs-lookup"><span data-stu-id="761d5-105">The **ExceptionFieldURI** element identifies particular errors in a request.</span></span> <span data-ttu-id="761d5-106">この要素を[MessageXml](messagexml.md)ノードにエラー応答の一部としてのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="761d5-106">This element is only used as part of an error response in the [MessageXml](messagexml.md) node.</span></span> 
  
```xml
<ExceptionFieldURI FieldURI="" />
```

 <span data-ttu-id="761d5-107">**ExceptionPropertyURIType**</span><span class="sxs-lookup"><span data-stu-id="761d5-107">**ExceptionPropertyURIType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="761d5-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="761d5-108">Attributes and elements</span></span>

<span data-ttu-id="761d5-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="761d5-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="761d5-110">属性</span><span class="sxs-lookup"><span data-stu-id="761d5-110">Attributes</span></span>

|<span data-ttu-id="761d5-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="761d5-111">**Attribute**</span></span>|<span data-ttu-id="761d5-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="761d5-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="761d5-113">**FieldURI**</span><span class="sxs-lookup"><span data-stu-id="761d5-113">**FieldURI**</span></span> <br/> |<span data-ttu-id="761d5-114">定期的なアイテムのプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="761d5-114">Identifies a property of an occurrence of a recurring item.</span></span> <span data-ttu-id="761d5-115">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="761d5-115">This attribute is required.</span></span>  <br/> |
   
#### <a name="fielduri-attribute"></a><span data-ttu-id="761d5-116">FieldURI 属性</span><span class="sxs-lookup"><span data-stu-id="761d5-116">FieldURI Attribute</span></span>

|<span data-ttu-id="761d5-117">**値**</span><span class="sxs-lookup"><span data-stu-id="761d5-117">**Value**</span></span>|<span data-ttu-id="761d5-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="761d5-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="761d5-119">添付ファイルの名前。</span><span class="sxs-lookup"><span data-stu-id="761d5-119">attachment:Name</span></span>  <br/> |<span data-ttu-id="761d5-120">エラーが含まれていると添付ファイル名を識別します。</span><span class="sxs-lookup"><span data-stu-id="761d5-120">Identifies the attachment name as containing an error.</span></span>  <br/> |
|<span data-ttu-id="761d5-121">: コンテンツ タイプの添付ファイル</span><span class="sxs-lookup"><span data-stu-id="761d5-121">attachment:ContentType</span></span>  <br/> |<span data-ttu-id="761d5-122">エラーが含まれているコンテンツの種類を識別します。</span><span class="sxs-lookup"><span data-stu-id="761d5-122">Identifies the content type as containing an error.</span></span>  <br/> |
|<span data-ttu-id="761d5-123">添付ファイルのコンテンツ。</span><span class="sxs-lookup"><span data-stu-id="761d5-123">attachment:Content</span></span>  <br/> |<span data-ttu-id="761d5-124">エラーがあること、コンテンツを識別します。</span><span class="sxs-lookup"><span data-stu-id="761d5-124">Identifies the content as containing an error.</span></span>  <br/> |
|<span data-ttu-id="761d5-125">定期的な月。</span><span class="sxs-lookup"><span data-stu-id="761d5-125">recurrence:Month</span></span>  <br/> |<span data-ttu-id="761d5-126">月] フィールドにエラーがあることを識別します。</span><span class="sxs-lookup"><span data-stu-id="761d5-126">Identifies the month field as containing an error.</span></span>  <br/> |
|<span data-ttu-id="761d5-127">定期的なアイテム: DayOfWeekIndex</span><span class="sxs-lookup"><span data-stu-id="761d5-127">recurrence:DayOfWeekIndex</span></span>  <br/> |<span data-ttu-id="761d5-128">日曜日のインデックス エラーがあることを識別します。</span><span class="sxs-lookup"><span data-stu-id="761d5-128">Identifies the day of week index as containing an error.</span></span>  <br/> |
|<span data-ttu-id="761d5-129">DaysOfWeek の定期的なアイテム。</span><span class="sxs-lookup"><span data-stu-id="761d5-129">recurrence:DaysOfWeek</span></span>  <br/> |<span data-ttu-id="761d5-130">DaysOfWeek プロパティ エラーがあることを識別します。</span><span class="sxs-lookup"><span data-stu-id="761d5-130">Identifies the DaysOfWeek property as containing an error.</span></span>  <br/> |
|<span data-ttu-id="761d5-131">DayOfMonth の定期的なアイテム。</span><span class="sxs-lookup"><span data-stu-id="761d5-131">recurrence:DayOfMonth</span></span>  <br/> |<span data-ttu-id="761d5-132">DayOfMonth エラーがあることを識別します。</span><span class="sxs-lookup"><span data-stu-id="761d5-132">Identifies the DayOfMonth as containing an error.</span></span>  <br/> |
|<span data-ttu-id="761d5-133">繰り返しの間隔:</span><span class="sxs-lookup"><span data-stu-id="761d5-133">recurrence:Interval</span></span>  <br/> |<span data-ttu-id="761d5-134">エラーが含まれているとの間隔を指定します。</span><span class="sxs-lookup"><span data-stu-id="761d5-134">Identifies the interval as containing an error.</span></span>  <br/> |
|<span data-ttu-id="761d5-135">定期的なアイテム: NumberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="761d5-135">recurrence:NumberOfOccurrences</span></span>  <br/> |<span data-ttu-id="761d5-136">エラーがあることの出現回数を指定します。</span><span class="sxs-lookup"><span data-stu-id="761d5-136">Identifies the number of occurrences as containing an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="761d5-137">子要素</span><span class="sxs-lookup"><span data-stu-id="761d5-137">Child elements</span></span>

<span data-ttu-id="761d5-138">なし。</span><span class="sxs-lookup"><span data-stu-id="761d5-138">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="761d5-139">親要素</span><span class="sxs-lookup"><span data-stu-id="761d5-139">Parent elements</span></span>

|<span data-ttu-id="761d5-140">**要素**</span><span class="sxs-lookup"><span data-stu-id="761d5-140">**Element**</span></span>|<span data-ttu-id="761d5-141">**説明**</span><span class="sxs-lookup"><span data-stu-id="761d5-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="761d5-142">MessageXml</span><span class="sxs-lookup"><span data-stu-id="761d5-142">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="761d5-143">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="761d5-143">Provides additional error response information.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="761d5-144">備考</span><span class="sxs-lookup"><span data-stu-id="761d5-144">Remarks</span></span>

<span data-ttu-id="761d5-145">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="761d5-145">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="761d5-146">要素情報</span><span class="sxs-lookup"><span data-stu-id="761d5-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="761d5-147">名前空間</span><span class="sxs-lookup"><span data-stu-id="761d5-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="761d5-148">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="761d5-148">Schema Name</span></span>  <br/> |<span data-ttu-id="761d5-149">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="761d5-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="761d5-150">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="761d5-150">Validation File</span></span>  <br/> |<span data-ttu-id="761d5-151">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="761d5-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="761d5-152">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="761d5-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="761d5-153">False</span><span class="sxs-lookup"><span data-stu-id="761d5-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="761d5-154">関連項目</span><span class="sxs-lookup"><span data-stu-id="761d5-154">See also</span></span>



- [<span data-ttu-id="761d5-155">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="761d5-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

