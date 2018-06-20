---
title: InboxFolderPermissionLevel
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
description: InboxFolderPermissionLevel 要素には、既定の受信トレイ フォルダーのアクセス許可が含まれています。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 59d0432fe9c49fdc1c4a470e1f3273c203b2ec4b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831902"
---
# <a name="inboxfolderpermissionlevel"></a><span data-ttu-id="6c007-104">InboxFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="6c007-104">InboxFolderPermissionLevel</span></span>

<span data-ttu-id="6c007-105">**InboxFolderPermissionLevel**要素には、既定の受信トレイ フォルダーのアクセス許可が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6c007-105">The **InboxFolderPermissionLevel** element contains the permissions for the default Inbox folder.</span></span> <span data-ttu-id="6c007-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6c007-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<InboxFolderPermissionLevel>
   None or Editor or Reviewer or Author or Custom
</InboxFolderPermissionLevel>
```

 <span data-ttu-id="6c007-107">**DelegateFolderPermissionLevelType**</span><span class="sxs-lookup"><span data-stu-id="6c007-107">**DelegateFolderPermissionLevelType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6c007-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6c007-108">Attributes and elements</span></span>

<span data-ttu-id="6c007-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6c007-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6c007-110">属性</span><span class="sxs-lookup"><span data-stu-id="6c007-110">Attributes</span></span>

<span data-ttu-id="6c007-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6c007-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6c007-112">子要素</span><span class="sxs-lookup"><span data-stu-id="6c007-112">Child elements</span></span>

<span data-ttu-id="6c007-113">なし。</span><span class="sxs-lookup"><span data-stu-id="6c007-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6c007-114">親要素</span><span class="sxs-lookup"><span data-stu-id="6c007-114">Parent elements</span></span>

|<span data-ttu-id="6c007-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="6c007-115">**Element**</span></span>|<span data-ttu-id="6c007-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="6c007-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6c007-117">DelegatePermissions</span><span class="sxs-lookup"><span data-stu-id="6c007-117">DelegatePermissions</span></span>](delegatepermissions.md) <br/> |<span data-ttu-id="6c007-118">ユーザーの代理人のアクセス許可レベルの設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6c007-118">Contains the delegate permission level settings for a user.</span></span> <span data-ttu-id="6c007-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6c007-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6c007-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6c007-120">Text value</span></span>

<span data-ttu-id="6c007-121">アクセス許可レベルを表す文字列値を次の表に一覧します。</span><span class="sxs-lookup"><span data-stu-id="6c007-121">The following table lists the text values that represent the permission levels.</span></span>
  
<span data-ttu-id="6c007-122">**アクセス許可レベルのテキスト値**</span><span class="sxs-lookup"><span data-stu-id="6c007-122">**Permission level text values**</span></span>

|<span data-ttu-id="6c007-123">**アクセス許可レベル**</span><span class="sxs-lookup"><span data-stu-id="6c007-123">**Permission level**</span></span>|<span data-ttu-id="6c007-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="6c007-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6c007-125">なし</span><span class="sxs-lookup"><span data-stu-id="6c007-125">None</span></span>  <br/> |<span data-ttu-id="6c007-126">代理ユーザーの受信トレイ フォルダーにアクセス許可がありません。</span><span class="sxs-lookup"><span data-stu-id="6c007-126">The delegate user has no access permissions to the Inbox folder.</span></span>  <br/> |
|<span data-ttu-id="6c007-127">Reviewer</span><span class="sxs-lookup"><span data-stu-id="6c007-127">Reviewer</span></span>  <br/> |<span data-ttu-id="6c007-128">代理ユーザーは、受信トレイ フォルダー内のアイテムを読み取ることができます。</span><span class="sxs-lookup"><span data-stu-id="6c007-128">The delegate user can read items in the Inbox folder.</span></span>  <br/> |
|<span data-ttu-id="6c007-129">作成者</span><span class="sxs-lookup"><span data-stu-id="6c007-129">Author</span></span>  <br/> |<span data-ttu-id="6c007-130">代理ユーザーでは、読み取りでき、受信トレイ フォルダーにアイテムを作成することができます。</span><span class="sxs-lookup"><span data-stu-id="6c007-130">The delegate user can read and create items in the Inbox folder.</span></span>  <br/> |
|<span data-ttu-id="6c007-131">Editor</span><span class="sxs-lookup"><span data-stu-id="6c007-131">Editor</span></span>  <br/> |<span data-ttu-id="6c007-132">代理ユーザーは読み取り、作成、および [受信トレイ] フォルダー内のアイテムを変更します。</span><span class="sxs-lookup"><span data-stu-id="6c007-132">The delegate user can read, create, and modify items in the Inbox folder.</span></span>  <br/> |
|<span data-ttu-id="6c007-133">カスタム</span><span class="sxs-lookup"><span data-stu-id="6c007-133">Custom</span></span>  <br/> |<span data-ttu-id="6c007-134">代理ユーザーは、受信トレイ フォルダーにカスタム アクセス許可を持ちます。</span><span class="sxs-lookup"><span data-stu-id="6c007-134">The delegate user has custom access permissions to the Inbox folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6c007-135">備考</span><span class="sxs-lookup"><span data-stu-id="6c007-135">Remarks</span></span>

<span data-ttu-id="6c007-136">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="6c007-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6c007-137">要素情報</span><span class="sxs-lookup"><span data-stu-id="6c007-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6c007-138">名前空間</span><span class="sxs-lookup"><span data-stu-id="6c007-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6c007-139">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6c007-139">Schema Name</span></span>  <br/> |<span data-ttu-id="6c007-140">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="6c007-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="6c007-141">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6c007-141">Validation File</span></span>  <br/> |<span data-ttu-id="6c007-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6c007-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6c007-143">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6c007-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="6c007-144">False</span><span class="sxs-lookup"><span data-stu-id="6c007-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6c007-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="6c007-145">See also</span></span>



[<span data-ttu-id="6c007-146">AddDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="6c007-146">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="6c007-147">UpdateDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="6c007-147">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="6c007-148">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="6c007-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="6c007-149">デリゲートを追加します。</span><span class="sxs-lookup"><span data-stu-id="6c007-149">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

