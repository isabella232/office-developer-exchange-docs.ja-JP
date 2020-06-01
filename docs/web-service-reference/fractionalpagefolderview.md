---
title: FractionalPageFolderView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FractionalPageFolderView
api_type:
- schema
ms.assetid: ef681f8a-136a-4c0e-ade6-ddcdbf2d85ad
description: FractionalPageFolderView 要素は、ページビューの開始位置と、FindFolder 要求で返されるフォルダーの最大数を示します。
ms.openlocfilehash: a8627c6277b49655d3933679128b844118633cda
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463070"
---
# <a name="fractionalpagefolderview"></a><span data-ttu-id="0855c-103">FractionalPageFolderView</span><span class="sxs-lookup"><span data-stu-id="0855c-103">FractionalPageFolderView</span></span>

<span data-ttu-id="0855c-104">**FractionalPageFolderView**要素は、ページビューの開始位置と、 [findfolder](findfolder.md)要求で返されるフォルダーの最大数を示します。</span><span class="sxs-lookup"><span data-stu-id="0855c-104">The **FractionalPageFolderView** element describes where the paged view starts and the maximum number of folders returned in a [FindFolder](findfolder.md) request.</span></span> 
  
[<span data-ttu-id="0855c-105">FindFolder</span><span class="sxs-lookup"><span data-stu-id="0855c-105">FindFolder</span></span>](findfolder.md)
  
[<span data-ttu-id="0855c-106">FractionalPageFolderView</span><span class="sxs-lookup"><span data-stu-id="0855c-106">FractionalPageFolderView</span></span>](fractionalpagefolderview.md)
  
```xml
<FractionalPageFolderView MaxEntriesReturned="" Numerator="" Denominator=""/>
```

 <span data-ttu-id="0855c-107">**FractionalPageViewType**</span><span class="sxs-lookup"><span data-stu-id="0855c-107">**FractionalPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0855c-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0855c-108">Attributes and elements</span></span>

<span data-ttu-id="0855c-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0855c-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0855c-110">属性</span><span class="sxs-lookup"><span data-stu-id="0855c-110">Attributes</span></span>

|<span data-ttu-id="0855c-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="0855c-111">**Attribute**</span></span>|<span data-ttu-id="0855c-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="0855c-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0855c-113">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="0855c-113">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="0855c-114">[Findfolder](findfolder.md)応答で返される結果の最大数を指定します。</span><span class="sxs-lookup"><span data-stu-id="0855c-114">Identifies the maximum number of results to return in the [FindFolder](findfolder.md) response.</span></span> <span data-ttu-id="0855c-115">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="0855c-115">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="0855c-116">**分子**</span><span class="sxs-lookup"><span data-stu-id="0855c-116">**Numerator**</span></span> <br/> |<span data-ttu-id="0855c-117">結果セットの先頭からの、分数のオフセットの分子を表します。</span><span class="sxs-lookup"><span data-stu-id="0855c-117">Represents the numerator of the fractional offset from the start of the result set.</span></span> <span data-ttu-id="0855c-118">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="0855c-118">This attribute is required.</span></span> <span data-ttu-id="0855c-119">分子は、分母以下の値である必要があります。</span><span class="sxs-lookup"><span data-stu-id="0855c-119">The numerator must be equal to or less than the denominator.</span></span> <span data-ttu-id="0855c-120">この属性は、ゼロ以上の整数値を表す必要があります。</span><span class="sxs-lookup"><span data-stu-id="0855c-120">This attribute must represent an integral value that is equal to or greater than zero.</span></span> <span data-ttu-id="0855c-121">詳細については、このトピックで後述する「備考」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0855c-121">For more information, see Remarks later in this topic.</span></span>  <br/> |
|<span data-ttu-id="0855c-122">**分母**</span><span class="sxs-lookup"><span data-stu-id="0855c-122">**Denominator**</span></span> <br/> |<span data-ttu-id="0855c-123">結果セット内のフォルダーの総数の先頭からの、分単位のオフセットの分母を表します。</span><span class="sxs-lookup"><span data-stu-id="0855c-123">Represents the denominator of the fractional offset from the start of the total number of folders in the result set.</span></span> <span data-ttu-id="0855c-124">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="0855c-124">This attribute is required.</span></span> <span data-ttu-id="0855c-125">この属性は、1より大きい整数値を表す必要があります。</span><span class="sxs-lookup"><span data-stu-id="0855c-125">This attribute must represent an integral value that is greater than one.</span></span> <span data-ttu-id="0855c-126">詳細については、このトピックで後述する「備考」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0855c-126">For more information, see Remarks later in this topic.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0855c-127">子要素</span><span class="sxs-lookup"><span data-stu-id="0855c-127">Child elements</span></span>

<span data-ttu-id="0855c-128">なし。</span><span class="sxs-lookup"><span data-stu-id="0855c-128">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0855c-129">親要素</span><span class="sxs-lookup"><span data-stu-id="0855c-129">Parent elements</span></span>

|<span data-ttu-id="0855c-130">**要素**</span><span class="sxs-lookup"><span data-stu-id="0855c-130">**Element**</span></span>|<span data-ttu-id="0855c-131">**説明**</span><span class="sxs-lookup"><span data-stu-id="0855c-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0855c-132">FindFolder</span><span class="sxs-lookup"><span data-stu-id="0855c-132">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="0855c-133">メールボックス内のフォルダーを識別する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="0855c-133">Defines a request to identify folders in a mailbox.</span></span>  <br/> <span data-ttu-id="0855c-134">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0855c-134">The following is the XPath expression to this element:</span></span>  <br/>  `/FindFolder` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0855c-135">注釈</span><span class="sxs-lookup"><span data-stu-id="0855c-135">Remarks</span></span>

<span data-ttu-id="0855c-136">検索されたフォルダーのセットの先頭からのページビューオフセットは、分数で示されます。</span><span class="sxs-lookup"><span data-stu-id="0855c-136">The paged view offset from the start of the set of found folders is described by a fraction.</span></span> <span data-ttu-id="0855c-137">**分子**および**分母**属性で定義されている分数は、情報のページが開始する場所を示します。</span><span class="sxs-lookup"><span data-stu-id="0855c-137">The fraction, which is defined by the **Numerator** and **Denominator** attributes, describes where the page of information starts.</span></span> <span data-ttu-id="0855c-138">たとえば、**分子**が4で、**分母**が5の場合、返された情報のページは、結果セット内の fifths にあるエントリから始まります。</span><span class="sxs-lookup"><span data-stu-id="0855c-138">For example, if **Numerator** equals four and **Denominator** equals five, the page of returned information starts at an entry located four-fifths of the way in to the result set.</span></span> 
  
<span data-ttu-id="0855c-139">分数が0に評価された場合は、結果セットの開始を示します。</span><span class="sxs-lookup"><span data-stu-id="0855c-139">If the fraction evaluates to zero, that indicates the start of the results set.</span></span> <span data-ttu-id="0855c-140">分数が1に評価される場合は、結果セットの末尾を示します。</span><span class="sxs-lookup"><span data-stu-id="0855c-140">If the fraction evaluates to one, that indicates the end of the result set.</span></span>
  
> [!NOTE]
> <span data-ttu-id="0855c-141">分数は、結果セット内の結果の数ではなく、ページの開始点を表します。</span><span class="sxs-lookup"><span data-stu-id="0855c-141">The fraction represents the start point of page, not how many results in the result set will be returned.</span></span> 
  
<span data-ttu-id="0855c-142">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="0855c-142">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0855c-143">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0855c-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0855c-144">Namespace</span><span class="sxs-lookup"><span data-stu-id="0855c-144">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0855c-145">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0855c-145">Schema Name</span></span>  <br/> |<span data-ttu-id="0855c-146">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="0855c-146">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0855c-147">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0855c-147">Validation File</span></span>  <br/> |<span data-ttu-id="0855c-148">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="0855c-148">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0855c-149">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0855c-149">Can be Empty</span></span>  <br/> |<span data-ttu-id="0855c-150">正しくない</span><span class="sxs-lookup"><span data-stu-id="0855c-150">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0855c-151">関連項目</span><span class="sxs-lookup"><span data-stu-id="0855c-151">See also</span></span>



<span data-ttu-id="0855c-152">
  [FindFolder 操作](findfolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="0855c-152">[FindFolder operation](findfolder-operation.md)</span></span>


[<span data-ttu-id="0855c-153">フォルダーの検索</span><span class="sxs-lookup"><span data-stu-id="0855c-153">Finding Folders</span></span>](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

