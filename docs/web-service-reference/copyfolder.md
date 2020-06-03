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
description: CopyFolder 要素は、Exchange ストア内のメールボックスにフォルダーをコピーする要求を定義します。
ms.openlocfilehash: fa75272540169a96d5567181d27b8a8f056cce42
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44452511"
---
# <a name="copyfolder"></a><span data-ttu-id="5cdb5-103">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="5cdb5-103">CopyFolder</span></span>

<span data-ttu-id="5cdb5-104">**Copyfolder**要素は、Exchange ストア内のメールボックスにフォルダーをコピーする要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="5cdb5-104">The **CopyFolder** element defines a request to copy folders in a mailbox in the Exchange store.</span></span> 
  
```xml
<CopyFolder>
   <ToFolderId/>
   <FolderIds/>
</CopyFolder>
```

 <span data-ttu-id="5cdb5-105">**CopyFolderType**</span><span class="sxs-lookup"><span data-stu-id="5cdb5-105">**CopyFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5cdb5-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="5cdb5-106">Attributes and elements</span></span>

<span data-ttu-id="5cdb5-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5cdb5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5cdb5-108">属性</span><span class="sxs-lookup"><span data-stu-id="5cdb5-108">Attributes</span></span>

<span data-ttu-id="5cdb5-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5cdb5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5cdb5-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5cdb5-110">Child elements</span></span>

|<span data-ttu-id="5cdb5-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="5cdb5-111">**Element**</span></span>|<span data-ttu-id="5cdb5-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="5cdb5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5cdb5-113">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="5cdb5-113">ToFolderId</span></span>](tofolderid.md) <br/> |<span data-ttu-id="5cdb5-114">コピー先のフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="5cdb5-114">Represents the destination folder for a copied folder.</span></span>  <br/> |
|[<span data-ttu-id="5cdb5-115">FolderIds</span><span class="sxs-lookup"><span data-stu-id="5cdb5-115">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="5cdb5-116">[ToFolderId](tofolderid.md)要素によって識別されるフォルダーにコピーするフォルダーの配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="5cdb5-116">Contains an array of folders to copy to the folder identified by the [ToFolderId](tofolderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5cdb5-117">親要素</span><span class="sxs-lookup"><span data-stu-id="5cdb5-117">Parent elements</span></span>

<span data-ttu-id="5cdb5-118">なし。</span><span class="sxs-lookup"><span data-stu-id="5cdb5-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5cdb5-119">注釈</span><span class="sxs-lookup"><span data-stu-id="5cdb5-119">Remarks</span></span>

<span data-ttu-id="5cdb5-120">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="5cdb5-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5cdb5-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="5cdb5-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5cdb5-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="5cdb5-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5cdb5-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5cdb5-123">Schema Name</span></span>  <br/> |<span data-ttu-id="5cdb5-124">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="5cdb5-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5cdb5-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5cdb5-125">Validation File</span></span>  <br/> |<span data-ttu-id="5cdb5-126">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="5cdb5-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5cdb5-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5cdb5-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="5cdb5-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="5cdb5-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5cdb5-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="5cdb5-129">See also</span></span>



[<span data-ttu-id="5cdb5-130">CopyFolder 操作</span><span class="sxs-lookup"><span data-stu-id="5cdb5-130">CopyFolder operation</span></span>](copyfolder-operation.md)

