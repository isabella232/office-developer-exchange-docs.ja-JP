---
title: (フォルダー) の更新
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
description: 更新プログラム要素を定義する要素のセットが含まれています。 追加、設定、およびフォルダーのプロパティへの変更を削除します。
ms.openlocfilehash: 31f25b1e88fb8756f189a6d75259dd4fc198582f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839891"
---
# <a name="updates-folder"></a><span data-ttu-id="a600b-103">(フォルダー) の更新</span><span class="sxs-lookup"><span data-stu-id="a600b-103">Updates (Folder)</span></span>

<span data-ttu-id="a600b-104">**更新プログラム**要素を定義する要素のセットが含まれています。 追加、設定、およびフォルダーのプロパティへの変更を削除します。</span><span class="sxs-lookup"><span data-stu-id="a600b-104">The **Updates** element contains a set of elements that define append, set, and delete changes to folder properties.</span></span> 
  
- [<span data-ttu-id="a600b-105">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="a600b-105">UpdateFolder</span></span>](updatefolder.md)
  
- [<span data-ttu-id="a600b-106">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="a600b-106">FolderChanges</span></span>](folderchanges.md)
  
- [<span data-ttu-id="a600b-107">FolderChange</span><span class="sxs-lookup"><span data-stu-id="a600b-107">FolderChange</span></span>](folderchange.md)
  
- [<span data-ttu-id="a600b-108">(フォルダー) の更新</span><span class="sxs-lookup"><span data-stu-id="a600b-108">Updates (Folder)</span></span>](updates-folder.md)
  
```xml
<Updates>
   <AppendToFolderField/>
   <SetFolderField/>
   <DeleteFolderField/>
</Updates>
```

<span data-ttu-id="a600b-109">**NonEmptyArrayOfFolderChangeDescriptionsType**</span><span class="sxs-lookup"><span data-stu-id="a600b-109">**NonEmptyArrayOfFolderChangeDescriptionsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a600b-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a600b-110">Attributes and elements</span></span>

<span data-ttu-id="a600b-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a600b-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a600b-112">属性</span><span class="sxs-lookup"><span data-stu-id="a600b-112">Attributes</span></span>

<span data-ttu-id="a600b-113">なし。</span><span class="sxs-lookup"><span data-stu-id="a600b-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a600b-114">子要素</span><span class="sxs-lookup"><span data-stu-id="a600b-114">Child elements</span></span>

|<span data-ttu-id="a600b-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="a600b-115">**Element**</span></span>|<span data-ttu-id="a600b-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="a600b-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a600b-117">AppendToFolderField</span><span class="sxs-lookup"><span data-stu-id="a600b-117">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="a600b-118">[UpdateFolder 操作](updatefolder-operation.md)中にフォルダーのプロパティを追加するデータを表します。</span><span class="sxs-lookup"><span data-stu-id="a600b-118">Represents data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="a600b-119">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="a600b-119">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="a600b-120">[UpdateFolder 操作](updatefolder-operation.md)でフォルダーの 1 つのプロパティには、更新プログラムを表します。</span><span class="sxs-lookup"><span data-stu-id="a600b-120">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="a600b-121">DeleteFolderField</span><span class="sxs-lookup"><span data-stu-id="a600b-121">DeleteFolderField</span></span>](deletefolderfield.md) <br/> |<span data-ttu-id="a600b-122">[UpdateFolder 操作](updatefolder-operation.md)中に、フォルダーから特定のプロパティを削除する操作を表します。</span><span class="sxs-lookup"><span data-stu-id="a600b-122">Represents an operation to delete a given property from a folder during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a600b-123">親要素</span><span class="sxs-lookup"><span data-stu-id="a600b-123">Parent elements</span></span>

|<span data-ttu-id="a600b-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="a600b-124">**Element**</span></span>|<span data-ttu-id="a600b-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="a600b-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a600b-126">FolderChange</span><span class="sxs-lookup"><span data-stu-id="a600b-126">FolderChange</span></span>](folderchange.md) <br/> |<span data-ttu-id="a600b-127">1 つのフォルダーで実行される変更のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="a600b-127">Represents a collection of changes to be performed on a single folder.</span></span>  <br/> <span data-ttu-id="a600b-128">この要素への XPath 式は、次のようにします。`/UpdateFolder/FolderChanges/FolderChange[i]`</span><span class="sxs-lookup"><span data-stu-id="a600b-128">The following is the XPath expression to this element:  `/UpdateFolder/FolderChanges/FolderChange[i]`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a600b-129">備考</span><span class="sxs-lookup"><span data-stu-id="a600b-129">Remarks</span></span>

<span data-ttu-id="a600b-130">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="a600b-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a600b-131">要素情報</span><span class="sxs-lookup"><span data-stu-id="a600b-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a600b-132">名前空間</span><span class="sxs-lookup"><span data-stu-id="a600b-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a600b-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a600b-133">Schema Name</span></span>  <br/> |<span data-ttu-id="a600b-134">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="a600b-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="a600b-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a600b-135">Validation File</span></span>  <br/> |<span data-ttu-id="a600b-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a600b-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a600b-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a600b-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="a600b-138">False</span><span class="sxs-lookup"><span data-stu-id="a600b-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a600b-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="a600b-139">See also</span></span>

- <span data-ttu-id="a600b-140">
  [UpdateFolder 操作](updatefolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="a600b-140">[UpdateFolder operation](updatefolder-operation.md)</span></span>
- [<span data-ttu-id="a600b-141">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="a600b-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

