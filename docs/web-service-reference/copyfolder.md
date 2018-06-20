---
title: CopyFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyFolder
api_type:
- schema
ms.assetid: 7d5cd08a-fe81-4cb6-a5a0-6dec2d3c93d4
description: CopyFolder 要素は、Exchange ストア内のメールボックスでフォルダーをコピーするための要求を定義します。
ms.openlocfilehash: 7bcfcc7f4212b3a3bd339fa5863df2990eb20d6d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759780"
---
# <a name="copyfolder"></a><span data-ttu-id="e45d3-103">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="e45d3-103">CopyFolder</span></span>

<span data-ttu-id="e45d3-104">**CopyFolder**要素は、Exchange ストア内のメールボックスでフォルダーをコピーするための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="e45d3-104">The **CopyFolder** element defines a request to copy folders in a mailbox in the Exchange store.</span></span> 
  
```xml
<CopyFolder>
   <ToFolderId/>
   <FolderIds/>
</CopyFolder>
```

 <span data-ttu-id="e45d3-105">**CopyFolderType**</span><span class="sxs-lookup"><span data-stu-id="e45d3-105">**CopyFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e45d3-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e45d3-106">Attributes and elements</span></span>

<span data-ttu-id="e45d3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e45d3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e45d3-108">属性</span><span class="sxs-lookup"><span data-stu-id="e45d3-108">Attributes</span></span>

<span data-ttu-id="e45d3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e45d3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e45d3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e45d3-110">Child elements</span></span>

|<span data-ttu-id="e45d3-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="e45d3-111">**Element**</span></span>|<span data-ttu-id="e45d3-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="e45d3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e45d3-113">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="e45d3-113">ToFolderId</span></span>](tofolderid.md) <br/> |<span data-ttu-id="e45d3-114">コピーしたフォルダーのコピー先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="e45d3-114">Represents the destination folder for a copied folder.</span></span>  <br/> |
|[<span data-ttu-id="e45d3-115">FolderIds</span><span class="sxs-lookup"><span data-stu-id="e45d3-115">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="e45d3-116">[ToFolderId](tofolderid.md)要素で指定されたフォルダーにコピーするフォルダーの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e45d3-116">Contains an array of folders to copy to the folder identified by the [ToFolderId](tofolderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e45d3-117">親要素</span><span class="sxs-lookup"><span data-stu-id="e45d3-117">Parent elements</span></span>

<span data-ttu-id="e45d3-118">なし。</span><span class="sxs-lookup"><span data-stu-id="e45d3-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e45d3-119">備考</span><span class="sxs-lookup"><span data-stu-id="e45d3-119">Remarks</span></span>

<span data-ttu-id="e45d3-120">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="e45d3-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e45d3-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="e45d3-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e45d3-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="e45d3-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e45d3-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e45d3-123">Schema Name</span></span>  <br/> |<span data-ttu-id="e45d3-124">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="e45d3-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e45d3-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e45d3-125">Validation File</span></span>  <br/> |<span data-ttu-id="e45d3-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e45d3-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e45d3-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e45d3-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="e45d3-128">False</span><span class="sxs-lookup"><span data-stu-id="e45d3-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e45d3-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="e45d3-129">See also</span></span>



[<span data-ttu-id="e45d3-130">CopyFolder 操作</span><span class="sxs-lookup"><span data-stu-id="e45d3-130">CopyFolder operation</span></span>](copyfolder-operation.md)

