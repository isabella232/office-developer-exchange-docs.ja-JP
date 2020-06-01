---
title: Updates (フォルダー)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Updates
api_type:
- schema
ms.assetid: b047e3a4-a5ab-4098-b7a0-273bc809e702
description: Updates 要素には、フォルダーのプロパティに対する追加、設定、および削除の変更を定義する一連の要素が含まれています。
ms.openlocfilehash: 3282171dfc188a9d4735a19a97e80fe0e2f79b89
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457180"
---
# <a name="updates-folder"></a><span data-ttu-id="8882b-103">Updates (フォルダー)</span><span class="sxs-lookup"><span data-stu-id="8882b-103">Updates (Folder)</span></span>

<span data-ttu-id="8882b-104">**Updates**要素には、フォルダーのプロパティに対する追加、設定、および削除の変更を定義する一連の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8882b-104">The **Updates** element contains a set of elements that define append, set, and delete changes to folder properties.</span></span> 
  
- [<span data-ttu-id="8882b-105">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="8882b-105">UpdateFolder</span></span>](updatefolder.md)
  
- [<span data-ttu-id="8882b-106">FolderChanges 変更</span><span class="sxs-lookup"><span data-stu-id="8882b-106">FolderChanges</span></span>](folderchanges.md)
  
- [<span data-ttu-id="8882b-107">FolderChange</span><span class="sxs-lookup"><span data-stu-id="8882b-107">FolderChange</span></span>](folderchange.md)
  
- [<span data-ttu-id="8882b-108">Updates (フォルダー)</span><span class="sxs-lookup"><span data-stu-id="8882b-108">Updates (Folder)</span></span>](updates-folder.md)
  
```xml
<Updates>
   <AppendToFolderField/>
   <SetFolderField/>
   <DeleteFolderField/>
</Updates>
```

<span data-ttu-id="8882b-109">**NonEmptyArrayOfFolderChangeDescriptionsType**</span><span class="sxs-lookup"><span data-stu-id="8882b-109">**NonEmptyArrayOfFolderChangeDescriptionsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="8882b-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="8882b-110">Attributes and elements</span></span>

<span data-ttu-id="8882b-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8882b-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8882b-112">属性</span><span class="sxs-lookup"><span data-stu-id="8882b-112">Attributes</span></span>

<span data-ttu-id="8882b-113">なし。</span><span class="sxs-lookup"><span data-stu-id="8882b-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8882b-114">子要素</span><span class="sxs-lookup"><span data-stu-id="8882b-114">Child elements</span></span>

|<span data-ttu-id="8882b-115">**Element**</span><span class="sxs-lookup"><span data-stu-id="8882b-115">**Element**</span></span>|<span data-ttu-id="8882b-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="8882b-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8882b-117">AppendToFolderField</span><span class="sxs-lookup"><span data-stu-id="8882b-117">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="8882b-118">[Updatefolder 操作](updatefolder-operation.md)中に folder プロパティに追加するデータを表します。</span><span class="sxs-lookup"><span data-stu-id="8882b-118">Represents data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="8882b-119">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="8882b-119">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="8882b-120">[Updatefolder 操作](updatefolder-operation.md)のフォルダーの1つのプロパティに対する更新を表します。</span><span class="sxs-lookup"><span data-stu-id="8882b-120">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="8882b-121">DeleteFolderField</span><span class="sxs-lookup"><span data-stu-id="8882b-121">DeleteFolderField</span></span>](deletefolderfield.md) <br/> |<span data-ttu-id="8882b-122">[Updatefolder 操作](updatefolder-operation.md)中にフォルダーから特定のプロパティを削除する操作を表します。</span><span class="sxs-lookup"><span data-stu-id="8882b-122">Represents an operation to delete a given property from a folder during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8882b-123">親要素</span><span class="sxs-lookup"><span data-stu-id="8882b-123">Parent elements</span></span>

|<span data-ttu-id="8882b-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="8882b-124">**Element**</span></span>|<span data-ttu-id="8882b-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="8882b-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8882b-126">FolderChange</span><span class="sxs-lookup"><span data-stu-id="8882b-126">FolderChange</span></span>](folderchange.md) <br/> |<span data-ttu-id="8882b-127">1つのフォルダーに対して実行される変更のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="8882b-127">Represents a collection of changes to be performed on a single folder.</span></span>  <br/> <span data-ttu-id="8882b-128">この要素の XPath 式を次に示します。`/UpdateFolder/FolderChanges/FolderChange[i]`</span><span class="sxs-lookup"><span data-stu-id="8882b-128">The following is the XPath expression to this element:  `/UpdateFolder/FolderChanges/FolderChange[i]`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8882b-129">注釈</span><span class="sxs-lookup"><span data-stu-id="8882b-129">Remarks</span></span>

<span data-ttu-id="8882b-130">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="8882b-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8882b-131">要素の情報</span><span class="sxs-lookup"><span data-stu-id="8882b-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8882b-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="8882b-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8882b-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8882b-133">Schema Name</span></span>  <br/> |<span data-ttu-id="8882b-134">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="8882b-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="8882b-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8882b-135">Validation File</span></span>  <br/> |<span data-ttu-id="8882b-136">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="8882b-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8882b-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="8882b-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="8882b-138">正しくない</span><span class="sxs-lookup"><span data-stu-id="8882b-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8882b-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="8882b-139">See also</span></span>

- <span data-ttu-id="8882b-140">
  [UpdateFolder 操作](updatefolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="8882b-140">[UpdateFolder operation](updatefolder-operation.md)</span></span>
- [<span data-ttu-id="8882b-141">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="8882b-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

