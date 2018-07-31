---
title: ParentFolderId (TargetFolderIdType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ParentFolderId
api_type:
- schema
ms.assetid: 0e3e6e5f-06d0-499b-8ca4-d36036521658
description: ParentFolderId 要素内のフォルダーを識別する新しいフォルダーを作成するか、FindConversation の操作を検索するフォルダーです。
ms.openlocfilehash: 8e80b9b342274a8b2004838ebd16f8425a2d3fa3
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353827"
---
# <a name="parentfolderid-targetfolderidtype"></a><span data-ttu-id="094b3-103">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="094b3-103">ParentFolderId (TargetFolderIdType)</span></span>

<span data-ttu-id="094b3-104">**ParentFolderId**要素内のフォルダーを識別する新しいフォルダーを作成または[操作の FindConversation](findconversation-operation.md)を検索するフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="094b3-104">The **ParentFolderId** element identifies the folder in which a new folder is created or the folder to search for the [FindConversation operation](findconversation-operation.md).</span></span>
  
```xml
<ParentFolderId>
   <DistinguishedFolderId/>
</ParentFolderId>
```

```xml
<ParentFolderId>
   <FolderId/> 
</ParentFolderId>
```

<span data-ttu-id="094b3-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="094b3-105">**TargetFolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="094b3-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="094b3-106">Attributes and elements</span></span>

<span data-ttu-id="094b3-107">**ParentFolderId**要素には、2 つの子要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="094b3-107">The **ParentFolderId** element contains two child elements.</span></span> <span data-ttu-id="094b3-108">子要素は、スキーマ内で相互に排他的です。</span><span class="sxs-lookup"><span data-stu-id="094b3-108">The child elements are mutually exclusive in the schema.</span></span> 
  
### <a name="attributes"></a><span data-ttu-id="094b3-109">属性</span><span class="sxs-lookup"><span data-stu-id="094b3-109">Attributes</span></span>

<span data-ttu-id="094b3-110">なし。</span><span class="sxs-lookup"><span data-stu-id="094b3-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="094b3-111">子要素</span><span class="sxs-lookup"><span data-stu-id="094b3-111">Child elements</span></span>

|<span data-ttu-id="094b3-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="094b3-112">**Element**</span></span>|<span data-ttu-id="094b3-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="094b3-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="094b3-114">FolderId</span><span class="sxs-lookup"><span data-stu-id="094b3-114">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="094b3-115">必須の識別子とキーを含む、省略可能な変更でフォルダーの新しいフォルダーを作成または[FindConversation 操作](findconversation-operation.md)のために検索されるフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="094b3-115">Contains the required identifier and the optional change key of a folder in which a new folder is created or the folder that is searched for the [FindConversation operation](findconversation-operation.md).</span></span> <span data-ttu-id="094b3-116">この要素を使用するには、 [DistinguishedFolderId](distinguishedfolderid.md)要素の使用が含まれません。</span><span class="sxs-lookup"><span data-stu-id="094b3-116">Using this element excludes the use of the [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="094b3-117">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="094b3-117">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="094b3-118">Microsoft Exchange Server 2007 の既定のフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="094b3-118">Identifies default Microsoft Exchange Server 2007 folders.</span></span> <span data-ttu-id="094b3-119">この要素を使用して、[フォルダー Id](folderid.md)要素の使用が除外されます。</span><span class="sxs-lookup"><span data-stu-id="094b3-119">Using this element excludes the use of the [FolderId](folderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="094b3-120">親要素</span><span class="sxs-lookup"><span data-stu-id="094b3-120">Parent elements</span></span>

|<span data-ttu-id="094b3-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="094b3-121">**Element**</span></span>|<span data-ttu-id="094b3-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="094b3-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="094b3-123">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="094b3-123">CreateFolder</span></span>](createfolder.md) <br/> |<span data-ttu-id="094b3-124">Exchange データベース内のフォルダーを作成する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="094b3-124">Defines a request to create a folder in the Exchange database.</span></span>  <br/> <span data-ttu-id="094b3-125">この要素への XPath 式は、次のようにします。`/CreateFolder`</span><span class="sxs-lookup"><span data-stu-id="094b3-125">The following is the XPath expression to this element:  `/CreateFolder`</span></span> <br/> |
|[<span data-ttu-id="094b3-126">FindConversation</span><span class="sxs-lookup"><span data-stu-id="094b3-126">FindConversation</span></span>](findconversation.md) <br/> |<span data-ttu-id="094b3-127">メールボックス内の会話を検索するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="094b3-127">Defines a request to find conversations in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="094b3-128">テキスト値</span><span class="sxs-lookup"><span data-stu-id="094b3-128">Text value</span></span>

<span data-ttu-id="094b3-129">なし。</span><span class="sxs-lookup"><span data-stu-id="094b3-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="094b3-130">注釈</span><span class="sxs-lookup"><span data-stu-id="094b3-130">Remarks</span></span>

<span data-ttu-id="094b3-131">2 つの子要素を使用して、新しいフォルダーを格納するフォルダーを定義します。</span><span class="sxs-lookup"><span data-stu-id="094b3-131">The two child elements are used to define the folder that will contain the new folder.</span></span> <span data-ttu-id="094b3-132">[フォルダー Id](folderid.md)または[DistinguishedFolderId](distinguishedfolderid.md)要素のいずれか、新しいフォルダーの親フォルダーを識別するを選択する必要があります。</span><span class="sxs-lookup"><span data-stu-id="094b3-132">You must select either the [FolderId](folderid.md) or the [DistinguishedFolderId](distinguishedfolderid.md) element to identify the parent folder of the new folder.</span></span> <span data-ttu-id="094b3-133">同時に両方の要素を使用することはできません。</span><span class="sxs-lookup"><span data-stu-id="094b3-133">You cannot use both elements at the same time.</span></span> <span data-ttu-id="094b3-134">この要素は、フォルダーを作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="094b3-134">This element is required to create folders.</span></span> 
  
<span data-ttu-id="094b3-135">[ParentFolderId](parentfolderid.md)要素では、既存のアイテムとフォルダーの場所について説明します。</span><span class="sxs-lookup"><span data-stu-id="094b3-135">The [ParentFolderId](parentfolderid.md) element describes the location of existing items and folders.</span></span> 
  
<span data-ttu-id="094b3-136">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="094b3-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="094b3-137">要素情報</span><span class="sxs-lookup"><span data-stu-id="094b3-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="094b3-138">名前空間</span><span class="sxs-lookup"><span data-stu-id="094b3-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="094b3-139">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="094b3-139">Schema Name</span></span>  <br/> |<span data-ttu-id="094b3-140">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="094b3-140">Message schema</span></span>  <br/> |
|<span data-ttu-id="094b3-141">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="094b3-141">Validation File</span></span>  <br/> |<span data-ttu-id="094b3-142">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="094b3-142">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="094b3-143">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="094b3-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="094b3-144">False</span><span class="sxs-lookup"><span data-stu-id="094b3-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="094b3-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="094b3-145">See also</span></span>

- <span data-ttu-id="094b3-146">
  [CreateFolder 操作](createfolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="094b3-146">[CreateFolder operation](createfolder-operation.md)</span></span>
- [<span data-ttu-id="094b3-147">FindConversation 操作</span><span class="sxs-lookup"><span data-stu-id="094b3-147">FindConversation operation</span></span>](findconversation-operation.md)
- [<span data-ttu-id="094b3-148">フォルダー (Exchange Web サービス) を作成します。</span><span class="sxs-lookup"><span data-stu-id="094b3-148">Creating Folders (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

