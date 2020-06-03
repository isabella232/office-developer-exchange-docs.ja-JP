---
title: CalendarPermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarPermissionLevel
api_type:
- schema
ms.assetid: 6ac2b792-4326-4a3f-b6cb-977bf523b5b2
description: CalendarPermissionLevel 要素は、ユーザーが予定表フォルダーに対して持っているアクセス許可レベルを表します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 670f78e0b3cef7a40339c83d84916871f8969536
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527181"
---
# <a name="calendarpermissionlevel"></a><span data-ttu-id="755cb-104">CalendarPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="755cb-104">CalendarPermissionLevel</span></span>

<span data-ttu-id="755cb-105">**Calendarpermissionlevel**要素は、ユーザーが予定表フォルダーに対して持っているアクセス許可レベルを表します。</span><span class="sxs-lookup"><span data-stu-id="755cb-105">The **CalendarPermissionLevel** element represents the permission level that a user has on a Calendar folder.</span></span> <span data-ttu-id="755cb-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="755cb-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CalendarPermissionLevel>None or Owner or PublishingEditor or Editor or PublishingAuthor or Author or NoneditingAuthor or Reviewer or Contributor or FreeBusyTimeOnly or FreeBusyTimeAndSubjectAndLocation or Custom</CalendarPermissionLevel>
```

 <span data-ttu-id="755cb-107">**CalendarPermissionLevelType**</span><span class="sxs-lookup"><span data-stu-id="755cb-107">**CalendarPermissionLevelType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="755cb-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="755cb-108">Attributes and elements</span></span>

<span data-ttu-id="755cb-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="755cb-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="755cb-110">属性</span><span class="sxs-lookup"><span data-stu-id="755cb-110">Attributes</span></span>

<span data-ttu-id="755cb-111">なし。</span><span class="sxs-lookup"><span data-stu-id="755cb-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="755cb-112">子要素</span><span class="sxs-lookup"><span data-stu-id="755cb-112">Child elements</span></span>

<span data-ttu-id="755cb-113">なし。</span><span class="sxs-lookup"><span data-stu-id="755cb-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="755cb-114">親要素</span><span class="sxs-lookup"><span data-stu-id="755cb-114">Parent elements</span></span>

|<span data-ttu-id="755cb-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="755cb-115">**Element**</span></span>|<span data-ttu-id="755cb-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="755cb-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="755cb-117">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="755cb-117">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="755cb-118">ユーザーが予定表フォルダーに対して持っているアクセス権を定義します。</span><span class="sxs-lookup"><span data-stu-id="755cb-118">Defines the access that a user has to a Calendar folder.</span></span> <span data-ttu-id="755cb-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="755cb-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="755cb-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="755cb-120">Text value</span></span>

<span data-ttu-id="755cb-121">次の表に、 **Calendarpermissionlevel**要素に指定できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="755cb-121">The following table lists the possible values for the **CalendarPermissionLevel** element.</span></span> 
  
<span data-ttu-id="755cb-122">**CalendarPermissionLevel 要素のテキスト値**</span><span class="sxs-lookup"><span data-stu-id="755cb-122">**CalendarPermissionLevel element text values**</span></span>

|<span data-ttu-id="755cb-123">**値**</span><span class="sxs-lookup"><span data-stu-id="755cb-123">**Value**</span></span>|<span data-ttu-id="755cb-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="755cb-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="755cb-125">なし</span><span class="sxs-lookup"><span data-stu-id="755cb-125">None</span></span>  <br/> |<span data-ttu-id="755cb-126">ユーザーがフォルダーに対するアクセス許可を持っていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="755cb-126">Indicates that the user has no permissions on the folder.</span></span>  <br/> |
|<span data-ttu-id="755cb-127">Owner</span><span class="sxs-lookup"><span data-stu-id="755cb-127">Owner</span></span>  <br/> |<span data-ttu-id="755cb-128">ユーザーがフォルダー内のすべてのアイテムを作成、読み取り、編集、および削除できること、およびサブフォルダーを作成できることを示します。</span><span class="sxs-lookup"><span data-stu-id="755cb-128">Indicates that the user can create, read, edit, and delete all items in the folder, and create subfolders.</span></span> <span data-ttu-id="755cb-129">ユーザーはフォルダーの所有者とフォルダーの両方の連絡先です。</span><span class="sxs-lookup"><span data-stu-id="755cb-129">The user is both folder owner and folder contact.</span></span>  <br/> |
|<span data-ttu-id="755cb-130">PublishingEditor (出版編集者)</span><span class="sxs-lookup"><span data-stu-id="755cb-130">PublishingEditor</span></span>  <br/> |<span data-ttu-id="755cb-131">ユーザーがフォルダー内のすべてのアイテムを作成、読み取り、編集、および削除できること、およびサブフォルダーを作成できることを示します。</span><span class="sxs-lookup"><span data-stu-id="755cb-131">Indicates that the user can create, read, edit, and delete all items in the folder, and create subfolders.</span></span>  <br/> |
|<span data-ttu-id="755cb-132">エディター</span><span class="sxs-lookup"><span data-stu-id="755cb-132">Editor</span></span>  <br/> |<span data-ttu-id="755cb-133">ユーザーがフォルダー内のすべてのアイテムを作成、読み取り、編集、および削除できることを示します。</span><span class="sxs-lookup"><span data-stu-id="755cb-133">Indicates that the user can create, read, edit and delete all items in the folder.</span></span>  <br/> |
|<span data-ttu-id="755cb-134">PublishingAuthor (出版著者)</span><span class="sxs-lookup"><span data-stu-id="755cb-134">PublishingAuthor</span></span>  <br/> |<span data-ttu-id="755cb-135">ユーザーがフォルダー内のすべてのアイテムを作成および読み取り、ユーザーが作成したアイテムのみを編集および削除し、サブフォルダーを作成できることを示します。</span><span class="sxs-lookup"><span data-stu-id="755cb-135">Indicates that the user can create and read all items in the folder, edit and delete only items that the user creates, and create subfolders.</span></span>  <br/> |
|<span data-ttu-id="755cb-136">設定元</span><span class="sxs-lookup"><span data-stu-id="755cb-136">Author</span></span>  <br/> |<span data-ttu-id="755cb-137">ユーザーがフォルダー内のすべてのアイテムを作成および読み取ることができ、ユーザーが作成したアイテムのみを編集および削除できることを示します。</span><span class="sxs-lookup"><span data-stu-id="755cb-137">Indicates that the user can create and read all items in the folder, and edit and delete only items that the user creates.</span></span>  <br/> |
|<span data-ttu-id="755cb-138">NoneditingAuthor (非編集著者)</span><span class="sxs-lookup"><span data-stu-id="755cb-138">NoneditingAuthor</span></span>  <br/> |<span data-ttu-id="755cb-139">ユーザーがフォルダー内のすべてのアイテムを作成および読み取ることができ、ユーザーが作成したアイテムのみを削除できることを示します。</span><span class="sxs-lookup"><span data-stu-id="755cb-139">Indicates that the user can create and read all items in the folder, and delete only items that the user creates.</span></span>  <br/> |
|<span data-ttu-id="755cb-140">レビュー担当者</span><span class="sxs-lookup"><span data-stu-id="755cb-140">Reviewer</span></span>  <br/> |<span data-ttu-id="755cb-141">ユーザーがフォルダー内のすべてのアイテムを読み取ることができることを示します。</span><span class="sxs-lookup"><span data-stu-id="755cb-141">Indicates that the user can read all items in the folder.</span></span>  <br/> |
|<span data-ttu-id="755cb-142">共同作成者</span><span class="sxs-lookup"><span data-stu-id="755cb-142">Contributor</span></span>  <br/> |<span data-ttu-id="755cb-143">ユーザーがフォルダー内にアイテムを作成できることを示します。</span><span class="sxs-lookup"><span data-stu-id="755cb-143">Indicates that the user can create items in the folder.</span></span> <span data-ttu-id="755cb-144">フォルダーの内容は表示されません。</span><span class="sxs-lookup"><span data-stu-id="755cb-144">The contents of the folder do not appear.</span></span>  <br/> |
|<span data-ttu-id="755cb-145">FreeBusyTimeOnly</span><span class="sxs-lookup"><span data-stu-id="755cb-145">FreeBusyTimeOnly</span></span>  <br/> |<span data-ttu-id="755cb-146">ユーザーが予定表内でのみ空き時間情報を表示できることを示します。</span><span class="sxs-lookup"><span data-stu-id="755cb-146">Indicates that the user can view only free/busy time within the calendar.</span></span>  <br/> |
|<span data-ttu-id="755cb-147">FreeBusyTimeAndSubjectAndLocation</span><span class="sxs-lookup"><span data-stu-id="755cb-147">FreeBusyTimeAndSubjectAndLocation</span></span>  <br/> |<span data-ttu-id="755cb-148">ユーザーが予定表内の空き時間情報を表示できること、および予定の件名と場所を表示できることを示します。</span><span class="sxs-lookup"><span data-stu-id="755cb-148">Indicates that the user can view free/busy time within the calendar and the subject and location of appointments.</span></span>  <br/> |
|<span data-ttu-id="755cb-149">Custom</span><span class="sxs-lookup"><span data-stu-id="755cb-149">Custom</span></span>  <br/> |<span data-ttu-id="755cb-150">ユーザーがフォルダーに対して独自のアクセス許可を持っていることを示します。</span><span class="sxs-lookup"><span data-stu-id="755cb-150">Indicates that the user has custom access permissions on the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="755cb-151">注釈</span><span class="sxs-lookup"><span data-stu-id="755cb-151">Remarks</span></span>

<span data-ttu-id="755cb-152">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="755cb-152">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="755cb-153">要素の情報</span><span class="sxs-lookup"><span data-stu-id="755cb-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="755cb-154">Namespace</span><span class="sxs-lookup"><span data-stu-id="755cb-154">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="755cb-155">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="755cb-155">Schema Name</span></span>  <br/> |<span data-ttu-id="755cb-156">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="755cb-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="755cb-157">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="755cb-157">Validation File</span></span>  <br/> |<span data-ttu-id="755cb-158">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="755cb-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="755cb-159">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="755cb-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="755cb-160">正しくない</span><span class="sxs-lookup"><span data-stu-id="755cb-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="755cb-161">関連項目</span><span class="sxs-lookup"><span data-stu-id="755cb-161">See also</span></span>



- [<span data-ttu-id="755cb-162">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="755cb-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="755cb-163">フォルダーレベルのアクセス許可を設定する</span><span class="sxs-lookup"><span data-stu-id="755cb-163">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

