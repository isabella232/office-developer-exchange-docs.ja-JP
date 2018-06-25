---
title: ArchiveTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c4cb0718-37cd-41aa-86e7-b492c4bb86aa
description: ArchiveTag 要素は、アイテムまたはフォルダーの [アーカイブのタグの保存期間の識別子を指定します。
ms.openlocfilehash: ae9c7d512981af3bf564bcb73a9a27c5c78217fc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759435"
---
# <a name="archivetag"></a><span data-ttu-id="fda63-103">ArchiveTag</span><span class="sxs-lookup"><span data-stu-id="fda63-103">ArchiveTag</span></span>

<span data-ttu-id="fda63-104">**ArchiveTag**要素は、アイテムまたはフォルダーの [アーカイブのタグの保存期間の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="fda63-104">The **ArchiveTag** element specifies the retention identifier of the archive tag set on an item or folder.</span></span> 
  
```XML
<ArchiveTag IsExplicit=""></ArchiveTag>
```

 <span data-ttu-id="fda63-105">**RetentionTagType**</span><span class="sxs-lookup"><span data-stu-id="fda63-105">**RetentionTagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fda63-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="fda63-106">Attributes and elements</span></span>

<span data-ttu-id="fda63-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fda63-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fda63-108">属性</span><span class="sxs-lookup"><span data-stu-id="fda63-108">Attributes</span></span>

|<span data-ttu-id="fda63-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="fda63-109">**Attribute**</span></span>|<span data-ttu-id="fda63-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="fda63-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fda63-111">**IsExplicit**</span><span class="sxs-lookup"><span data-stu-id="fda63-111">**IsExplicit**</span></span> <br/> |<span data-ttu-id="fda63-112">アイテムまたはフォルダーにアイテム保持ポリシーを明示的に設定するかどうか、または親フォルダーから継承されているかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="fda63-112">Specifies whether the retention policy is explicitly set on an item or folder or whether it is inherited from a parent folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="fda63-113">子要素</span><span class="sxs-lookup"><span data-stu-id="fda63-113">Child elements</span></span>

<span data-ttu-id="fda63-114">なし。</span><span class="sxs-lookup"><span data-stu-id="fda63-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fda63-115">親要素</span><span class="sxs-lookup"><span data-stu-id="fda63-115">Parent elements</span></span>

|<span data-ttu-id="fda63-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="fda63-116">**Element**</span></span>|<span data-ttu-id="fda63-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="fda63-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fda63-118">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="fda63-118">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="fda63-119">主に予定表のアイテムを含むフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="fda63-119">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="fda63-120">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="fda63-120">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="fda63-121">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="fda63-121">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="fda63-122">Contact</span><span class="sxs-lookup"><span data-stu-id="fda63-122">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="fda63-123">Exchange ストア内の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="fda63-123">Represents a contact item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="fda63-124">メッセージ</span><span class="sxs-lookup"><span data-stu-id="fda63-124">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="fda63-125">メールボックスに格納されている連絡先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="fda63-125">Represents a contacts folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="fda63-126">DistributionList</span><span class="sxs-lookup"><span data-stu-id="fda63-126">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="fda63-127">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="fda63-127">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="fda63-128">Folder</span><span class="sxs-lookup"><span data-stu-id="fda63-128">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="fda63-129">作成、取得、検索、同期、または更新するフォルダーを定義します。</span><span class="sxs-lookup"><span data-stu-id="fda63-129">Defines a folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="fda63-130">アイテム</span><span class="sxs-lookup"><span data-stu-id="fda63-130">Item</span></span>](item.md) <br/> |<span data-ttu-id="fda63-131">Exchange ストア内の一般的な項目を表します。</span><span class="sxs-lookup"><span data-stu-id="fda63-131">Represents a generic item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="fda63-132">Message</span><span class="sxs-lookup"><span data-stu-id="fda63-132">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="fda63-133">Microsoft Exchange の電子メール メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="fda63-133">Represents a Microsoft Exchange email message.</span></span>  <br/> |
|[<span data-ttu-id="fda63-134">PostItem</span><span class="sxs-lookup"><span data-stu-id="fda63-134">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="fda63-135">Exchange ストア内の投稿アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="fda63-135">Represents a post item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="fda63-136">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="fda63-136">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="fda63-137">メールボックスに格納されている検索フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="fda63-137">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="fda63-138">タスク</span><span class="sxs-lookup"><span data-stu-id="fda63-138">Task</span></span>](task.md) <br/> |<span data-ttu-id="fda63-139">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="fda63-139">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="fda63-140">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="fda63-140">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="fda63-141">メールボックスに含まれるタスク フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="fda63-141">Represents a tasks folder that is contained in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fda63-142">テキスト値</span><span class="sxs-lookup"><span data-stu-id="fda63-142">Text value</span></span>

<span data-ttu-id="fda63-143">**ArchiveTag**要素のテキスト値は、保持ポリシーを識別する GUID です。</span><span class="sxs-lookup"><span data-stu-id="fda63-143">The text value of the **ArchiveTag** element is a GUID that identifies the retention policy.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="fda63-144">備考</span><span class="sxs-lookup"><span data-stu-id="fda63-144">Remarks</span></span>

<span data-ttu-id="fda63-145">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="fda63-145">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="fda63-146">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="fda63-146">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fda63-147">要素情報</span><span class="sxs-lookup"><span data-stu-id="fda63-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fda63-148">名前空間</span><span class="sxs-lookup"><span data-stu-id="fda63-148">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fda63-149">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fda63-149">Schema Name</span></span>  <br/> |<span data-ttu-id="fda63-150">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="fda63-150">Type schema</span></span>  <br/> |
|<span data-ttu-id="fda63-151">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fda63-151">Validation File</span></span>  <br/> |<span data-ttu-id="fda63-152">types.xsd</span><span class="sxs-lookup"><span data-stu-id="fda63-152">types.xsd</span></span>  <br/> |
|<span data-ttu-id="fda63-153">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="fda63-153">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="fda63-154">関連項目</span><span class="sxs-lookup"><span data-stu-id="fda63-154">See also</span></span>

- [<span data-ttu-id="fda63-155">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="fda63-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

