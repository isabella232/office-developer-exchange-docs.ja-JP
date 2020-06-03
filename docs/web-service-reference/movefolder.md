---
title: MoveFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveFolder
api_type:
- schema
ms.assetid: f2bb0a73-94d7-4bc7-8902-bd9c69120221
description: MoveFolder 要素は、Exchange ストア内のフォルダーを移動する要求を定義します。
ms.openlocfilehash: d2fe33a6d7893d45fa116a1516fcc6ab2dea3bcf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457292"
---
# <a name="movefolder"></a><span data-ttu-id="27a5c-103">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="27a5c-103">MoveFolder</span></span>

<span data-ttu-id="27a5c-104">**Movefolder**要素は、Exchange ストア内のフォルダーを移動する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="27a5c-104">The **MoveFolder** element defines a request to move a folder in the Exchange store.</span></span> 
  
```xml
<MoveFolder>
   <ToFolderId/>
   <FolderIds/>
</MoveFolder>
```

 <span data-ttu-id="27a5c-105">**MoveFolderType**</span><span class="sxs-lookup"><span data-stu-id="27a5c-105">**MoveFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="27a5c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="27a5c-106">Attributes and elements</span></span>

<span data-ttu-id="27a5c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="27a5c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="27a5c-108">属性</span><span class="sxs-lookup"><span data-stu-id="27a5c-108">Attributes</span></span>

<span data-ttu-id="27a5c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="27a5c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="27a5c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="27a5c-110">Child elements</span></span>

|<span data-ttu-id="27a5c-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="27a5c-111">**Element**</span></span>|<span data-ttu-id="27a5c-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="27a5c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="27a5c-113">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="27a5c-113">ToFolderId</span></span>](tofolderid.md) <br/> |<span data-ttu-id="27a5c-114">移動先フォルダーのフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="27a5c-114">Represents the destination folder for a moved folder.</span></span>  <br/> |
|[<span data-ttu-id="27a5c-115">FolderIds</span><span class="sxs-lookup"><span data-stu-id="27a5c-115">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="27a5c-116">[ToFolderId](tofolderid.md)要素によって識別されるフォルダーに移動するフォルダーの配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="27a5c-116">Contains an array of folders to move to the folder identified by the [ToFolderId](tofolderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="27a5c-117">親要素</span><span class="sxs-lookup"><span data-stu-id="27a5c-117">Parent elements</span></span>

<span data-ttu-id="27a5c-118">なし。</span><span class="sxs-lookup"><span data-stu-id="27a5c-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="27a5c-119">注釈</span><span class="sxs-lookup"><span data-stu-id="27a5c-119">Remarks</span></span>

<span data-ttu-id="27a5c-120">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="27a5c-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="27a5c-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="27a5c-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="27a5c-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="27a5c-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="27a5c-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="27a5c-123">Schema Name</span></span>  <br/> |<span data-ttu-id="27a5c-124">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="27a5c-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="27a5c-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="27a5c-125">Validation File</span></span>  <br/> |<span data-ttu-id="27a5c-126">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="27a5c-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="27a5c-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="27a5c-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="27a5c-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="27a5c-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="27a5c-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="27a5c-129">See also</span></span>



[<span data-ttu-id="27a5c-130">MoveFolder 操作</span><span class="sxs-lookup"><span data-stu-id="27a5c-130">MoveFolder operation</span></span>](movefolder-operation.md)

