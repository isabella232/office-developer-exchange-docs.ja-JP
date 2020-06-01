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
description: ParentFolderId 要素は、新しいフォルダーを作成するフォルダー、または FindConversation 操作を検索するフォルダーを指定します。
ms.openlocfilehash: 36e63266d10603c4d453a37e2b0d22e02599e516
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467803"
---
# <a name="parentfolderid-targetfolderidtype"></a><span data-ttu-id="eb9aa-103">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="eb9aa-103">ParentFolderId (TargetFolderIdType)</span></span>

<span data-ttu-id="eb9aa-104">**ParentFolderId**要素は、新しいフォルダーを作成するフォルダー、または[findconversation 操作](findconversation-operation.md)を検索するフォルダーを指定します。</span><span class="sxs-lookup"><span data-stu-id="eb9aa-104">The **ParentFolderId** element identifies the folder in which a new folder is created or the folder to search for the [FindConversation operation](findconversation-operation.md).</span></span>
  
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

<span data-ttu-id="eb9aa-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="eb9aa-105">**TargetFolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="eb9aa-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="eb9aa-106">Attributes and elements</span></span>

<span data-ttu-id="eb9aa-107">**ParentFolderId**要素には、2つの子要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="eb9aa-107">The **ParentFolderId** element contains two child elements.</span></span> <span data-ttu-id="eb9aa-108">子要素は、スキーマ内で相互に排他的です。</span><span class="sxs-lookup"><span data-stu-id="eb9aa-108">The child elements are mutually exclusive in the schema.</span></span> 
  
### <a name="attributes"></a><span data-ttu-id="eb9aa-109">属性</span><span class="sxs-lookup"><span data-stu-id="eb9aa-109">Attributes</span></span>

<span data-ttu-id="eb9aa-110">なし。</span><span class="sxs-lookup"><span data-stu-id="eb9aa-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eb9aa-111">子要素</span><span class="sxs-lookup"><span data-stu-id="eb9aa-111">Child elements</span></span>

|<span data-ttu-id="eb9aa-112">**Element**</span><span class="sxs-lookup"><span data-stu-id="eb9aa-112">**Element**</span></span>|<span data-ttu-id="eb9aa-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="eb9aa-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eb9aa-114">FolderId</span><span class="sxs-lookup"><span data-stu-id="eb9aa-114">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="eb9aa-115">新しいフォルダーを作成するフォルダーの必須の識別子と省略可能な change キー、および[Findconversation 操作](findconversation-operation.md)の検索先のフォルダーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="eb9aa-115">Contains the required identifier and the optional change key of a folder in which a new folder is created or the folder that is searched for the [FindConversation operation](findconversation-operation.md).</span></span> <span data-ttu-id="eb9aa-116">この要素を使用すると、 [DistinguishedFolderId](distinguishedfolderid.md)要素の使用は除外されます。</span><span class="sxs-lookup"><span data-stu-id="eb9aa-116">Using this element excludes the use of the [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="eb9aa-117">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="eb9aa-117">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="eb9aa-118">Microsoft Exchange Server 2007 の既定のフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="eb9aa-118">Identifies default Microsoft Exchange Server 2007 folders.</span></span> <span data-ttu-id="eb9aa-119">この要素を使用すると、 [FolderId](folderid.md)要素の使用は除外されます。</span><span class="sxs-lookup"><span data-stu-id="eb9aa-119">Using this element excludes the use of the [FolderId](folderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="eb9aa-120">親要素</span><span class="sxs-lookup"><span data-stu-id="eb9aa-120">Parent elements</span></span>

|<span data-ttu-id="eb9aa-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="eb9aa-121">**Element**</span></span>|<span data-ttu-id="eb9aa-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="eb9aa-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eb9aa-123">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="eb9aa-123">CreateFolder</span></span>](createfolder.md) <br/> |<span data-ttu-id="eb9aa-124">Exchange データベースにフォルダーを作成するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="eb9aa-124">Defines a request to create a folder in the Exchange database.</span></span>  <br/> <span data-ttu-id="eb9aa-125">この要素の XPath 式を次に示します。`/CreateFolder`</span><span class="sxs-lookup"><span data-stu-id="eb9aa-125">The following is the XPath expression to this element:  `/CreateFolder`</span></span> <br/> |
|[<span data-ttu-id="eb9aa-126">FindConversation</span><span class="sxs-lookup"><span data-stu-id="eb9aa-126">FindConversation</span></span>](findconversation.md) <br/> |<span data-ttu-id="eb9aa-127">メールボックス内のスレッドを検索する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="eb9aa-127">Defines a request to find conversations in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="eb9aa-128">テキスト値</span><span class="sxs-lookup"><span data-stu-id="eb9aa-128">Text value</span></span>

<span data-ttu-id="eb9aa-129">なし。</span><span class="sxs-lookup"><span data-stu-id="eb9aa-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="eb9aa-130">注釈</span><span class="sxs-lookup"><span data-stu-id="eb9aa-130">Remarks</span></span>

<span data-ttu-id="eb9aa-131">2つの子要素は、新しいフォルダーを格納するフォルダーを定義するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="eb9aa-131">The two child elements are used to define the folder that will contain the new folder.</span></span> <span data-ttu-id="eb9aa-132">新しいフォルダーの親フォルダーを識別するには、 [FolderId](folderid.md)または[DistinguishedFolderId](distinguishedfolderid.md)のいずれかの要素を選択する必要があります。</span><span class="sxs-lookup"><span data-stu-id="eb9aa-132">You must select either the [FolderId](folderid.md) or the [DistinguishedFolderId](distinguishedfolderid.md) element to identify the parent folder of the new folder.</span></span> <span data-ttu-id="eb9aa-133">両方の要素を同時に使用することはできません。</span><span class="sxs-lookup"><span data-stu-id="eb9aa-133">You cannot use both elements at the same time.</span></span> <span data-ttu-id="eb9aa-134">この要素は、フォルダーを作成するために必要です。</span><span class="sxs-lookup"><span data-stu-id="eb9aa-134">This element is required to create folders.</span></span> 
  
<span data-ttu-id="eb9aa-135">[ParentFolderId](parentfolderid.md)要素は、既存のアイテムとフォルダーの場所を表します。</span><span class="sxs-lookup"><span data-stu-id="eb9aa-135">The [ParentFolderId](parentfolderid.md) element describes the location of existing items and folders.</span></span> 
  
<span data-ttu-id="eb9aa-136">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="eb9aa-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eb9aa-137">要素の情報</span><span class="sxs-lookup"><span data-stu-id="eb9aa-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eb9aa-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="eb9aa-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="eb9aa-139">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="eb9aa-139">Schema Name</span></span>  <br/> |<span data-ttu-id="eb9aa-140">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="eb9aa-140">Message schema</span></span>  <br/> |
|<span data-ttu-id="eb9aa-141">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="eb9aa-141">Validation File</span></span>  <br/> |<span data-ttu-id="eb9aa-142">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="eb9aa-142">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="eb9aa-143">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="eb9aa-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="eb9aa-144">正しくない</span><span class="sxs-lookup"><span data-stu-id="eb9aa-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="eb9aa-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="eb9aa-145">See also</span></span>

- <span data-ttu-id="eb9aa-146">
  [CreateFolder 操作](createfolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="eb9aa-146">[CreateFolder operation](createfolder-operation.md)</span></span>
- [<span data-ttu-id="eb9aa-147">FindConversation 操作</span><span class="sxs-lookup"><span data-stu-id="eb9aa-147">FindConversation operation</span></span>](findconversation-operation.md)
- [<span data-ttu-id="eb9aa-148">フォルダーの作成 (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="eb9aa-148">Creating Folders (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

