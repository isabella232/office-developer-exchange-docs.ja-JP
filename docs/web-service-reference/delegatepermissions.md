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
description: DelegatePermissions 要素には、ユーザーの代理人アクセス許可レベルの設定が含まれています。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 319592b6c3386a07b3094115c335c7fb8ffe1130
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759950"
---
# <a name="delegatepermissions"></a><span data-ttu-id="9fada-104">DelegatePermissions</span><span class="sxs-lookup"><span data-stu-id="9fada-104">DelegatePermissions</span></span>

<span data-ttu-id="9fada-105">**DelegatePermissions**要素には、ユーザーの代理人アクセス許可レベルの設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9fada-105">The **DelegatePermissions** element contains the delegate permission-level settings for a user.</span></span> <span data-ttu-id="9fada-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9fada-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
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

<span data-ttu-id="9fada-107">**DelegatePermissionsType**</span><span class="sxs-lookup"><span data-stu-id="9fada-107">**DelegatePermissionsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="9fada-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9fada-108">Attributes and elements</span></span>

<span data-ttu-id="9fada-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9fada-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9fada-110">属性</span><span class="sxs-lookup"><span data-stu-id="9fada-110">Attributes</span></span>

<span data-ttu-id="9fada-111">なし。</span><span class="sxs-lookup"><span data-stu-id="9fada-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9fada-112">子要素</span><span class="sxs-lookup"><span data-stu-id="9fada-112">Child elements</span></span>

|<span data-ttu-id="9fada-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="9fada-113">**Element**</span></span>|<span data-ttu-id="9fada-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="9fada-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9fada-115">CalendarFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="9fada-115">CalendarFolderPermissionLevel</span></span>](calendarfolderpermissionlevel.md) <br/> |<span data-ttu-id="9fada-116">既定の予定表フォルダーのアクセス許可が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9fada-116">Contains the permissions for the default Calendar folder.</span></span> <span data-ttu-id="9fada-117">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9fada-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="9fada-118">TasksFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="9fada-118">TasksFolderPermissionLevel</span></span>](tasksfolderpermissionlevel.md) <br/> |<span data-ttu-id="9fada-119">既定の作業フォルダーのアクセス許可が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9fada-119">Contains the permissions for the default Task folder.</span></span> <span data-ttu-id="9fada-120">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9fada-120">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="9fada-121">InboxFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="9fada-121">InboxFolderPermissionLevel</span></span>](inboxfolderpermissionlevel.md) <br/> |<span data-ttu-id="9fada-122">既定の受信トレイ フォルダーのアクセス許可が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9fada-122">Contains the permissions for the default Inbox folder.</span></span> <span data-ttu-id="9fada-123">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9fada-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="9fada-124">ContactsFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="9fada-124">ContactsFolderPermissionLevel</span></span>](contactsfolderpermissionlevel.md) <br/> |<span data-ttu-id="9fada-125">既定の連絡先フォルダーのアクセス許可が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9fada-125">Contains the permissions for the default Contacts folder.</span></span> <span data-ttu-id="9fada-126">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9fada-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="9fada-127">NotesFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="9fada-127">NotesFolderPermissionLevel</span></span>](notesfolderpermissionlevel.md) <br/> |<span data-ttu-id="9fada-128">既定のメモ フォルダーのアクセス許可が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9fada-128">Contains the permissions for the default Notes folder.</span></span> <span data-ttu-id="9fada-129">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9fada-129">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="9fada-130">JournalFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="9fada-130">JournalFolderPermissionLevel</span></span>](journalfolderpermissionlevel.md) <br/> |<span data-ttu-id="9fada-131">仕訳帳の既定のフォルダーのアクセス許可が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9fada-131">Contains the permissions for the default Journal folder.</span></span> <span data-ttu-id="9fada-132">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9fada-132">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9fada-133">親要素</span><span class="sxs-lookup"><span data-stu-id="9fada-133">Parent elements</span></span>

|<span data-ttu-id="9fada-134">**要素**</span><span class="sxs-lookup"><span data-stu-id="9fada-134">**Element**</span></span>|<span data-ttu-id="9fada-135">**説明**</span><span class="sxs-lookup"><span data-stu-id="9fada-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9fada-136">DelegateUser</span><span class="sxs-lookup"><span data-stu-id="9fada-136">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="9fada-137">1 つのデリゲートを追加するメールボックスの更新を識別します。</span><span class="sxs-lookup"><span data-stu-id="9fada-137">Identifies a single delegate to add or update in a mailbox.</span></span> <span data-ttu-id="9fada-138">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9fada-138">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9fada-139">備考</span><span class="sxs-lookup"><span data-stu-id="9fada-139">Remarks</span></span>

<span data-ttu-id="9fada-140">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="9fada-140">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9fada-141">要素情報</span><span class="sxs-lookup"><span data-stu-id="9fada-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9fada-142">名前空間</span><span class="sxs-lookup"><span data-stu-id="9fada-142">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9fada-143">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9fada-143">Schema Name</span></span>  <br/> |<span data-ttu-id="9fada-144">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="9fada-144">Types schema</span></span>  <br/> |
|<span data-ttu-id="9fada-145">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9fada-145">Validation File</span></span>  <br/> |<span data-ttu-id="9fada-146">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9fada-146">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9fada-147">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9fada-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="9fada-148">False</span><span class="sxs-lookup"><span data-stu-id="9fada-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9fada-149">関連項目</span><span class="sxs-lookup"><span data-stu-id="9fada-149">See also</span></span>

- [<span data-ttu-id="9fada-150">AddDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="9fada-150">AddDelegate operation</span></span>](adddelegate-operation.md) 
- [<span data-ttu-id="9fada-151">UpdateDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="9fada-151">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
- [<span data-ttu-id="9fada-152">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="9fada-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="9fada-153">デリゲートを追加します。</span><span class="sxs-lookup"><span data-stu-id="9fada-153">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

