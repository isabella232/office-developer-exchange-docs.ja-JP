---
title: IndexedPageFolderView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IndexedPageFolderView
api_type:
- schema
ms.assetid: c6dac232-244b-4db0-9a15-5e01b8aa7a7d
description: IndexedPageFolderView 要素は、ページアイテムの情報が FindFolder 応答で返される方法を記述します。
ms.openlocfilehash: 6e9e2796c0bdcd9a15487f0e1bc7cbdf09d0a492
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457201"
---
# <a name="indexedpagefolderview"></a><span data-ttu-id="44d4b-103">IndexedPageFolderView</span><span class="sxs-lookup"><span data-stu-id="44d4b-103">IndexedPageFolderView</span></span>

<span data-ttu-id="44d4b-104">**Indexedpagefolderview**要素は、ページアイテムの情報が[findfolder](findfolder.md)応答で返される方法を記述します。</span><span class="sxs-lookup"><span data-stu-id="44d4b-104">The **IndexedPageFolderView** element describes how paged item information is returned in a [FindFolder](findfolder.md) response.</span></span> 
  
[<span data-ttu-id="44d4b-105">FindFolder</span><span class="sxs-lookup"><span data-stu-id="44d4b-105">FindFolder</span></span>](findfolder.md)
  
[<span data-ttu-id="44d4b-106">IndexedPageFolderView</span><span class="sxs-lookup"><span data-stu-id="44d4b-106">IndexedPageFolderView</span></span>](indexedpagefolderview.md)
  
```xml
<IndexedPageFolderView MaxEntriesReturned="" Offset="" BasePoint="" />
```

 <span data-ttu-id="44d4b-107">**IndexedPageViewType**</span><span class="sxs-lookup"><span data-stu-id="44d4b-107">**IndexedPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="44d4b-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="44d4b-108">Attributes and elements</span></span>

<span data-ttu-id="44d4b-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="44d4b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="44d4b-110">属性</span><span class="sxs-lookup"><span data-stu-id="44d4b-110">Attributes</span></span>

|<span data-ttu-id="44d4b-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="44d4b-111">**Attribute**</span></span>|<span data-ttu-id="44d4b-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="44d4b-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="44d4b-113">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="44d4b-113">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="44d4b-114">応答で返されるフォルダーの最大数を表します。</span><span class="sxs-lookup"><span data-stu-id="44d4b-114">Describes the maximum number of folders to return in the response.</span></span> <span data-ttu-id="44d4b-115">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="44d4b-115">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="44d4b-116">**Offset**</span><span class="sxs-lookup"><span data-stu-id="44d4b-116">**Offset**</span></span> <br/> |<span data-ttu-id="44d4b-117">**BasePoint**からのオフセットを記述します。</span><span class="sxs-lookup"><span data-stu-id="44d4b-117">Describes the offset from the **BasePoint**.</span></span> <span data-ttu-id="44d4b-118">オフセットは0以上である必要があります。</span><span class="sxs-lookup"><span data-stu-id="44d4b-118">Offset must be greater than or equal to zero.</span></span> <span data-ttu-id="44d4b-119">**BasePoint**が先頭と等しい場合、オフセットは正になります。</span><span class="sxs-lookup"><span data-stu-id="44d4b-119">If **BasePoint** is equal to Beginning, the offset is positive.</span></span> <span data-ttu-id="44d4b-120">**BasePoint**が End と等しい場合、オフセットは負の値として処理されます。</span><span class="sxs-lookup"><span data-stu-id="44d4b-120">If **BasePoint** is equal to End, the offset is handled as if it were negative.</span></span>  <br/> <span data-ttu-id="44d4b-121">これにより、どのフォルダーが応答で配信される最初のフォルダーになるかを識別します。</span><span class="sxs-lookup"><span data-stu-id="44d4b-121">This identifies which folder will be the first folder delivered in the response.</span></span> <span data-ttu-id="44d4b-122">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="44d4b-122">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="44d4b-123">**BasePoint**</span><span class="sxs-lookup"><span data-stu-id="44d4b-123">**BasePoint**</span></span> <br/> |<span data-ttu-id="44d4b-124">フォルダーのページが検索条件に一致する一連のフォルダーの先頭から開始するか、または末尾から開始するかを指定します。</span><span class="sxs-lookup"><span data-stu-id="44d4b-124">Describes whether the page of folders will start from the start or the end of the set of folders that are found with the search criteria.</span></span> <span data-ttu-id="44d4b-125">末尾からシークすると、常に逆方向に検索されます。</span><span class="sxs-lookup"><span data-stu-id="44d4b-125">Seeking from the end always searches backward.</span></span> <span data-ttu-id="44d4b-126">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="44d4b-126">This attribute is required.</span></span>  <br/> |
   
#### <a name="basepoint-attribute"></a><span data-ttu-id="44d4b-127">BasePoint 属性</span><span class="sxs-lookup"><span data-stu-id="44d4b-127">BasePoint Attribute</span></span>

|<span data-ttu-id="44d4b-128">**値**</span><span class="sxs-lookup"><span data-stu-id="44d4b-128">**Value**</span></span>|<span data-ttu-id="44d4b-129">**説明**</span><span class="sxs-lookup"><span data-stu-id="44d4b-129">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="44d4b-130">始まる</span><span class="sxs-lookup"><span data-stu-id="44d4b-130">Beginning</span></span>  <br/> |<span data-ttu-id="44d4b-131">ページビューは、見つかったフォルダーセットの先頭から開始されます。</span><span class="sxs-lookup"><span data-stu-id="44d4b-131">The paged view starts at the beginning of the found folder set.</span></span>  <br/> |
|<span data-ttu-id="44d4b-132">End</span><span class="sxs-lookup"><span data-stu-id="44d4b-132">End</span></span>  <br/> |<span data-ttu-id="44d4b-133">ページビューは、見つかったフォルダーセットの末尾から開始されます。</span><span class="sxs-lookup"><span data-stu-id="44d4b-133">The paged view starts at the end of the found folder set.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="44d4b-134">子要素</span><span class="sxs-lookup"><span data-stu-id="44d4b-134">Child elements</span></span>

<span data-ttu-id="44d4b-135">なし。</span><span class="sxs-lookup"><span data-stu-id="44d4b-135">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="44d4b-136">親要素</span><span class="sxs-lookup"><span data-stu-id="44d4b-136">Parent elements</span></span>

|<span data-ttu-id="44d4b-137">**要素**</span><span class="sxs-lookup"><span data-stu-id="44d4b-137">**Element**</span></span>|<span data-ttu-id="44d4b-138">**説明**</span><span class="sxs-lookup"><span data-stu-id="44d4b-138">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="44d4b-139">FindFolder</span><span class="sxs-lookup"><span data-stu-id="44d4b-139">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="44d4b-140">メールボックス内のフォルダーを検索する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="44d4b-140">Defines a request to find folders in a mailbox.</span></span>  <br/> <span data-ttu-id="44d4b-141">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="44d4b-141">The following is the XPath expression to this element:</span></span>  <br/>  `/FindFolder` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="44d4b-142">注釈</span><span class="sxs-lookup"><span data-stu-id="44d4b-142">Remarks</span></span>

<span data-ttu-id="44d4b-143">End からシークするには、オフセットで識別される起点に移動する必要があります。</span><span class="sxs-lookup"><span data-stu-id="44d4b-143">Seeking from end involves moving to the origin identified by the offset.</span></span> <span data-ttu-id="44d4b-144">さらに、要求されたレコードの数だけポインターが戻されます。</span><span class="sxs-lookup"><span data-stu-id="44d4b-144">Additionally, the pointer is moved back by the number of requested records.</span></span> <span data-ttu-id="44d4b-145">たとえば、100レコードがあり、オフセットが最後から25である場合、検索は75から開始されます。</span><span class="sxs-lookup"><span data-stu-id="44d4b-145">For example, if there are 100 records and the offset is 25 from the end, the search starts from 75.</span></span> <span data-ttu-id="44d4b-146">10件のレコードが返された場合、ポインターは10レコード後ろに65に移動され、レコード 65 ~ 75 を返します。</span><span class="sxs-lookup"><span data-stu-id="44d4b-146">If 10 records are returned, the pointer is moved backward an additional 10 records to 65 and returns records 65 through 75.</span></span> <span data-ttu-id="44d4b-147">次のインデックスは64です。</span><span class="sxs-lookup"><span data-stu-id="44d4b-147">The next index is 64.</span></span> <span data-ttu-id="44d4b-148">ページの最後からの次のオフセットは、36と等しい 100-64 です。</span><span class="sxs-lookup"><span data-stu-id="44d4b-148">The next offset from the end for a page is 100 minus 64 which equals 36.</span></span> <span data-ttu-id="44d4b-149">次のインデックス付きページを取得するために、末尾からの次のオフセットの値は36です。</span><span class="sxs-lookup"><span data-stu-id="44d4b-149">The value for the next offset from the end to get the next indexed page is 36.</span></span>
  
<span data-ttu-id="44d4b-150">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="44d4b-150">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="44d4b-151">要素の情報</span><span class="sxs-lookup"><span data-stu-id="44d4b-151">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="44d4b-152">Namespace</span><span class="sxs-lookup"><span data-stu-id="44d4b-152">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="44d4b-153">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="44d4b-153">Schema Name</span></span>  <br/> |<span data-ttu-id="44d4b-154">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="44d4b-154">Messages schema</span></span>  <br/> |
|<span data-ttu-id="44d4b-155">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="44d4b-155">Validation File</span></span>  <br/> |<span data-ttu-id="44d4b-156">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="44d4b-156">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="44d4b-157">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="44d4b-157">Can be Empty</span></span>  <br/> |<span data-ttu-id="44d4b-158">いいえ</span><span class="sxs-lookup"><span data-stu-id="44d4b-158">False</span></span>  <br/> |
   

