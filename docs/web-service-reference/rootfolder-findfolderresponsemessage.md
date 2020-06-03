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
description: RootFolder 要素には、FindFolder 操作中の1つのルートフォルダーの検索結果が含まれています。
ms.openlocfilehash: b5601d6abec67196c9991908e272a2122a201d69
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457138"
---
# <a name="rootfolder-findfolderresponsemessage"></a><span data-ttu-id="602c1-103">RootFolder (FindFolderResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="602c1-103">RootFolder (FindFolderResponseMessage)</span></span>

<span data-ttu-id="602c1-104">**RootFolder**要素には、 [findfolder 操作](findfolder-operation.md)中の1つのルートフォルダーの検索結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="602c1-104">The **RootFolder** element contains the results of a search of a single root folder during a [FindFolder operation](findfolder-operation.md).</span></span>
  
```xml
<RootFolder IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Folders/>
</RootFolder>
```

 <span data-ttu-id="602c1-105">**FindFolderParentType**</span><span class="sxs-lookup"><span data-stu-id="602c1-105">**FindFolderParentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="602c1-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="602c1-106">Attributes and elements</span></span>

<span data-ttu-id="602c1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="602c1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="602c1-108">属性</span><span class="sxs-lookup"><span data-stu-id="602c1-108">Attributes</span></span>

|<span data-ttu-id="602c1-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="602c1-109">**Attribute**</span></span>|<span data-ttu-id="602c1-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="602c1-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="602c1-111">IndexedPagingOffset</span><span class="sxs-lookup"><span data-stu-id="602c1-111">IndexedPagingOffset</span></span>  <br/> |<span data-ttu-id="602c1-112">インデックス付きページングビューを使用するときに次の要求に使用される次のインデックスを表します。</span><span class="sxs-lookup"><span data-stu-id="602c1-112">Represents the next index that should be used for the next request when using an indexed paging view.</span></span>  <br/> |
|<span data-ttu-id="602c1-113">NumeratorOffset</span><span class="sxs-lookup"><span data-stu-id="602c1-113">NumeratorOffset</span></span>  <br/> |<span data-ttu-id="602c1-114">分数のページビューを使用する場合に、次の要求に対して使用する新しい分子の値を表します。</span><span class="sxs-lookup"><span data-stu-id="602c1-114">Represents the new numerator value to use for the next request when using fractional page views.</span></span>  <br/> |
|<span data-ttu-id="602c1-115">AbsoluteDenominator</span><span class="sxs-lookup"><span data-stu-id="602c1-115">AbsoluteDenominator</span></span>  <br/> |<span data-ttu-id="602c1-116">分数のページングを行うときに、次の要求に対して使用する次の分母を表します。</span><span class="sxs-lookup"><span data-stu-id="602c1-116">Represents the next denominator to use for the next request when doing fractional paging.</span></span>  <br/> |
|<span data-ttu-id="602c1-117">IncludesLastItemInRange</span><span class="sxs-lookup"><span data-stu-id="602c1-117">IncludesLastItemInRange</span></span>  <br/> |<span data-ttu-id="602c1-118">現在の結果にクエリ内の最後のフォルダーが含まれているかどうかを示します。これは、追加のページングは必要ありません。</span><span class="sxs-lookup"><span data-stu-id="602c1-118">Indicates whether the current results contain the last folder in the query, such that further paging is not needed.</span></span>  <br/> |
|<span data-ttu-id="602c1-119">TotalItemsInView</span><span class="sxs-lookup"><span data-stu-id="602c1-119">TotalItemsInView</span></span>  <br/> |<span data-ttu-id="602c1-120">制限に合格したフォルダーの合計数を表します。</span><span class="sxs-lookup"><span data-stu-id="602c1-120">Represents the total number of folders that pass the restriction.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="602c1-121">子要素</span><span class="sxs-lookup"><span data-stu-id="602c1-121">Child elements</span></span>

|<span data-ttu-id="602c1-122">**Element**</span><span class="sxs-lookup"><span data-stu-id="602c1-122">**Element**</span></span>|<span data-ttu-id="602c1-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="602c1-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="602c1-124">フォルダー</span><span class="sxs-lookup"><span data-stu-id="602c1-124">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="602c1-125">[Findfolder 操作](findfolder-operation.md)を使用して見つかったフォルダーの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="602c1-125">Contains an array of folders found by using the [FindFolder operation](findfolder-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="602c1-126">親要素</span><span class="sxs-lookup"><span data-stu-id="602c1-126">Parent elements</span></span>

|<span data-ttu-id="602c1-127">**要素**</span><span class="sxs-lookup"><span data-stu-id="602c1-127">**Element**</span></span>|<span data-ttu-id="602c1-128">**説明**</span><span class="sxs-lookup"><span data-stu-id="602c1-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="602c1-129">FindFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="602c1-129">FindFolderResponseMessage</span></span>](findfolderresponsemessage.md) <br/> |<span data-ttu-id="602c1-130">[Findfolder 操作](findfolder-operation.md)要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="602c1-130">Contains the status and result of a [FindFolder operation](findfolder-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="602c1-131">注釈</span><span class="sxs-lookup"><span data-stu-id="602c1-131">Remarks</span></span>

<span data-ttu-id="602c1-132">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="602c1-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="602c1-133">要素の情報</span><span class="sxs-lookup"><span data-stu-id="602c1-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="602c1-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="602c1-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="602c1-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="602c1-135">Schema name</span></span>  <br/> |<span data-ttu-id="602c1-136">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="602c1-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="602c1-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="602c1-137">Validation file</span></span>  <br/> |<span data-ttu-id="602c1-138">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="602c1-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="602c1-139">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="602c1-139">Can be empty</span></span>  <br/> |<span data-ttu-id="602c1-140">正しくない</span><span class="sxs-lookup"><span data-stu-id="602c1-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="602c1-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="602c1-141">See also</span></span>



[<span data-ttu-id="602c1-142">FindFolder 操作</span><span class="sxs-lookup"><span data-stu-id="602c1-142">FindFolder operation</span></span>](findfolder-operation.md)


[<span data-ttu-id="602c1-143">フォルダーの検索</span><span class="sxs-lookup"><span data-stu-id="602c1-143">Finding Folders</span></span>](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

