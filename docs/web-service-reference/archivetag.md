---
title: ArchiveTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c4cb0718-37cd-41aa-86e7-b492c4bb86aa
description: アーカイブタグ要素は、アイテムまたはフォルダーに設定されているアーカイブタグセットの保持識別子を指定します。
ms.openlocfilehash: 23167f3c96a6756fe4c6d915a4de91e815e620d9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464764"
---
# <a name="archivetag"></a><span data-ttu-id="4d20c-103">ArchiveTag</span><span class="sxs-lookup"><span data-stu-id="4d20c-103">ArchiveTag</span></span>

<span data-ttu-id="4d20c-104">アーカイブ**タグ要素は、アイテム**またはフォルダーに設定されているアーカイブタグセットの保持識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="4d20c-104">The **ArchiveTag** element specifies the retention identifier of the archive tag set on an item or folder.</span></span> 
  
```XML
<ArchiveTag IsExplicit=""></ArchiveTag>
```

 <span data-ttu-id="4d20c-105">**RetentionTagType**</span><span class="sxs-lookup"><span data-stu-id="4d20c-105">**RetentionTagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4d20c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="4d20c-106">Attributes and elements</span></span>

<span data-ttu-id="4d20c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4d20c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4d20c-108">属性</span><span class="sxs-lookup"><span data-stu-id="4d20c-108">Attributes</span></span>

|<span data-ttu-id="4d20c-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="4d20c-109">**Attribute**</span></span>|<span data-ttu-id="4d20c-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="4d20c-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4d20c-111">**IsExplicit**</span><span class="sxs-lookup"><span data-stu-id="4d20c-111">**IsExplicit**</span></span> <br/> |<span data-ttu-id="4d20c-112">アイテムまたはフォルダーにアイテム保持ポリシーを明示的に設定するかどうか、または親フォルダーから継承するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="4d20c-112">Specifies whether the retention policy is explicitly set on an item or folder or whether it is inherited from a parent folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4d20c-113">子要素</span><span class="sxs-lookup"><span data-stu-id="4d20c-113">Child elements</span></span>

<span data-ttu-id="4d20c-114">なし。</span><span class="sxs-lookup"><span data-stu-id="4d20c-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4d20c-115">親要素</span><span class="sxs-lookup"><span data-stu-id="4d20c-115">Parent elements</span></span>

|<span data-ttu-id="4d20c-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="4d20c-116">**Element**</span></span>|<span data-ttu-id="4d20c-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="4d20c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4d20c-118">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="4d20c-118">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="4d20c-119">主に予定表アイテムを含むフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="4d20c-119">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="4d20c-120">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="4d20c-120">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="4d20c-121">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="4d20c-121">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="4d20c-122">Contact</span><span class="sxs-lookup"><span data-stu-id="4d20c-122">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="4d20c-123">Exchange ストア内の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="4d20c-123">Represents a contact item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="4d20c-124">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="4d20c-124">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="4d20c-125">メールボックスに含まれている連絡先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="4d20c-125">Represents a contacts folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="4d20c-126">DistributionList</span><span class="sxs-lookup"><span data-stu-id="4d20c-126">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="4d20c-127">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="4d20c-127">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="4d20c-128">Folder</span><span class="sxs-lookup"><span data-stu-id="4d20c-128">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="4d20c-129">作成、取得、検索、同期、更新を行うフォルダーを定義します。</span><span class="sxs-lookup"><span data-stu-id="4d20c-129">Defines a folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="4d20c-130">Item</span><span class="sxs-lookup"><span data-stu-id="4d20c-130">Item</span></span>](item.md) <br/> |<span data-ttu-id="4d20c-131">Exchange ストア内の汎用アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="4d20c-131">Represents a generic item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="4d20c-132">Message</span><span class="sxs-lookup"><span data-stu-id="4d20c-132">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="4d20c-133">Microsoft Exchange の電子メールメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="4d20c-133">Represents a Microsoft Exchange email message.</span></span>  <br/> |
|[<span data-ttu-id="4d20c-134">PostItem</span><span class="sxs-lookup"><span data-stu-id="4d20c-134">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="4d20c-135">Exchange ストア内の投稿アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="4d20c-135">Represents a post item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="4d20c-136">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="4d20c-136">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="4d20c-137">メールボックスに含まれている検索フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="4d20c-137">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="4d20c-138">タスク</span><span class="sxs-lookup"><span data-stu-id="4d20c-138">Task</span></span>](task.md) <br/> |<span data-ttu-id="4d20c-139">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="4d20c-139">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="4d20c-140">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="4d20c-140">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="4d20c-141">メールボックスに含まれる tasks フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="4d20c-141">Represents a tasks folder that is contained in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4d20c-142">テキスト値</span><span class="sxs-lookup"><span data-stu-id="4d20c-142">Text value</span></span>

<span data-ttu-id="4d20c-143">**アーカイブタグ**要素のテキスト値は、アイテム保持ポリシーを識別する GUID です。</span><span class="sxs-lookup"><span data-stu-id="4d20c-143">The text value of the **ArchiveTag** element is a GUID that identifies the retention policy.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="4d20c-144">注釈</span><span class="sxs-lookup"><span data-stu-id="4d20c-144">Remarks</span></span>

<span data-ttu-id="4d20c-145">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="4d20c-145">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4d20c-146">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="4d20c-146">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4d20c-147">要素の情報</span><span class="sxs-lookup"><span data-stu-id="4d20c-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4d20c-148">Namespace</span><span class="sxs-lookup"><span data-stu-id="4d20c-148">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4d20c-149">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4d20c-149">Schema Name</span></span>  <br/> |<span data-ttu-id="4d20c-150">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="4d20c-150">Type schema</span></span>  <br/> |
|<span data-ttu-id="4d20c-151">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4d20c-151">Validation File</span></span>  <br/> |<span data-ttu-id="4d20c-152">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="4d20c-152">types.xsd</span></span>  <br/> |
|<span data-ttu-id="4d20c-153">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4d20c-153">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="4d20c-154">関連項目</span><span class="sxs-lookup"><span data-stu-id="4d20c-154">See also</span></span>

- [<span data-ttu-id="4d20c-155">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="4d20c-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

