---
title: CalendarFolderPermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarFolderPermissionLevel
api_type:
- schema
ms.assetid: 2a5c9381-dc2c-4fc6-b9b5-893477d0970e
description: CalendarFolderPermissionLevel 要素には、既定の予定表フォルダーのアクセス許可が含まれています。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 5d51fea522656910d8417e7f75214214e2c162c6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759586"
---
# <a name="calendarfolderpermissionlevel"></a><span data-ttu-id="43a3d-104">CalendarFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="43a3d-104">CalendarFolderPermissionLevel</span></span>

<span data-ttu-id="43a3d-105">**CalendarFolderPermissionLevel**要素には、既定の予定表フォルダーのアクセス許可が含まれています。</span><span class="sxs-lookup"><span data-stu-id="43a3d-105">The **CalendarFolderPermissionLevel** element contains the permissions for the default Calendar folder.</span></span> <span data-ttu-id="43a3d-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="43a3d-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CalendarFolderPermissionLevel>
   None or Editor or Reviewer or Author or Custom
</CalendarFolderPermissionLevel>
```

 <span data-ttu-id="43a3d-107">**DelegateFolderPermissionLevelType**</span><span class="sxs-lookup"><span data-stu-id="43a3d-107">**DelegateFolderPermissionLevelType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="43a3d-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="43a3d-108">Attributes and elements</span></span>

<span data-ttu-id="43a3d-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="43a3d-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="43a3d-110">属性</span><span class="sxs-lookup"><span data-stu-id="43a3d-110">Attributes</span></span>

<span data-ttu-id="43a3d-111">なし。</span><span class="sxs-lookup"><span data-stu-id="43a3d-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="43a3d-112">子要素</span><span class="sxs-lookup"><span data-stu-id="43a3d-112">Child elements</span></span>

<span data-ttu-id="43a3d-113">なし。</span><span class="sxs-lookup"><span data-stu-id="43a3d-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="43a3d-114">親要素</span><span class="sxs-lookup"><span data-stu-id="43a3d-114">Parent elements</span></span>

|<span data-ttu-id="43a3d-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="43a3d-115">**Element**</span></span>|<span data-ttu-id="43a3d-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="43a3d-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="43a3d-117">DelegatePermissions</span><span class="sxs-lookup"><span data-stu-id="43a3d-117">DelegatePermissions</span></span>](delegatepermissions.md) <br/> |<span data-ttu-id="43a3d-118">ユーザーの代理人のアクセス許可レベルの設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="43a3d-118">Contains the delegate permission level settings for a user.</span></span> <span data-ttu-id="43a3d-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="43a3d-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="43a3d-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="43a3d-120">Text value</span></span>

<span data-ttu-id="43a3d-121">アクセス許可レベルを表す文字列値を次の表に一覧します。</span><span class="sxs-lookup"><span data-stu-id="43a3d-121">The following table lists the text values that represent the permission levels.</span></span>
  
<span data-ttu-id="43a3d-122">**アクセス許可レベルのテキスト値**</span><span class="sxs-lookup"><span data-stu-id="43a3d-122">**Permission level text values**</span></span>

|<span data-ttu-id="43a3d-123">**アクセス許可レベル**</span><span class="sxs-lookup"><span data-stu-id="43a3d-123">**Permission level**</span></span>|<span data-ttu-id="43a3d-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="43a3d-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="43a3d-125">なし</span><span class="sxs-lookup"><span data-stu-id="43a3d-125">None</span></span>  <br/> |<span data-ttu-id="43a3d-126">代理ユーザーには、予定表フォルダーへのアクセス許可がありません。</span><span class="sxs-lookup"><span data-stu-id="43a3d-126">The delegate user has no access permissions to the Calendar folder.</span></span>  <br/> |
|<span data-ttu-id="43a3d-127">Reviewer</span><span class="sxs-lookup"><span data-stu-id="43a3d-127">Reviewer</span></span>  <br/> |<span data-ttu-id="43a3d-128">代理ユーザーは、予定表フォルダー内のアイテムを読み取ることができます。</span><span class="sxs-lookup"><span data-stu-id="43a3d-128">The delegate user can read items in the Calendar folder.</span></span>  <br/> |
|<span data-ttu-id="43a3d-129">作成者</span><span class="sxs-lookup"><span data-stu-id="43a3d-129">Author</span></span>  <br/> |<span data-ttu-id="43a3d-130">代理ユーザーは、読み取りし、予定表フォルダーにアイテムを作成できます。</span><span class="sxs-lookup"><span data-stu-id="43a3d-130">The delegate user can read and create items in the Calendar folder.</span></span>  <br/> |
|<span data-ttu-id="43a3d-131">Editor</span><span class="sxs-lookup"><span data-stu-id="43a3d-131">Editor</span></span>  <br/> |<span data-ttu-id="43a3d-132">代理ユーザーは読み取り、作成、および予定表フォルダー内の項目を変更します。</span><span class="sxs-lookup"><span data-stu-id="43a3d-132">The delegate user can read, create, and modify items in the Calendar folder.</span></span>  <br/> |
|<span data-ttu-id="43a3d-133">カスタム</span><span class="sxs-lookup"><span data-stu-id="43a3d-133">Custom</span></span>  <br/> |<span data-ttu-id="43a3d-134">代理ユーザーは、予定表フォルダーにカスタム アクセス許可を持ちます。</span><span class="sxs-lookup"><span data-stu-id="43a3d-134">The delegate user has custom access permissions to the Calendar folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="43a3d-135">備考</span><span class="sxs-lookup"><span data-stu-id="43a3d-135">Remarks</span></span>

<span data-ttu-id="43a3d-136">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="43a3d-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="43a3d-137">要素情報</span><span class="sxs-lookup"><span data-stu-id="43a3d-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="43a3d-138">名前空間</span><span class="sxs-lookup"><span data-stu-id="43a3d-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="43a3d-139">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="43a3d-139">Schema Name</span></span>  <br/> |<span data-ttu-id="43a3d-140">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="43a3d-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="43a3d-141">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="43a3d-141">Validation File</span></span>  <br/> |<span data-ttu-id="43a3d-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="43a3d-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="43a3d-143">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="43a3d-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="43a3d-144">False</span><span class="sxs-lookup"><span data-stu-id="43a3d-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="43a3d-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="43a3d-145">See also</span></span>



[<span data-ttu-id="43a3d-146">AddDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="43a3d-146">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="43a3d-147">UpdateDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="43a3d-147">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="43a3d-148">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="43a3d-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="43a3d-149">デリゲートを追加します。</span><span class="sxs-lookup"><span data-stu-id="43a3d-149">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

