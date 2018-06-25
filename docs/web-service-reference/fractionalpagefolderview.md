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
description: FractionalPageFolderView 要素は、ページ ビューが起動し、フォルダーの最大数は、FindFolder 要求で返されるについて説明します。
ms.openlocfilehash: 3cb5f8333634a0c484ae3ce6a6256631cff57cc5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760589"
---
# <a name="fractionalpagefolderview"></a><span data-ttu-id="46e9e-103">FractionalPageFolderView</span><span class="sxs-lookup"><span data-stu-id="46e9e-103">FractionalPageFolderView</span></span>

<span data-ttu-id="46e9e-104">**FractionalPageFolderView**要素は、ページ ビューが起動し、フォルダーの最大数は、 [FindFolder](findfolder.md)要求で返されるについて説明します。</span><span class="sxs-lookup"><span data-stu-id="46e9e-104">The **FractionalPageFolderView** element describes where the paged view starts and the maximum number of folders returned in a [FindFolder](findfolder.md) request.</span></span> 
  
[<span data-ttu-id="46e9e-105">FindFolder</span><span class="sxs-lookup"><span data-stu-id="46e9e-105">FindFolder</span></span>](findfolder.md)
  
[<span data-ttu-id="46e9e-106">FractionalPageFolderView</span><span class="sxs-lookup"><span data-stu-id="46e9e-106">FractionalPageFolderView</span></span>](fractionalpagefolderview.md)
  
```xml
<FractionalPageFolderView MaxEntriesReturned="" Numerator="" Denominator=""/>
```

 <span data-ttu-id="46e9e-107">**FractionalPageViewType**</span><span class="sxs-lookup"><span data-stu-id="46e9e-107">**FractionalPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="46e9e-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="46e9e-108">Attributes and elements</span></span>

<span data-ttu-id="46e9e-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="46e9e-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="46e9e-110">属性</span><span class="sxs-lookup"><span data-stu-id="46e9e-110">Attributes</span></span>

|<span data-ttu-id="46e9e-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="46e9e-111">**Attribute**</span></span>|<span data-ttu-id="46e9e-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="46e9e-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="46e9e-113">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="46e9e-113">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="46e9e-114">[FindFolder](findfolder.md)の応答で返す結果の最大数を指定します。</span><span class="sxs-lookup"><span data-stu-id="46e9e-114">Identifies the maximum number of results to return in the [FindFolder](findfolder.md) response.</span></span> <span data-ttu-id="46e9e-115">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="46e9e-115">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="46e9e-116">**分子**</span><span class="sxs-lookup"><span data-stu-id="46e9e-116">**Numerator**</span></span> <br/> |<span data-ttu-id="46e9e-117">結果セットの先頭からのオフセットを表す分数の分子を表します。</span><span class="sxs-lookup"><span data-stu-id="46e9e-117">Represents the numerator of the fractional offset from the start of the result set.</span></span> <span data-ttu-id="46e9e-118">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="46e9e-118">This attribute is required.</span></span> <span data-ttu-id="46e9e-119">分子は分母となる以下にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="46e9e-119">The numerator must be equal to or less than the denominator.</span></span> <span data-ttu-id="46e9e-120">この属性は、0 以上である整数値を表す必要があります。</span><span class="sxs-lookup"><span data-stu-id="46e9e-120">This attribute must represent an integral value that is equal to or greater than zero.</span></span> <span data-ttu-id="46e9e-121">詳細については、このトピックの後半の「解説」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="46e9e-121">For more information, see Remarks later in this topic.</span></span>  <br/> |
|<span data-ttu-id="46e9e-122">**分母**</span><span class="sxs-lookup"><span data-stu-id="46e9e-122">**Denominator**</span></span> <br/> |<span data-ttu-id="46e9e-123">結果セット内のフォルダーの合計数の先頭からのオフセットを表す分数の分母を表します。</span><span class="sxs-lookup"><span data-stu-id="46e9e-123">Represents the denominator of the fractional offset from the start of the total number of folders in the result set.</span></span> <span data-ttu-id="46e9e-124">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="46e9e-124">This attribute is required.</span></span> <span data-ttu-id="46e9e-125">この属性が 1 より大きい整数値を表す必要があります。</span><span class="sxs-lookup"><span data-stu-id="46e9e-125">This attribute must represent an integral value that is greater than one.</span></span> <span data-ttu-id="46e9e-126">詳細については、このトピックの後半の「解説」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="46e9e-126">For more information, see Remarks later in this topic.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="46e9e-127">子要素</span><span class="sxs-lookup"><span data-stu-id="46e9e-127">Child elements</span></span>

<span data-ttu-id="46e9e-128">なし。</span><span class="sxs-lookup"><span data-stu-id="46e9e-128">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="46e9e-129">親要素</span><span class="sxs-lookup"><span data-stu-id="46e9e-129">Parent elements</span></span>

|<span data-ttu-id="46e9e-130">**要素**</span><span class="sxs-lookup"><span data-stu-id="46e9e-130">**Element**</span></span>|<span data-ttu-id="46e9e-131">**説明**</span><span class="sxs-lookup"><span data-stu-id="46e9e-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="46e9e-132">FindFolder</span><span class="sxs-lookup"><span data-stu-id="46e9e-132">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="46e9e-133">メールボックス内のフォルダーを識別するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="46e9e-133">Defines a request to identify folders in a mailbox.</span></span>  <br/> <span data-ttu-id="46e9e-134">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="46e9e-134">The following is the XPath expression to this element:</span></span>  <br/>  `/FindFolder` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="46e9e-135">備考</span><span class="sxs-lookup"><span data-stu-id="46e9e-135">Remarks</span></span>

<span data-ttu-id="46e9e-136">検出されたフォルダーのセットの先頭からのページ ビュー オフセットは、分数で表されます。</span><span class="sxs-lookup"><span data-stu-id="46e9e-136">The paged view offset from the start of the set of found folders is described by a fraction.</span></span> <span data-ttu-id="46e9e-137">分数の**分子**と**分母**の属性によって定義されているは、情報のページを開始する位置について説明します。</span><span class="sxs-lookup"><span data-stu-id="46e9e-137">The fraction, which is defined by the **Numerator** and **Denominator** attributes, describes where the page of information starts.</span></span> <span data-ttu-id="46e9e-138">などの**分子**が 4 と等しいし、**分母**を"5"と等しい、エントリで返される情報の開始ページには 5 分の 4 つの結果セットにする方法が配置されています。</span><span class="sxs-lookup"><span data-stu-id="46e9e-138">For example, if **Numerator** equals four and **Denominator** equals five, the page of returned information starts at an entry located four-fifths of the way in to the result set.</span></span> 
  
<span data-ttu-id="46e9e-139">割合は、0 に評価されると、結果セットの先頭を示します。</span><span class="sxs-lookup"><span data-stu-id="46e9e-139">If the fraction evaluates to zero, that indicates the start of the results set.</span></span> <span data-ttu-id="46e9e-140">分数を 1 つに評価する場合、結果セットの末尾を示します。</span><span class="sxs-lookup"><span data-stu-id="46e9e-140">If the fraction evaluates to one, that indicates the end of the result set.</span></span>
  
> [!NOTE]
> <span data-ttu-id="46e9e-141">分数は、ページの開始位置を表す、結果セットにどのように多くの結果が返されます。</span><span class="sxs-lookup"><span data-stu-id="46e9e-141">The fraction represents the start point of page, not how many results in the result set will be returned.</span></span> 
  
<span data-ttu-id="46e9e-142">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="46e9e-142">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="46e9e-143">要素情報</span><span class="sxs-lookup"><span data-stu-id="46e9e-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="46e9e-144">名前空間</span><span class="sxs-lookup"><span data-stu-id="46e9e-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="46e9e-145">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="46e9e-145">Schema Name</span></span>  <br/> |<span data-ttu-id="46e9e-146">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="46e9e-146">Messages schema</span></span>  <br/> |
|<span data-ttu-id="46e9e-147">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="46e9e-147">Validation File</span></span>  <br/> |<span data-ttu-id="46e9e-148">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="46e9e-148">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="46e9e-149">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="46e9e-149">Can be Empty</span></span>  <br/> |<span data-ttu-id="46e9e-150">False</span><span class="sxs-lookup"><span data-stu-id="46e9e-150">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="46e9e-151">関連項目</span><span class="sxs-lookup"><span data-stu-id="46e9e-151">See also</span></span>



<span data-ttu-id="46e9e-152">
  [FindFolder 操作](findfolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="46e9e-152">[FindFolder operation](findfolder-operation.md)</span></span>


[<span data-ttu-id="46e9e-153">フォルダーを検索します。</span><span class="sxs-lookup"><span data-stu-id="46e9e-153">Finding Folders</span></span>](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

