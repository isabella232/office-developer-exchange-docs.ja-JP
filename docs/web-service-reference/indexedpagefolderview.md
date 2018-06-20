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
description: IndexedPageFolderView 要素がどのようにページングされたアイテム情報を説明 FindFolder 応答が返されます。
ms.openlocfilehash: f32f778daa6fa3fea93ab2bc1951f2407dcf7f80
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831910"
---
# <a name="indexedpagefolderview"></a><span data-ttu-id="303fb-103">IndexedPageFolderView</span><span class="sxs-lookup"><span data-stu-id="303fb-103">IndexedPageFolderView</span></span>

<span data-ttu-id="303fb-104">**IndexedPageFolderView**要素がどのようにページングされたアイテム情報を説明[FindFolder](findfolder.md)応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="303fb-104">The **IndexedPageFolderView** element describes how paged item information is returned in a [FindFolder](findfolder.md) response.</span></span> 
  
[<span data-ttu-id="303fb-105">FindFolder</span><span class="sxs-lookup"><span data-stu-id="303fb-105">FindFolder</span></span>](findfolder.md)
  
[<span data-ttu-id="303fb-106">IndexedPageFolderView</span><span class="sxs-lookup"><span data-stu-id="303fb-106">IndexedPageFolderView</span></span>](indexedpagefolderview.md)
  
```xml
<IndexedPageFolderView MaxEntriesReturned="" Offset="" BasePoint="" />
```

 <span data-ttu-id="303fb-107">**IndexedPageViewType**</span><span class="sxs-lookup"><span data-stu-id="303fb-107">**IndexedPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="303fb-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="303fb-108">Attributes and elements</span></span>

<span data-ttu-id="303fb-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="303fb-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="303fb-110">属性</span><span class="sxs-lookup"><span data-stu-id="303fb-110">Attributes</span></span>

|<span data-ttu-id="303fb-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="303fb-111">**Attribute**</span></span>|<span data-ttu-id="303fb-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="303fb-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="303fb-113">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="303fb-113">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="303fb-114">応答を取得するフォルダーの最大数について説明します。</span><span class="sxs-lookup"><span data-stu-id="303fb-114">Describes the maximum number of folders to return in the response.</span></span> <span data-ttu-id="303fb-115">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="303fb-115">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="303fb-116">**Offset**</span><span class="sxs-lookup"><span data-stu-id="303fb-116">**Offset**</span></span> <br/> |<span data-ttu-id="303fb-117">**ベース ポイント**からのオフセットを示します。</span><span class="sxs-lookup"><span data-stu-id="303fb-117">Describes the offset from the **BasePoint**.</span></span> <span data-ttu-id="303fb-118">オフセットは、0 以上である必要があります。</span><span class="sxs-lookup"><span data-stu-id="303fb-118">Offset must be greater than or equal to zero.</span></span> <span data-ttu-id="303fb-119">**ベース ポイント**と等しい場合、開始オフセットが正の数値です。</span><span class="sxs-lookup"><span data-stu-id="303fb-119">If **BasePoint** is equal to Beginning, the offset is positive.</span></span> <span data-ttu-id="303fb-120">**ベース ポイント**が終了する場合、オフセットが負の場合と処理されます。</span><span class="sxs-lookup"><span data-stu-id="303fb-120">If **BasePoint** is equal to End, the offset is handled as if it were negative.</span></span>  <br/> <span data-ttu-id="303fb-121">これを識別するフォルダーは、応答で配信される最初のフォルダーになります。</span><span class="sxs-lookup"><span data-stu-id="303fb-121">This identifies which folder will be the first folder delivered in the response.</span></span> <span data-ttu-id="303fb-122">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="303fb-122">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="303fb-123">**ベース ポイント**</span><span class="sxs-lookup"><span data-stu-id="303fb-123">**BasePoint**</span></span> <br/> |<span data-ttu-id="303fb-124">フォルダーのページを開始または検索条件で検出されたフォルダーのセットの末尾から開始されるかどうかについて説明します。</span><span class="sxs-lookup"><span data-stu-id="303fb-124">Describes whether the page of folders will start from the start or the end of the set of folders that are found with the search criteria.</span></span> <span data-ttu-id="303fb-125">末尾からのシークを常に検索を進めます。</span><span class="sxs-lookup"><span data-stu-id="303fb-125">Seeking from the end always searches backward.</span></span> <span data-ttu-id="303fb-126">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="303fb-126">This attribute is required.</span></span>  <br/> |
   
#### <a name="basepoint-attribute"></a><span data-ttu-id="303fb-127">ベース ポイントの属性</span><span class="sxs-lookup"><span data-stu-id="303fb-127">BasePoint Attribute</span></span>

|<span data-ttu-id="303fb-128">**値**</span><span class="sxs-lookup"><span data-stu-id="303fb-128">**Value**</span></span>|<span data-ttu-id="303fb-129">**説明**</span><span class="sxs-lookup"><span data-stu-id="303fb-129">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="303fb-130">先頭</span><span class="sxs-lookup"><span data-stu-id="303fb-130">Beginning</span></span>  <br/> |<span data-ttu-id="303fb-131">ページ ビューは、検索フォルダーのセットの先頭から開始されます。</span><span class="sxs-lookup"><span data-stu-id="303fb-131">The paged view starts at the beginning of the found folder set.</span></span>  <br/> |
|<span data-ttu-id="303fb-132">終了</span><span class="sxs-lookup"><span data-stu-id="303fb-132">End</span></span>  <br/> |<span data-ttu-id="303fb-133">ページ ビューは、検索フォルダーのセットの末尾から開始します。</span><span class="sxs-lookup"><span data-stu-id="303fb-133">The paged view starts at the end of the found folder set.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="303fb-134">子要素</span><span class="sxs-lookup"><span data-stu-id="303fb-134">Child elements</span></span>

<span data-ttu-id="303fb-135">なし。</span><span class="sxs-lookup"><span data-stu-id="303fb-135">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="303fb-136">親要素</span><span class="sxs-lookup"><span data-stu-id="303fb-136">Parent elements</span></span>

|<span data-ttu-id="303fb-137">**要素**</span><span class="sxs-lookup"><span data-stu-id="303fb-137">**Element**</span></span>|<span data-ttu-id="303fb-138">**説明**</span><span class="sxs-lookup"><span data-stu-id="303fb-138">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="303fb-139">FindFolder</span><span class="sxs-lookup"><span data-stu-id="303fb-139">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="303fb-140">メールボックス内のフォルダーを検索するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="303fb-140">Defines a request to find folders in a mailbox.</span></span>  <br/> <span data-ttu-id="303fb-141">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="303fb-141">The following is the XPath expression to this element:</span></span>  <br/>  `/FindFolder` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="303fb-142">備考</span><span class="sxs-lookup"><span data-stu-id="303fb-142">Remarks</span></span>

<span data-ttu-id="303fb-143">末尾からのシークでは、オフセットによって識別される原点に移動します。</span><span class="sxs-lookup"><span data-stu-id="303fb-143">Seeking from end involves moving to the origin identified by the offset.</span></span> <span data-ttu-id="303fb-144">さらに、ポインターが再び要求されたレコードの数によって。</span><span class="sxs-lookup"><span data-stu-id="303fb-144">Additionally, the pointer is moved back by the number of requested records.</span></span> <span data-ttu-id="303fb-145">などの場合は 100 個のレコードがある、オフセットが末尾から 25、75 から検索を開始します。</span><span class="sxs-lookup"><span data-stu-id="303fb-145">For example, if there are 100 records and the offset is 25 from the end, the search starts from 75.</span></span> <span data-ttu-id="303fb-146">10 個のレコードが返された場合ポインターが逆方向、さらに 10 が 65 を記録し、65 75 からのレコードを返します。</span><span class="sxs-lookup"><span data-stu-id="303fb-146">If 10 records are returned, the pointer is moved backward an additional 10 records to 65 and returns records 65 through 75.</span></span> <span data-ttu-id="303fb-147">次のインデックスは、64 です。</span><span class="sxs-lookup"><span data-stu-id="303fb-147">The next index is 64.</span></span> <span data-ttu-id="303fb-148">ページの末尾からの次のオフセットは、100-36 に相当する 64 です。</span><span class="sxs-lookup"><span data-stu-id="303fb-148">The next offset from the end for a page is 100 minus 64 which equals 36.</span></span> <span data-ttu-id="303fb-149">次のインデックス付きのページを取得する、末尾からの次のオフセットの値は、36 です。</span><span class="sxs-lookup"><span data-stu-id="303fb-149">The value for the next offset from the end to get the next indexed page is 36.</span></span>
  
<span data-ttu-id="303fb-150">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="303fb-150">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="303fb-151">要素情報</span><span class="sxs-lookup"><span data-stu-id="303fb-151">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="303fb-152">名前空間</span><span class="sxs-lookup"><span data-stu-id="303fb-152">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="303fb-153">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="303fb-153">Schema Name</span></span>  <br/> |<span data-ttu-id="303fb-154">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="303fb-154">Messages schema</span></span>  <br/> |
|<span data-ttu-id="303fb-155">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="303fb-155">Validation File</span></span>  <br/> |<span data-ttu-id="303fb-156">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="303fb-156">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="303fb-157">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="303fb-157">Can be Empty</span></span>  <br/> |<span data-ttu-id="303fb-158">いいえ</span><span class="sxs-lookup"><span data-stu-id="303fb-158">False</span></span>  <br/> |
   

