---
title: TasksFolderPermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TasksFolderPermissionLevel
api_type:
- schema
ms.assetid: 0f70b79b-3443-4048-b410-692d4e2464fc
description: TasksFolderPermissionLevel 要素には、既定の仕事フォルダーのアクセス許可が含まれています。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 49807896f9175bafbef106c41d1c9dff8f6178c4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839649"
---
# <a name="tasksfolderpermissionlevel"></a><span data-ttu-id="efe57-104">TasksFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="efe57-104">TasksFolderPermissionLevel</span></span>

<span data-ttu-id="efe57-105">**TasksFolderPermissionLevel**要素には、既定の仕事フォルダーのアクセス許可が含まれています。</span><span class="sxs-lookup"><span data-stu-id="efe57-105">The **TasksFolderPermissionLevel** element contains the permissions for the default Tasks folder.</span></span> <span data-ttu-id="efe57-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="efe57-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<TasksFolderPermissionLevel>
   None or Editor or Reviewer or Author or Custom
</TasksFolderPermissionLevel>
```

<span data-ttu-id="efe57-107">**DelegateFolderPermissionLevelType**</span><span class="sxs-lookup"><span data-stu-id="efe57-107">**DelegateFolderPermissionLevelType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="efe57-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="efe57-108">Attributes and elements</span></span>

<span data-ttu-id="efe57-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="efe57-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="efe57-110">属性</span><span class="sxs-lookup"><span data-stu-id="efe57-110">Attributes</span></span>

<span data-ttu-id="efe57-111">なし。</span><span class="sxs-lookup"><span data-stu-id="efe57-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="efe57-112">子要素</span><span class="sxs-lookup"><span data-stu-id="efe57-112">Child elements</span></span>

<span data-ttu-id="efe57-113">なし。</span><span class="sxs-lookup"><span data-stu-id="efe57-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="efe57-114">親要素</span><span class="sxs-lookup"><span data-stu-id="efe57-114">Parent elements</span></span>

|<span data-ttu-id="efe57-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="efe57-115">**Element**</span></span>|<span data-ttu-id="efe57-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="efe57-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="efe57-117">DelegatePermissions</span><span class="sxs-lookup"><span data-stu-id="efe57-117">DelegatePermissions</span></span>](delegatepermissions.md) <br/> |<span data-ttu-id="efe57-118">ユーザーの代理人のアクセス許可レベルの設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="efe57-118">Contains the delegate permission level settings for a user.</span></span> <span data-ttu-id="efe57-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="efe57-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="efe57-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="efe57-120">Text value</span></span>

<span data-ttu-id="efe57-121">アクセス許可レベルを表す文字列値を次の表に一覧します。</span><span class="sxs-lookup"><span data-stu-id="efe57-121">The following table lists the text values that represent the permission levels.</span></span>
  
<span data-ttu-id="efe57-122">**アクセス許可レベルのテキスト値**</span><span class="sxs-lookup"><span data-stu-id="efe57-122">**Permission level text values**</span></span>

|<span data-ttu-id="efe57-123">**アクセス許可レベル**</span><span class="sxs-lookup"><span data-stu-id="efe57-123">**Permission level**</span></span>|<span data-ttu-id="efe57-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="efe57-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="efe57-125">なし</span><span class="sxs-lookup"><span data-stu-id="efe57-125">None</span></span>  <br/> |<span data-ttu-id="efe57-126">[仕事] フォルダーには、代理ユーザーのアクセス許可がありません。</span><span class="sxs-lookup"><span data-stu-id="efe57-126">The delegate user has no access permissions to the Tasks folder.</span></span>  <br/> |
|<span data-ttu-id="efe57-127">Reviewer</span><span class="sxs-lookup"><span data-stu-id="efe57-127">Reviewer</span></span>  <br/> |<span data-ttu-id="efe57-128">代理ユーザーは、[仕事] フォルダー内のアイテムを読み取ることができます。</span><span class="sxs-lookup"><span data-stu-id="efe57-128">The delegate user can read items in the Tasks folder.</span></span>  <br/> |
|<span data-ttu-id="efe57-129">作成者</span><span class="sxs-lookup"><span data-stu-id="efe57-129">Author</span></span>  <br/> |<span data-ttu-id="efe57-130">代理ユーザーは、読み取りし、[仕事] フォルダーにアイテムを作成できます。</span><span class="sxs-lookup"><span data-stu-id="efe57-130">The delegate user can read and create items in the Tasks folder.</span></span>  <br/> |
|<span data-ttu-id="efe57-131">Editor</span><span class="sxs-lookup"><span data-stu-id="efe57-131">Editor</span></span>  <br/> |<span data-ttu-id="efe57-132">代理ユーザーは読み取り、作成、および [仕事] フォルダー内の項目を変更します。</span><span class="sxs-lookup"><span data-stu-id="efe57-132">The delegate user can read, create, and modify items in the Tasks folder.</span></span>  <br/> |
|<span data-ttu-id="efe57-133">カスタム</span><span class="sxs-lookup"><span data-stu-id="efe57-133">Custom</span></span>  <br/> |<span data-ttu-id="efe57-134">代理ユーザーは、[仕事] フォルダーにカスタム アクセス許可を持ちます。</span><span class="sxs-lookup"><span data-stu-id="efe57-134">The delegate user has custom access permissions to the Tasks folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="efe57-135">備考</span><span class="sxs-lookup"><span data-stu-id="efe57-135">Remarks</span></span>

<span data-ttu-id="efe57-136">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="efe57-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="efe57-137">要素情報</span><span class="sxs-lookup"><span data-stu-id="efe57-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="efe57-138">名前空間</span><span class="sxs-lookup"><span data-stu-id="efe57-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="efe57-139">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="efe57-139">Schema Name</span></span>  <br/> |<span data-ttu-id="efe57-140">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="efe57-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="efe57-141">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="efe57-141">Validation File</span></span>  <br/> |<span data-ttu-id="efe57-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="efe57-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="efe57-143">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="efe57-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="efe57-144">False</span><span class="sxs-lookup"><span data-stu-id="efe57-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="efe57-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="efe57-145">See also</span></span>

- [<span data-ttu-id="efe57-146">AddDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="efe57-146">AddDelegate operation</span></span>](adddelegate-operation.md)
- [<span data-ttu-id="efe57-147">UpdateDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="efe57-147">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
- [<span data-ttu-id="efe57-148">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="efe57-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="efe57-149">デリゲートを追加します。</span><span class="sxs-lookup"><span data-stu-id="efe57-149">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

