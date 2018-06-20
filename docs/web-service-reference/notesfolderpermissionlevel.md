---
title: NotesFolderPermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NotesFolderPermissionLevel
api_type:
- schema
ms.assetid: 76a2520c-f453-4fd7-b3eb-1c5f4666680a
description: NotesFolderPermissionLevel 要素には、既定のメモ フォルダーのアクセス許可が含まれています。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: dd8644210692e0c342079d055ddf00b8d9283d7d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832552"
---
# <a name="notesfolderpermissionlevel"></a><span data-ttu-id="7dabe-104">NotesFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="7dabe-104">NotesFolderPermissionLevel</span></span>

<span data-ttu-id="7dabe-105">**NotesFolderPermissionLevel**要素には、既定のメモ フォルダーのアクセス許可が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7dabe-105">The **NotesFolderPermissionLevel** element contains the permissions for the default Notes folder.</span></span> <span data-ttu-id="7dabe-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="7dabe-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<NotesFolderPermissionLevel>
   None or Editor or Reviewer or Author or Custom
</NotesFolderPermissionLevel>
```

 <span data-ttu-id="7dabe-107">**DelegateFolderPermissionLevelType**</span><span class="sxs-lookup"><span data-stu-id="7dabe-107">**DelegateFolderPermissionLevelType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7dabe-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7dabe-108">Attributes and elements</span></span>

<span data-ttu-id="7dabe-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7dabe-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7dabe-110">属性</span><span class="sxs-lookup"><span data-stu-id="7dabe-110">Attributes</span></span>

<span data-ttu-id="7dabe-111">なし。</span><span class="sxs-lookup"><span data-stu-id="7dabe-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7dabe-112">子要素</span><span class="sxs-lookup"><span data-stu-id="7dabe-112">Child elements</span></span>

<span data-ttu-id="7dabe-113">なし。</span><span class="sxs-lookup"><span data-stu-id="7dabe-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7dabe-114">親要素</span><span class="sxs-lookup"><span data-stu-id="7dabe-114">Parent elements</span></span>

|<span data-ttu-id="7dabe-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="7dabe-115">**Element**</span></span>|<span data-ttu-id="7dabe-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="7dabe-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7dabe-117">DelegatePermissions</span><span class="sxs-lookup"><span data-stu-id="7dabe-117">DelegatePermissions</span></span>](delegatepermissions.md) <br/> |<span data-ttu-id="7dabe-118">ユーザーの代理人のアクセス許可レベルの設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7dabe-118">Contains the delegate permission level settings for a user.</span></span> <span data-ttu-id="7dabe-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="7dabe-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7dabe-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7dabe-120">Text value</span></span>

<span data-ttu-id="7dabe-121">アクセス許可レベルを表す文字列値を次の表に一覧します。</span><span class="sxs-lookup"><span data-stu-id="7dabe-121">The following table lists the text values that represent the permission levels.</span></span>
  
<span data-ttu-id="7dabe-122">**アクセス許可レベルのテキスト値**</span><span class="sxs-lookup"><span data-stu-id="7dabe-122">**Permission level text values**</span></span>

|<span data-ttu-id="7dabe-123">**アクセス許可レベル**</span><span class="sxs-lookup"><span data-stu-id="7dabe-123">**Permission level**</span></span>|<span data-ttu-id="7dabe-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="7dabe-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7dabe-125">なし</span><span class="sxs-lookup"><span data-stu-id="7dabe-125">None</span></span>  <br/> |<span data-ttu-id="7dabe-126">代理ユーザーには、メモ フォルダーへのアクセス許可がありません。</span><span class="sxs-lookup"><span data-stu-id="7dabe-126">The delegate user has no access permissions to the Notes folder.</span></span>  <br/> |
|<span data-ttu-id="7dabe-127">Reviewer</span><span class="sxs-lookup"><span data-stu-id="7dabe-127">Reviewer</span></span>  <br/> |<span data-ttu-id="7dabe-128">代理ユーザーは、メモ フォルダー内のアイテムを読み取ることができます。</span><span class="sxs-lookup"><span data-stu-id="7dabe-128">The delegate user can read items in the Notes folder.</span></span>  <br/> |
|<span data-ttu-id="7dabe-129">作成者</span><span class="sxs-lookup"><span data-stu-id="7dabe-129">Author</span></span>  <br/> |<span data-ttu-id="7dabe-130">代理ユーザーは、読み取りし、メモ フォルダー内のアイテムを作成できます。</span><span class="sxs-lookup"><span data-stu-id="7dabe-130">The delegate user can read and create items in the Notes folder.</span></span>  <br/> |
|<span data-ttu-id="7dabe-131">Editor</span><span class="sxs-lookup"><span data-stu-id="7dabe-131">Editor</span></span>  <br/> |<span data-ttu-id="7dabe-132">代理ユーザーは読み取り、作成、およびメモ フォルダー内の項目を変更します。</span><span class="sxs-lookup"><span data-stu-id="7dabe-132">The delegate user can read, create, and modify items in the Notes folder.</span></span>  <br/> |
|<span data-ttu-id="7dabe-133">カスタム</span><span class="sxs-lookup"><span data-stu-id="7dabe-133">Custom</span></span>  <br/> |<span data-ttu-id="7dabe-134">代理ユーザーは、メモ フォルダーにカスタム アクセス許可を持ちます。</span><span class="sxs-lookup"><span data-stu-id="7dabe-134">The delegate user has custom access permissions to the Notes folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7dabe-135">備考</span><span class="sxs-lookup"><span data-stu-id="7dabe-135">Remarks</span></span>

<span data-ttu-id="7dabe-136">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="7dabe-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7dabe-137">要素情報</span><span class="sxs-lookup"><span data-stu-id="7dabe-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7dabe-138">名前空間</span><span class="sxs-lookup"><span data-stu-id="7dabe-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7dabe-139">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7dabe-139">Schema Name</span></span>  <br/> |<span data-ttu-id="7dabe-140">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="7dabe-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="7dabe-141">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7dabe-141">Validation File</span></span>  <br/> |<span data-ttu-id="7dabe-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7dabe-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7dabe-143">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7dabe-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="7dabe-144">False</span><span class="sxs-lookup"><span data-stu-id="7dabe-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7dabe-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="7dabe-145">See also</span></span>



[<span data-ttu-id="7dabe-146">AddDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="7dabe-146">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="7dabe-147">UpdateDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="7dabe-147">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="7dabe-148">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="7dabe-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="7dabe-149">デリゲートを追加します。</span><span class="sxs-lookup"><span data-stu-id="7dabe-149">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

