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
description: CalendarPermissionLevel 要素は、ユーザーが予定表フォルダーに必要なアクセス許可レベルを表します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 646e4df3b70350a16cdd1f3e134260c2984a5161
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759596"
---
# <a name="calendarpermissionlevel"></a><span data-ttu-id="931a2-104">CalendarPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="931a2-104">CalendarPermissionLevel</span></span>

<span data-ttu-id="931a2-105">**CalendarPermissionLevel**要素は、ユーザーが予定表フォルダーに必要なアクセス許可レベルを表します。</span><span class="sxs-lookup"><span data-stu-id="931a2-105">The **CalendarPermissionLevel** element represents the permission level that a user has on a Calendar folder.</span></span> <span data-ttu-id="931a2-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="931a2-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CalendarPermissionLevel>None or Owner or PublishingEditor or Editor or PublishingAuthor or Author or NoneditingAuthor or Reviewer or Contributor or FreeBusyTimeOnly or FreeBusyTimeAndSubjectAndLocation or Custom</CalendarPermissionLevel>
```

 <span data-ttu-id="931a2-107">**CalendarPermissionLevelType**</span><span class="sxs-lookup"><span data-stu-id="931a2-107">**CalendarPermissionLevelType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="931a2-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="931a2-108">Attributes and elements</span></span>

<span data-ttu-id="931a2-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="931a2-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="931a2-110">属性</span><span class="sxs-lookup"><span data-stu-id="931a2-110">Attributes</span></span>

<span data-ttu-id="931a2-111">なし。</span><span class="sxs-lookup"><span data-stu-id="931a2-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="931a2-112">子要素</span><span class="sxs-lookup"><span data-stu-id="931a2-112">Child elements</span></span>

<span data-ttu-id="931a2-113">なし。</span><span class="sxs-lookup"><span data-stu-id="931a2-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="931a2-114">親要素</span><span class="sxs-lookup"><span data-stu-id="931a2-114">Parent elements</span></span>

|<span data-ttu-id="931a2-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="931a2-115">**Element**</span></span>|<span data-ttu-id="931a2-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="931a2-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="931a2-117">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="931a2-117">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="931a2-118">予定表フォルダーにユーザーが持つアクセス権を定義します。</span><span class="sxs-lookup"><span data-stu-id="931a2-118">Defines the access that a user has to a Calendar folder.</span></span> <span data-ttu-id="931a2-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="931a2-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="931a2-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="931a2-120">Text value</span></span>

<span data-ttu-id="931a2-121">次の表は、 **CalendarPermissionLevel**要素の値を一覧します。</span><span class="sxs-lookup"><span data-stu-id="931a2-121">The following table lists the possible values for the **CalendarPermissionLevel** element.</span></span> 
  
<span data-ttu-id="931a2-122">**CalendarPermissionLevel 要素のテキスト値**</span><span class="sxs-lookup"><span data-stu-id="931a2-122">**CalendarPermissionLevel element text values**</span></span>

|<span data-ttu-id="931a2-123">**値**</span><span class="sxs-lookup"><span data-stu-id="931a2-123">**Value**</span></span>|<span data-ttu-id="931a2-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="931a2-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="931a2-125">なし</span><span class="sxs-lookup"><span data-stu-id="931a2-125">None</span></span>  <br/> |<span data-ttu-id="931a2-126">そのユーザーの権限を持ってフォルダーを示します。</span><span class="sxs-lookup"><span data-stu-id="931a2-126">Indicates that the user has no permissions on the folder.</span></span>  <br/> |
|<span data-ttu-id="931a2-127">Owner</span><span class="sxs-lookup"><span data-stu-id="931a2-127">Owner</span></span>  <br/> |<span data-ttu-id="931a2-128">ユーザーことができます作成、読み取り、編集、および、フォルダー内のすべてのアイテムを削除およびサブフォルダーを作成することを示します。</span><span class="sxs-lookup"><span data-stu-id="931a2-128">Indicates that the user can create, read, edit, and delete all items in the folder, and create subfolders.</span></span> <span data-ttu-id="931a2-129">ユーザーは、フォルダーの所有者とフォルダーの連絡先の両方です。</span><span class="sxs-lookup"><span data-stu-id="931a2-129">The user is both folder owner and folder contact.</span></span>  <br/> |
|<span data-ttu-id="931a2-130">PublishingEditor (出版編集者)</span><span class="sxs-lookup"><span data-stu-id="931a2-130">PublishingEditor</span></span>  <br/> |<span data-ttu-id="931a2-131">ユーザーことができます作成、読み取り、編集、および、フォルダー内のすべてのアイテムを削除およびサブフォルダーを作成することを示します。</span><span class="sxs-lookup"><span data-stu-id="931a2-131">Indicates that the user can create, read, edit, and delete all items in the folder, and create subfolders.</span></span>  <br/> |
|<span data-ttu-id="931a2-132">Editor</span><span class="sxs-lookup"><span data-stu-id="931a2-132">Editor</span></span>  <br/> |<span data-ttu-id="931a2-133">ユーザーが作成、読み取り、編集およびフォルダー内のすべてのアイテムを削除することを示します。</span><span class="sxs-lookup"><span data-stu-id="931a2-133">Indicates that the user can create, read, edit and delete all items in the folder.</span></span>  <br/> |
|<span data-ttu-id="931a2-134">PublishingAuthor (出版著者)</span><span class="sxs-lookup"><span data-stu-id="931a2-134">PublishingAuthor</span></span>  <br/> |<span data-ttu-id="931a2-135">ユーザーを作成し、フォルダー内のすべてのアイテム編集しユーザーを作成するアイテムのみを削除し、ことサブフォルダーを作成することを示します。</span><span class="sxs-lookup"><span data-stu-id="931a2-135">Indicates that the user can create and read all items in the folder, edit and delete only items that the user creates, and create subfolders.</span></span>  <br/> |
|<span data-ttu-id="931a2-136">作成者</span><span class="sxs-lookup"><span data-stu-id="931a2-136">Author</span></span>  <br/> |<span data-ttu-id="931a2-137">ユーザーを作成し、フォルダー内のすべてのアイテムし編集および削除できますユーザーが作成したアイテムのみを示します。</span><span class="sxs-lookup"><span data-stu-id="931a2-137">Indicates that the user can create and read all items in the folder, and edit and delete only items that the user creates.</span></span>  <br/> |
|<span data-ttu-id="931a2-138">NoneditingAuthor (非編集著者)</span><span class="sxs-lookup"><span data-stu-id="931a2-138">NoneditingAuthor</span></span>  <br/> |<span data-ttu-id="931a2-139">ユーザーを作成し、フォルダー内のすべてのアイテムを読み取るし、ことユーザーが作成したアイテムのみを削除することを示します。</span><span class="sxs-lookup"><span data-stu-id="931a2-139">Indicates that the user can create and read all items in the folder, and delete only items that the user creates.</span></span>  <br/> |
|<span data-ttu-id="931a2-140">Reviewer</span><span class="sxs-lookup"><span data-stu-id="931a2-140">Reviewer</span></span>  <br/> |<span data-ttu-id="931a2-141">ユーザーがフォルダー内のすべてのアイテムを読み取ることができますを示します。</span><span class="sxs-lookup"><span data-stu-id="931a2-141">Indicates that the user can read all items in the folder.</span></span>  <br/> |
|<span data-ttu-id="931a2-142">Contributor</span><span class="sxs-lookup"><span data-stu-id="931a2-142">Contributor</span></span>  <br/> |<span data-ttu-id="931a2-143">ユーザーがフォルダーにアイテムを作成できることを示します。</span><span class="sxs-lookup"><span data-stu-id="931a2-143">Indicates that the user can create items in the folder.</span></span> <span data-ttu-id="931a2-144">フォルダーの内容は表示されません。</span><span class="sxs-lookup"><span data-stu-id="931a2-144">The contents of the folder do not appear.</span></span>  <br/> |
|<span data-ttu-id="931a2-145">FreeBusyTimeOnly</span><span class="sxs-lookup"><span data-stu-id="931a2-145">FreeBusyTimeOnly</span></span>  <br/> |<span data-ttu-id="931a2-146">表示できますのみ空き時間情報、予定表のことを示します。</span><span class="sxs-lookup"><span data-stu-id="931a2-146">Indicates that the user can view only free/busy time within the calendar.</span></span>  <br/> |
|<span data-ttu-id="931a2-147">FreeBusyTimeAndSubjectAndLocation</span><span class="sxs-lookup"><span data-stu-id="931a2-147">FreeBusyTimeAndSubjectAndLocation</span></span>  <br/> |<span data-ttu-id="931a2-148">ユーザーは、予定表、件名と予定の場所の範囲内の時間の空き時間情報を表示できますを示します。</span><span class="sxs-lookup"><span data-stu-id="931a2-148">Indicates that the user can view free/busy time within the calendar and the subject and location of appointments.</span></span>  <br/> |
|<span data-ttu-id="931a2-149">カスタム</span><span class="sxs-lookup"><span data-stu-id="931a2-149">Custom</span></span>  <br/> |<span data-ttu-id="931a2-150">ユーザーがフォルダーのカスタム アクセス許可を持っていることを示します。</span><span class="sxs-lookup"><span data-stu-id="931a2-150">Indicates that the user has custom access permissions on the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="931a2-151">備考</span><span class="sxs-lookup"><span data-stu-id="931a2-151">Remarks</span></span>

<span data-ttu-id="931a2-152">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="931a2-152">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="931a2-153">要素情報</span><span class="sxs-lookup"><span data-stu-id="931a2-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="931a2-154">名前空間</span><span class="sxs-lookup"><span data-stu-id="931a2-154">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="931a2-155">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="931a2-155">Schema Name</span></span>  <br/> |<span data-ttu-id="931a2-156">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="931a2-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="931a2-157">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="931a2-157">Validation File</span></span>  <br/> |<span data-ttu-id="931a2-158">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="931a2-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="931a2-159">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="931a2-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="931a2-160">False</span><span class="sxs-lookup"><span data-stu-id="931a2-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="931a2-161">関連項目</span><span class="sxs-lookup"><span data-stu-id="931a2-161">See also</span></span>



- [<span data-ttu-id="931a2-162">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="931a2-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="931a2-163">フォルダー レベルのアクセス許可の設定</span><span class="sxs-lookup"><span data-stu-id="931a2-163">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

