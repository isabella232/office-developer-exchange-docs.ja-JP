---
title: DelegatePermissions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DelegatePermissions
api_type:
- schema
ms.assetid: 292badc7-bab3-4368-9d7c-9a8b7edb279b
description: DelegatePermissions 要素には、ユーザーの代理アクセス許可レベルの設定が含まれています。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 2cf8c9a8d3c5db8e13d43c207df173c12fca5acb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457411"
---
# <a name="delegatepermissions"></a><span data-ttu-id="0db9f-104">DelegatePermissions</span><span class="sxs-lookup"><span data-stu-id="0db9f-104">DelegatePermissions</span></span>

<span data-ttu-id="0db9f-105">**DelegatePermissions**要素には、ユーザーの代理アクセス許可レベルの設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0db9f-105">The **DelegatePermissions** element contains the delegate permission-level settings for a user.</span></span> <span data-ttu-id="0db9f-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="0db9f-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<DelegatePermissions>
   <CalendarFolderPermissionLevel/>
   <TasksFolderPermissionLevel/>
   <InboxFolderPermissionLevel/>
   <ContactsFolderPermissionLevel/>
   <NotesFolderPermissionLevel/>
   <JournalFolderPermissionLevel/>
</DelegatePermissions>
```

<span data-ttu-id="0db9f-107">**DelegatePermissionsType**</span><span class="sxs-lookup"><span data-stu-id="0db9f-107">**DelegatePermissionsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="0db9f-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0db9f-108">Attributes and elements</span></span>

<span data-ttu-id="0db9f-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0db9f-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0db9f-110">属性</span><span class="sxs-lookup"><span data-stu-id="0db9f-110">Attributes</span></span>

<span data-ttu-id="0db9f-111">なし。</span><span class="sxs-lookup"><span data-stu-id="0db9f-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0db9f-112">子要素</span><span class="sxs-lookup"><span data-stu-id="0db9f-112">Child elements</span></span>

|<span data-ttu-id="0db9f-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="0db9f-113">**Element**</span></span>|<span data-ttu-id="0db9f-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="0db9f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0db9f-115">CalendarFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="0db9f-115">CalendarFolderPermissionLevel</span></span>](calendarfolderpermissionlevel.md) <br/> |<span data-ttu-id="0db9f-116">既定の予定表フォルダーのアクセス許可が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0db9f-116">Contains the permissions for the default Calendar folder.</span></span> <span data-ttu-id="0db9f-117">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="0db9f-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="0db9f-118">タスク Folderpermissionlevel</span><span class="sxs-lookup"><span data-stu-id="0db9f-118">TasksFolderPermissionLevel</span></span>](tasksfolderpermissionlevel.md) <br/> |<span data-ttu-id="0db9f-119">既定のタスクフォルダーのアクセス許可が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0db9f-119">Contains the permissions for the default Task folder.</span></span> <span data-ttu-id="0db9f-120">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="0db9f-120">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="0db9f-121">受信トレイフォルダーの Permissionlevel</span><span class="sxs-lookup"><span data-stu-id="0db9f-121">InboxFolderPermissionLevel</span></span>](inboxfolderpermissionlevel.md) <br/> |<span data-ttu-id="0db9f-122">既定の受信トレイフォルダーのアクセス許可が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0db9f-122">Contains the permissions for the default Inbox folder.</span></span> <span data-ttu-id="0db9f-123">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="0db9f-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="0db9f-124">ContactsFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="0db9f-124">ContactsFolderPermissionLevel</span></span>](contactsfolderpermissionlevel.md) <br/> |<span data-ttu-id="0db9f-125">既定の連絡先フォルダーのアクセス許可が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0db9f-125">Contains the permissions for the default Contacts folder.</span></span> <span data-ttu-id="0db9f-126">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="0db9f-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="0db9f-127">注釈 Folderpermissionlevel</span><span class="sxs-lookup"><span data-stu-id="0db9f-127">NotesFolderPermissionLevel</span></span>](notesfolderpermissionlevel.md) <br/> |<span data-ttu-id="0db9f-128">既定のメモフォルダーのアクセス許可が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0db9f-128">Contains the permissions for the default Notes folder.</span></span> <span data-ttu-id="0db9f-129">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="0db9f-129">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="0db9f-130">JournalFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="0db9f-130">JournalFolderPermissionLevel</span></span>](journalfolderpermissionlevel.md) <br/> |<span data-ttu-id="0db9f-131">既定の履歴フォルダーのアクセス許可が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0db9f-131">Contains the permissions for the default Journal folder.</span></span> <span data-ttu-id="0db9f-132">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="0db9f-132">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0db9f-133">親要素</span><span class="sxs-lookup"><span data-stu-id="0db9f-133">Parent elements</span></span>

|<span data-ttu-id="0db9f-134">**要素**</span><span class="sxs-lookup"><span data-stu-id="0db9f-134">**Element**</span></span>|<span data-ttu-id="0db9f-135">**説明**</span><span class="sxs-lookup"><span data-stu-id="0db9f-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0db9f-136">DelegateUser</span><span class="sxs-lookup"><span data-stu-id="0db9f-136">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="0db9f-137">メールボックスに追加または更新する単一の代理人を指定します。</span><span class="sxs-lookup"><span data-stu-id="0db9f-137">Identifies a single delegate to add or update in a mailbox.</span></span> <span data-ttu-id="0db9f-138">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="0db9f-138">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0db9f-139">注釈</span><span class="sxs-lookup"><span data-stu-id="0db9f-139">Remarks</span></span>

<span data-ttu-id="0db9f-140">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="0db9f-140">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0db9f-141">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0db9f-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0db9f-142">Namespace</span><span class="sxs-lookup"><span data-stu-id="0db9f-142">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0db9f-143">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0db9f-143">Schema Name</span></span>  <br/> |<span data-ttu-id="0db9f-144">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="0db9f-144">Types schema</span></span>  <br/> |
|<span data-ttu-id="0db9f-145">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0db9f-145">Validation File</span></span>  <br/> |<span data-ttu-id="0db9f-146">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="0db9f-146">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0db9f-147">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0db9f-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="0db9f-148">正しくない</span><span class="sxs-lookup"><span data-stu-id="0db9f-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0db9f-149">関連項目</span><span class="sxs-lookup"><span data-stu-id="0db9f-149">See also</span></span>

- [<span data-ttu-id="0db9f-150">AddDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="0db9f-150">AddDelegate operation</span></span>](adddelegate-operation.md) 
- [<span data-ttu-id="0db9f-151">UpdateDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="0db9f-151">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
- [<span data-ttu-id="0db9f-152">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="0db9f-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="0db9f-153">代理人の追加</span><span class="sxs-lookup"><span data-stu-id="0db9f-153">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

