---
title: 受信トレイフォルダーの Permissionlevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InboxFolderPermissionLevel
api_type:
- schema
ms.assetid: f250d31b-9193-4c1c-8350-900dead3a023
description: 受信トレイフォルダーには、既定の受信トレイフォルダーのアクセス許可が含まれています。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 8a497a38a58e6455f2bd754aa8da97b421a2bca3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465710"
---
# <a name="inboxfolderpermissionlevel"></a><span data-ttu-id="7e917-104">受信トレイフォルダーの Permissionlevel</span><span class="sxs-lookup"><span data-stu-id="7e917-104">InboxFolderPermissionLevel</span></span>

<span data-ttu-id="7e917-105">受信トレイフォルダー**には、** 既定の受信トレイフォルダーのアクセス許可が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7e917-105">The **InboxFolderPermissionLevel** element contains the permissions for the default Inbox folder.</span></span> <span data-ttu-id="7e917-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="7e917-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<InboxFolderPermissionLevel>
   None or Editor or Reviewer or Author or Custom
</InboxFolderPermissionLevel>
```

 <span data-ttu-id="7e917-107">**DelegateFolderPermissionLevelType**</span><span class="sxs-lookup"><span data-stu-id="7e917-107">**DelegateFolderPermissionLevelType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7e917-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7e917-108">Attributes and elements</span></span>

<span data-ttu-id="7e917-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7e917-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7e917-110">属性</span><span class="sxs-lookup"><span data-stu-id="7e917-110">Attributes</span></span>

<span data-ttu-id="7e917-111">なし。</span><span class="sxs-lookup"><span data-stu-id="7e917-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7e917-112">子要素</span><span class="sxs-lookup"><span data-stu-id="7e917-112">Child elements</span></span>

<span data-ttu-id="7e917-113">なし。</span><span class="sxs-lookup"><span data-stu-id="7e917-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7e917-114">親要素</span><span class="sxs-lookup"><span data-stu-id="7e917-114">Parent elements</span></span>

|<span data-ttu-id="7e917-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="7e917-115">**Element**</span></span>|<span data-ttu-id="7e917-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="7e917-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e917-117">DelegatePermissions</span><span class="sxs-lookup"><span data-stu-id="7e917-117">DelegatePermissions</span></span>](delegatepermissions.md) <br/> |<span data-ttu-id="7e917-118">ユーザーの代理アクセス許可レベルの設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7e917-118">Contains the delegate permission level settings for a user.</span></span> <span data-ttu-id="7e917-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="7e917-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7e917-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7e917-120">Text value</span></span>

<span data-ttu-id="7e917-121">次の表に、アクセス許可レベルを表すテキスト値の一覧を示します。</span><span class="sxs-lookup"><span data-stu-id="7e917-121">The following table lists the text values that represent the permission levels.</span></span>
  
<span data-ttu-id="7e917-122">**アクセス許可レベルのテキスト値**</span><span class="sxs-lookup"><span data-stu-id="7e917-122">**Permission level text values**</span></span>

|<span data-ttu-id="7e917-123">**アクセス許可レベル**</span><span class="sxs-lookup"><span data-stu-id="7e917-123">**Permission level**</span></span>|<span data-ttu-id="7e917-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="7e917-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7e917-125">なし</span><span class="sxs-lookup"><span data-stu-id="7e917-125">None</span></span>  <br/> |<span data-ttu-id="7e917-126">代理人ユーザーには、受信トレイフォルダーへのアクセス許可はありません。</span><span class="sxs-lookup"><span data-stu-id="7e917-126">The delegate user has no access permissions to the Inbox folder.</span></span>  <br/> |
|<span data-ttu-id="7e917-127">レビュー担当者</span><span class="sxs-lookup"><span data-stu-id="7e917-127">Reviewer</span></span>  <br/> |<span data-ttu-id="7e917-128">代理人のユーザーは、受信トレイフォルダー内のアイテムを読み取ることができます。</span><span class="sxs-lookup"><span data-stu-id="7e917-128">The delegate user can read items in the Inbox folder.</span></span>  <br/> |
|<span data-ttu-id="7e917-129">設定元</span><span class="sxs-lookup"><span data-stu-id="7e917-129">Author</span></span>  <br/> |<span data-ttu-id="7e917-130">代理人のユーザーは、受信トレイフォルダー内のアイテムの読み取りと作成を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="7e917-130">The delegate user can read and create items in the Inbox folder.</span></span>  <br/> |
|<span data-ttu-id="7e917-131">エディター</span><span class="sxs-lookup"><span data-stu-id="7e917-131">Editor</span></span>  <br/> |<span data-ttu-id="7e917-132">代理人のユーザーは、受信トレイフォルダー内のアイテムの読み取り、作成、および変更を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="7e917-132">The delegate user can read, create, and modify items in the Inbox folder.</span></span>  <br/> |
|<span data-ttu-id="7e917-133">Custom</span><span class="sxs-lookup"><span data-stu-id="7e917-133">Custom</span></span>  <br/> |<span data-ttu-id="7e917-134">代理人ユーザーには、受信トレイフォルダーに対する独自のアクセス許可があります。</span><span class="sxs-lookup"><span data-stu-id="7e917-134">The delegate user has custom access permissions to the Inbox folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7e917-135">注釈</span><span class="sxs-lookup"><span data-stu-id="7e917-135">Remarks</span></span>

<span data-ttu-id="7e917-136">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="7e917-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7e917-137">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7e917-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7e917-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="7e917-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7e917-139">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7e917-139">Schema Name</span></span>  <br/> |<span data-ttu-id="7e917-140">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="7e917-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="7e917-141">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7e917-141">Validation File</span></span>  <br/> |<span data-ttu-id="7e917-142">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="7e917-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7e917-143">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7e917-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="7e917-144">正しくない</span><span class="sxs-lookup"><span data-stu-id="7e917-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7e917-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="7e917-145">See also</span></span>



[<span data-ttu-id="7e917-146">AddDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="7e917-146">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="7e917-147">UpdateDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="7e917-147">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="7e917-148">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="7e917-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="7e917-149">代理人の追加</span><span class="sxs-lookup"><span data-stu-id="7e917-149">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

