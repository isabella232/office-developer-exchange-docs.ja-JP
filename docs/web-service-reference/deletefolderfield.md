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
description: DeleteFolderField 要素は、UpdateFolder の呼び出し中に、フォルダーから特定のプロパティを削除する操作を表します。
ms.openlocfilehash: 60d4a5c19d89c109913e83fea99c2f7910566c72
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354093"
---
# <a name="deletefolderfield"></a><span data-ttu-id="a1416-103">DeleteFolderField</span><span class="sxs-lookup"><span data-stu-id="a1416-103">DeleteFolderField</span></span>

<span data-ttu-id="a1416-104">**DeleteFolderField**要素は、UpdateFolder の呼び出し中に、フォルダーから特定のプロパティを削除する操作を表します。</span><span class="sxs-lookup"><span data-stu-id="a1416-104">The **DeleteFolderField** element represents an operation to delete a given property from a folder during an UpdateFolder call.</span></span> 
  
- [<span data-ttu-id="a1416-105">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="a1416-105">UpdateFolder</span></span>](updatefolder.md) 
- [<span data-ttu-id="a1416-106">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="a1416-106">FolderChanges</span></span>](folderchanges.md)  
- [<span data-ttu-id="a1416-107">FolderChange</span><span class="sxs-lookup"><span data-stu-id="a1416-107">FolderChange</span></span>](folderchange.md)  
- [<span data-ttu-id="a1416-108">Updates (Folder)</span><span class="sxs-lookup"><span data-stu-id="a1416-108">Updates (Folder)</span></span>](updates-folder.md) 
- [<span data-ttu-id="a1416-109">DeleteFolderField</span><span class="sxs-lookup"><span data-stu-id="a1416-109">DeleteFolderField</span></span>](deletefolderfield.md)
  
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

<span data-ttu-id="a1416-110">**DeleteFolderFieldType**</span><span class="sxs-lookup"><span data-stu-id="a1416-110">**DeleteFolderFieldType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a1416-111">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a1416-111">Attributes and elements</span></span>

<span data-ttu-id="a1416-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a1416-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a1416-113">属性</span><span class="sxs-lookup"><span data-stu-id="a1416-113">Attributes</span></span>

<span data-ttu-id="a1416-114">なし。</span><span class="sxs-lookup"><span data-stu-id="a1416-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a1416-115">子要素</span><span class="sxs-lookup"><span data-stu-id="a1416-115">Child elements</span></span>

|<span data-ttu-id="a1416-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="a1416-116">**Element**</span></span>|<span data-ttu-id="a1416-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="a1416-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a1416-118">FieldURI</span><span class="sxs-lookup"><span data-stu-id="a1416-118">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="a1416-119">URI によって頻繁に参照されるプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="a1416-119">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="a1416-120">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="a1416-120">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="a1416-121">ディクショナリ プロパティの個々 のメンバーを識別します。</span><span class="sxs-lookup"><span data-stu-id="a1416-121">Identifies individual members of a dictionary property.</span></span>  <br/> |
|[<span data-ttu-id="a1416-122">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="a1416-122">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="a1416-123">拡張 MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="a1416-123">Identifies extended MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a1416-124">親要素</span><span class="sxs-lookup"><span data-stu-id="a1416-124">Parent elements</span></span>

|<span data-ttu-id="a1416-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="a1416-125">**Element**</span></span>|<span data-ttu-id="a1416-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="a1416-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a1416-127">Updates (Folder)</span><span class="sxs-lookup"><span data-stu-id="a1416-127">Updates (Folder)</span></span>](updates-folder.md) <br/> |<span data-ttu-id="a1416-128">定義する要素のセットが含まれていて、このオプションを設定すると、フォルダーのプロパティへの変更を削除します。</span><span class="sxs-lookup"><span data-stu-id="a1416-128">Contains a set of elements that define append, set, and delete changes to folder properties.</span></span>  <br/> <span data-ttu-id="a1416-129">この要素への XPath 式は、次のようにします。`/UpdateFolder/FolderChanges/FolderChange[i]/Updates`</span><span class="sxs-lookup"><span data-stu-id="a1416-129">The following is the XPath expression to this element:  `/UpdateFolder/FolderChanges/FolderChange[i]/Updates`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a1416-130">注釈</span><span class="sxs-lookup"><span data-stu-id="a1416-130">Remarks</span></span>

<span data-ttu-id="a1416-131">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="a1416-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a1416-132">要素情報</span><span class="sxs-lookup"><span data-stu-id="a1416-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a1416-133">名前空間</span><span class="sxs-lookup"><span data-stu-id="a1416-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a1416-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a1416-134">Schema Name</span></span>  <br/> |<span data-ttu-id="a1416-135">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="a1416-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="a1416-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a1416-136">Validation File</span></span>  <br/> |<span data-ttu-id="a1416-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a1416-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a1416-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a1416-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="a1416-139">False</span><span class="sxs-lookup"><span data-stu-id="a1416-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a1416-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="a1416-140">See also</span></span>

- <span data-ttu-id="a1416-141">
  [UpdateFolder 操作](updatefolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="a1416-141">[UpdateFolder operation](updatefolder-operation.md)</span></span>

