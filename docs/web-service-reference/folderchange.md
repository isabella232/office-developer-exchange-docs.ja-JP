---
title: FolderChange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderChange
api_type:
- schema
ms.assetid: 23279750-131b-4e1a-b7d1-be235c4e0891
description: FolderChange 要素は、1 つのフォルダーで実行される変更のコレクションを表します。
ms.openlocfilehash: 3f8b42ff4ac88eaef53d1d4ec1d61212bc14b8c7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760563"
---
# <a name="folderchange"></a><span data-ttu-id="d5234-103">FolderChange</span><span class="sxs-lookup"><span data-stu-id="d5234-103">FolderChange</span></span>

<span data-ttu-id="d5234-104">**FolderChange**要素は、1 つのフォルダーで実行される変更のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="d5234-104">The **FolderChange** element represents a collection of changes to be performed on a single folder.</span></span> 
  
[<span data-ttu-id="d5234-105">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="d5234-105">UpdateFolder</span></span>](updatefolder.md)
  
[<span data-ttu-id="d5234-106">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="d5234-106">FolderChanges</span></span>](folderchanges.md)
  
[<span data-ttu-id="d5234-107">FolderChange</span><span class="sxs-lookup"><span data-stu-id="d5234-107">FolderChange</span></span>](folderchange.md)
  
```xml
<FolderChange>
   <FolderId/>
   <Updates/>
</FolderChange>
```

 <span data-ttu-id="d5234-108">**FolderChangeType**</span><span class="sxs-lookup"><span data-stu-id="d5234-108">**FolderChangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d5234-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d5234-109">Attributes and elements</span></span>

<span data-ttu-id="d5234-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d5234-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d5234-111">属性</span><span class="sxs-lookup"><span data-stu-id="d5234-111">Attributes</span></span>

<span data-ttu-id="d5234-112">なし。</span><span class="sxs-lookup"><span data-stu-id="d5234-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d5234-113">子要素</span><span class="sxs-lookup"><span data-stu-id="d5234-113">Child elements</span></span>

|<span data-ttu-id="d5234-114">**要素**</span><span class="sxs-lookup"><span data-stu-id="d5234-114">**Element**</span></span>|<span data-ttu-id="d5234-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="d5234-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d5234-116">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="d5234-116">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="d5234-117">更新するフォルダーの識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="d5234-117">Contains the identifier and change key of a folder to update.</span></span>  <br/> |
|[<span data-ttu-id="d5234-118">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="d5234-118">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="d5234-119">名前で参照することができます MicrosoftExchange Server 2007 フォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="d5234-119">Identifies MicrosoftExchange Server 2007 folders that can be referenced by name.</span></span>  <br/> |
|[<span data-ttu-id="d5234-120">(フォルダー) の更新</span><span class="sxs-lookup"><span data-stu-id="d5234-120">Updates (Folder)</span></span>](updates-folder.md) <br/> |<span data-ttu-id="d5234-121">[フォルダー Id](folderid.md)または[DistinguishedFolderId](distinguishedfolderid.md)のいずれかの要素によって指定されているフォルダーに対して実行される更新の種類を定義します。</span><span class="sxs-lookup"><span data-stu-id="d5234-121">Defines the type of update that is performed on a folder that is identified by either the [FolderId](folderid.md) or [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d5234-122">親要素</span><span class="sxs-lookup"><span data-stu-id="d5234-122">Parent elements</span></span>

|<span data-ttu-id="d5234-123">**要素**</span><span class="sxs-lookup"><span data-stu-id="d5234-123">**Element**</span></span>|<span data-ttu-id="d5234-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="d5234-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d5234-125">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="d5234-125">FolderChanges</span></span>](folderchanges.md) <br/> |<span data-ttu-id="d5234-126">フォルダーの変更のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="d5234-126">Represents a collection of changes for a folder.</span></span>  <br/> <span data-ttu-id="d5234-127">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="d5234-127">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateFolder/FolderChanges` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d5234-128">備考</span><span class="sxs-lookup"><span data-stu-id="d5234-128">Remarks</span></span>

<span data-ttu-id="d5234-129">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="d5234-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d5234-130">要素情報</span><span class="sxs-lookup"><span data-stu-id="d5234-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d5234-131">名前空間</span><span class="sxs-lookup"><span data-stu-id="d5234-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d5234-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d5234-132">Schema name</span></span>  <br/> |<span data-ttu-id="d5234-133">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="d5234-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="d5234-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d5234-134">Validation file</span></span>  <br/> |<span data-ttu-id="d5234-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d5234-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d5234-136">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d5234-136">Can be empty</span></span>  <br/> |<span data-ttu-id="d5234-137">False</span><span class="sxs-lookup"><span data-stu-id="d5234-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d5234-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="d5234-138">See also</span></span>



<span data-ttu-id="d5234-139">
  [UpdateFolder 操作](updatefolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="d5234-139">[UpdateFolder operation](updatefolder-operation.md)</span></span>

