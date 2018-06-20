---
title: RootFolder (FindFolderResponseMessage)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RootFolder
api_type:
- schema
ms.assetid: 5089c815-663f-46be-bc59-aed9ee20f94a
description: RootFolder 要素には、FindFolder 操作中に単一のルート フォルダーの検索の結果が含まれています。
ms.openlocfilehash: 1cd79d5fa34318e7fe29606df84cbf0ef0520b93
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833253"
---
# <a name="rootfolder-findfolderresponsemessage"></a><span data-ttu-id="60e0d-103">RootFolder (FindFolderResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="60e0d-103">RootFolder (FindFolderResponseMessage)</span></span>

<span data-ttu-id="60e0d-104">**RootFolder**要素には、 [FindFolder 操作](findfolder-operation.md)中に単一のルート フォルダーの検索の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="60e0d-104">The **RootFolder** element contains the results of a search of a single root folder during a [FindFolder operation](findfolder-operation.md).</span></span>
  
```xml
<RootFolder IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Folders/>
</RootFolder>
```

 <span data-ttu-id="60e0d-105">**FindFolderParentType**</span><span class="sxs-lookup"><span data-stu-id="60e0d-105">**FindFolderParentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="60e0d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="60e0d-106">Attributes and elements</span></span>

<span data-ttu-id="60e0d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="60e0d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="60e0d-108">属性</span><span class="sxs-lookup"><span data-stu-id="60e0d-108">Attributes</span></span>

|<span data-ttu-id="60e0d-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="60e0d-109">**Attribute**</span></span>|<span data-ttu-id="60e0d-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="60e0d-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="60e0d-111">IndexedPagingOffset</span><span class="sxs-lookup"><span data-stu-id="60e0d-111">IndexedPagingOffset</span></span>  <br/> |<span data-ttu-id="60e0d-112">インデックス付きページング ビューを使用する場合、次の要求に使用する必要があります次のインデックスを表します。</span><span class="sxs-lookup"><span data-stu-id="60e0d-112">Represents the next index that should be used for the next request when using an indexed paging view.</span></span>  <br/> |
|<span data-ttu-id="60e0d-113">NumeratorOffset</span><span class="sxs-lookup"><span data-stu-id="60e0d-113">NumeratorOffset</span></span>  <br/> |<span data-ttu-id="60e0d-114">分数のページ ビューを使用する場合は、次の要求に使用する新しい分子の値を表します。</span><span class="sxs-lookup"><span data-stu-id="60e0d-114">Represents the new numerator value to use for the next request when using fractional page views.</span></span>  <br/> |
|<span data-ttu-id="60e0d-115">AbsoluteDenominator</span><span class="sxs-lookup"><span data-stu-id="60e0d-115">AbsoluteDenominator</span></span>  <br/> |<span data-ttu-id="60e0d-116">分数形式のページングを実行する場合、次の要求に使用する分母を表します。</span><span class="sxs-lookup"><span data-stu-id="60e0d-116">Represents the next denominator to use for the next request when doing fractional paging.</span></span>  <br/> |
|<span data-ttu-id="60e0d-117">IncludesLastItemInRange</span><span class="sxs-lookup"><span data-stu-id="60e0d-117">IncludesLastItemInRange</span></span>  <br/> |<span data-ttu-id="60e0d-118">さらにページングが必要ないように、現在の結果が、クエリ内の最後のフォルダーを含めるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="60e0d-118">Indicates whether the current results contain the last folder in the query, such that further paging is not needed.</span></span>  <br/> |
|<span data-ttu-id="60e0d-119">TotalItemsInView</span><span class="sxs-lookup"><span data-stu-id="60e0d-119">TotalItemsInView</span></span>  <br/> |<span data-ttu-id="60e0d-120">制限を満たすフォルダーの総数を表します。</span><span class="sxs-lookup"><span data-stu-id="60e0d-120">Represents the total number of folders that pass the restriction.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="60e0d-121">子要素</span><span class="sxs-lookup"><span data-stu-id="60e0d-121">Child elements</span></span>

|<span data-ttu-id="60e0d-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="60e0d-122">**Element**</span></span>|<span data-ttu-id="60e0d-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="60e0d-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="60e0d-124">フォルダー</span><span class="sxs-lookup"><span data-stu-id="60e0d-124">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="60e0d-125">[FindFolder 操作](findfolder-operation.md)を使用してフォルダーの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="60e0d-125">Contains an array of folders found by using the [FindFolder operation](findfolder-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="60e0d-126">親要素</span><span class="sxs-lookup"><span data-stu-id="60e0d-126">Parent elements</span></span>

|<span data-ttu-id="60e0d-127">**要素**</span><span class="sxs-lookup"><span data-stu-id="60e0d-127">**Element**</span></span>|<span data-ttu-id="60e0d-128">**説明**</span><span class="sxs-lookup"><span data-stu-id="60e0d-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="60e0d-129">FindFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="60e0d-129">FindFolderResponseMessage</span></span>](findfolderresponsemessage.md) <br/> |<span data-ttu-id="60e0d-130">[FindFolder 操作](findfolder-operation.md)要求の結果ステータスを格納します。</span><span class="sxs-lookup"><span data-stu-id="60e0d-130">Contains the status and result of a [FindFolder operation](findfolder-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="60e0d-131">備考</span><span class="sxs-lookup"><span data-stu-id="60e0d-131">Remarks</span></span>

<span data-ttu-id="60e0d-132">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="60e0d-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="60e0d-133">要素情報</span><span class="sxs-lookup"><span data-stu-id="60e0d-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="60e0d-134">名前空間</span><span class="sxs-lookup"><span data-stu-id="60e0d-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="60e0d-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="60e0d-135">Schema name</span></span>  <br/> |<span data-ttu-id="60e0d-136">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="60e0d-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="60e0d-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="60e0d-137">Validation file</span></span>  <br/> |<span data-ttu-id="60e0d-138">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="60e0d-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="60e0d-139">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="60e0d-139">Can be empty</span></span>  <br/> |<span data-ttu-id="60e0d-140">False</span><span class="sxs-lookup"><span data-stu-id="60e0d-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="60e0d-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="60e0d-141">See also</span></span>



<span data-ttu-id="60e0d-142">
  [FindFolder 操作](findfolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="60e0d-142">[FindFolder operation](findfolder-operation.md)</span></span>


[<span data-ttu-id="60e0d-143">フォルダーを検索します。</span><span class="sxs-lookup"><span data-stu-id="60e0d-143">Finding Folders</span></span>](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

