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
description: FolderChange 要素は、1つのフォルダーに対して実行される変更のコレクションを表します。
ms.openlocfilehash: e4a025bef100fdd478be545b6448b15886e47c60
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530240"
---
# <a name="folderchange"></a><span data-ttu-id="aefa1-103">FolderChange</span><span class="sxs-lookup"><span data-stu-id="aefa1-103">FolderChange</span></span>

<span data-ttu-id="aefa1-104">**Folderchange**要素は、1つのフォルダーに対して実行される変更のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="aefa1-104">The **FolderChange** element represents a collection of changes to be performed on a single folder.</span></span> 
  
- [<span data-ttu-id="aefa1-105">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="aefa1-105">UpdateFolder</span></span>](updatefolder.md) 
- [<span data-ttu-id="aefa1-106">FolderChanges 変更</span><span class="sxs-lookup"><span data-stu-id="aefa1-106">FolderChanges</span></span>](folderchanges.md) 
- [<span data-ttu-id="aefa1-107">FolderChange</span><span class="sxs-lookup"><span data-stu-id="aefa1-107">FolderChange</span></span>](folderchange.md)
  
```xml
<FolderChange>
   <FolderId/>
   <Updates/>
</FolderChange>
```

```xml
<FolderChange>
   <DistinguishedFolderId/>
   <Updates/>
</FolderChange>
```

<span data-ttu-id="aefa1-108">**FolderChangeType**</span><span class="sxs-lookup"><span data-stu-id="aefa1-108">**FolderChangeType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="aefa1-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="aefa1-109">Attributes and elements</span></span>

<span data-ttu-id="aefa1-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="aefa1-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aefa1-111">属性</span><span class="sxs-lookup"><span data-stu-id="aefa1-111">Attributes</span></span>

<span data-ttu-id="aefa1-112">なし。</span><span class="sxs-lookup"><span data-stu-id="aefa1-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aefa1-113">子要素</span><span class="sxs-lookup"><span data-stu-id="aefa1-113">Child elements</span></span>

|<span data-ttu-id="aefa1-114">**Element**</span><span class="sxs-lookup"><span data-stu-id="aefa1-114">**Element**</span></span>|<span data-ttu-id="aefa1-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="aefa1-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aefa1-116">FolderId</span><span class="sxs-lookup"><span data-stu-id="aefa1-116">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="aefa1-117">更新するフォルダーの識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="aefa1-117">Contains the identifier and change key of a folder to update.</span></span>  <br/> |
|[<span data-ttu-id="aefa1-118">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="aefa1-118">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="aefa1-119">名前で参照できる Microsoft Exchange Server 2007 フォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="aefa1-119">Identifies MicrosoftExchange Server 2007 folders that can be referenced by name.</span></span>  <br/> |
|[<span data-ttu-id="aefa1-120">Updates (フォルダー)</span><span class="sxs-lookup"><span data-stu-id="aefa1-120">Updates (Folder)</span></span>](updates-folder.md) <br/> |<span data-ttu-id="aefa1-121">[FolderId](folderid.md)または[DistinguishedFolderId](distinguishedfolderid.md)のいずれかの要素によって識別されるフォルダーに対して実行される更新の種類を定義します。</span><span class="sxs-lookup"><span data-stu-id="aefa1-121">Defines the type of update that is performed on a folder that is identified by either the [FolderId](folderid.md) or [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aefa1-122">親要素</span><span class="sxs-lookup"><span data-stu-id="aefa1-122">Parent elements</span></span>

|<span data-ttu-id="aefa1-123">**要素**</span><span class="sxs-lookup"><span data-stu-id="aefa1-123">**Element**</span></span>|<span data-ttu-id="aefa1-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="aefa1-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aefa1-125">FolderChanges 変更</span><span class="sxs-lookup"><span data-stu-id="aefa1-125">FolderChanges</span></span>](folderchanges.md) <br/> |<span data-ttu-id="aefa1-126">フォルダーに対する変更のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="aefa1-126">Represents a collection of changes for a folder.</span></span>  <br/> <span data-ttu-id="aefa1-127">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="aefa1-127">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateFolder/FolderChanges` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="aefa1-128">注釈</span><span class="sxs-lookup"><span data-stu-id="aefa1-128">Remarks</span></span>

<span data-ttu-id="aefa1-129">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="aefa1-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aefa1-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="aefa1-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aefa1-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="aefa1-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="aefa1-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="aefa1-132">Schema name</span></span>  <br/> |<span data-ttu-id="aefa1-133">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="aefa1-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="aefa1-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="aefa1-134">Validation file</span></span>  <br/> |<span data-ttu-id="aefa1-135">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="aefa1-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="aefa1-136">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="aefa1-136">Can be empty</span></span>  <br/> |<span data-ttu-id="aefa1-137">正しくない</span><span class="sxs-lookup"><span data-stu-id="aefa1-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aefa1-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="aefa1-138">See also</span></span>

- [<span data-ttu-id="aefa1-139">UpdateFolder 操作</span><span class="sxs-lookup"><span data-stu-id="aefa1-139">UpdateFolder operation</span></span>](updatefolder-operation.md)

