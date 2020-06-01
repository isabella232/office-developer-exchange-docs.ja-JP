---
title: DeleteFolderField
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteFolderField
api_type:
- schema
ms.assetid: f9c2187b-4c60-4358-b4b4-ede50eadae48
description: DeleteFolderField 要素は、UpdateFolder 呼び出しの実行中にフォルダーから特定のプロパティを削除する操作を表します。
ms.openlocfilehash: a0b48b667c8c8afbd5729d5deb84359a6a6ccc25
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462158"
---
# <a name="deletefolderfield"></a><span data-ttu-id="11766-103">DeleteFolderField</span><span class="sxs-lookup"><span data-stu-id="11766-103">DeleteFolderField</span></span>

<span data-ttu-id="11766-104">**Deletefolderfield**要素は、updatefolder 呼び出しの実行中にフォルダーから特定のプロパティを削除する操作を表します。</span><span class="sxs-lookup"><span data-stu-id="11766-104">The **DeleteFolderField** element represents an operation to delete a given property from a folder during an UpdateFolder call.</span></span> 
  
- [<span data-ttu-id="11766-105">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="11766-105">UpdateFolder</span></span>](updatefolder.md) 
- [<span data-ttu-id="11766-106">FolderChanges 変更</span><span class="sxs-lookup"><span data-stu-id="11766-106">FolderChanges</span></span>](folderchanges.md)  
- [<span data-ttu-id="11766-107">FolderChange</span><span class="sxs-lookup"><span data-stu-id="11766-107">FolderChange</span></span>](folderchange.md)  
- [<span data-ttu-id="11766-108">Updates (フォルダー)</span><span class="sxs-lookup"><span data-stu-id="11766-108">Updates (Folder)</span></span>](updates-folder.md) 
- [<span data-ttu-id="11766-109">DeleteFolderField</span><span class="sxs-lookup"><span data-stu-id="11766-109">DeleteFolderField</span></span>](deletefolderfield.md)
  
```xml
<DeleteFolderField>
   <FieldURI/>
</DeleteFolderField>
```

```xml
<DeleteFolderField>
   <ExtendedFieldURI/>
</DeleteFolderField>
```

```xml
<DeleteFolderField>
   <IndexedFieldURI/>
</DeleteFolderField>
```

<span data-ttu-id="11766-110">**DeleteFolderFieldType**</span><span class="sxs-lookup"><span data-stu-id="11766-110">**DeleteFolderFieldType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="11766-111">属性と要素</span><span class="sxs-lookup"><span data-stu-id="11766-111">Attributes and elements</span></span>

<span data-ttu-id="11766-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="11766-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="11766-113">属性</span><span class="sxs-lookup"><span data-stu-id="11766-113">Attributes</span></span>

<span data-ttu-id="11766-114">なし。</span><span class="sxs-lookup"><span data-stu-id="11766-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="11766-115">子要素</span><span class="sxs-lookup"><span data-stu-id="11766-115">Child elements</span></span>

|<span data-ttu-id="11766-116">**Element**</span><span class="sxs-lookup"><span data-stu-id="11766-116">**Element**</span></span>|<span data-ttu-id="11766-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="11766-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="11766-118">FieldURI</span><span class="sxs-lookup"><span data-stu-id="11766-118">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="11766-119">URI で頻繁に参照されるプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="11766-119">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="11766-120">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="11766-120">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="11766-121">Dictionary プロパティの個々のメンバーを識別します。</span><span class="sxs-lookup"><span data-stu-id="11766-121">Identifies individual members of a dictionary property.</span></span>  <br/> |
|[<span data-ttu-id="11766-122">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="11766-122">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="11766-123">拡張 MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="11766-123">Identifies extended MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="11766-124">親要素</span><span class="sxs-lookup"><span data-stu-id="11766-124">Parent elements</span></span>

|<span data-ttu-id="11766-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="11766-125">**Element**</span></span>|<span data-ttu-id="11766-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="11766-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="11766-127">Updates (フォルダー)</span><span class="sxs-lookup"><span data-stu-id="11766-127">Updates (Folder)</span></span>](updates-folder.md) <br/> |<span data-ttu-id="11766-128">フォルダーのプロパティに対する追加、設定、および削除の変更を定義する一連の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="11766-128">Contains a set of elements that define append, set, and delete changes to folder properties.</span></span>  <br/> <span data-ttu-id="11766-129">この要素の XPath 式を次に示します。`/UpdateFolder/FolderChanges/FolderChange[i]/Updates`</span><span class="sxs-lookup"><span data-stu-id="11766-129">The following is the XPath expression to this element:  `/UpdateFolder/FolderChanges/FolderChange[i]/Updates`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="11766-130">注釈</span><span class="sxs-lookup"><span data-stu-id="11766-130">Remarks</span></span>

<span data-ttu-id="11766-131">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="11766-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="11766-132">要素の情報</span><span class="sxs-lookup"><span data-stu-id="11766-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="11766-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="11766-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="11766-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="11766-134">Schema Name</span></span>  <br/> |<span data-ttu-id="11766-135">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="11766-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="11766-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="11766-136">Validation File</span></span>  <br/> |<span data-ttu-id="11766-137">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="11766-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="11766-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="11766-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="11766-139">正しくない</span><span class="sxs-lookup"><span data-stu-id="11766-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="11766-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="11766-140">See also</span></span>

- <span data-ttu-id="11766-141">
  [UpdateFolder 操作](updatefolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="11766-141">[UpdateFolder operation](updatefolder-operation.md)</span></span>

