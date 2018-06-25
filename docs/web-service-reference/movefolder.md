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
ms.openlocfilehash: 42a990ced18cc13c7694042df786d33c018f346c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832485"
---
# <a name="movefolder"></a><span data-ttu-id="9444b-103">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="9444b-103">MoveFolder</span></span>

<span data-ttu-id="9444b-104">**MoveFolder**要素は、Exchange ストア内のフォルダーを移動する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="9444b-104">The **MoveFolder** element defines a request to move a folder in the Exchange store.</span></span> 
  
```xml
<MoveFolder>
   <ToFolderId/>
   <FolderIds/>
</MoveFolder>
```

 <span data-ttu-id="9444b-105">**MoveFolderType**</span><span class="sxs-lookup"><span data-stu-id="9444b-105">**MoveFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9444b-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9444b-106">Attributes and elements</span></span>

<span data-ttu-id="9444b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9444b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9444b-108">属性</span><span class="sxs-lookup"><span data-stu-id="9444b-108">Attributes</span></span>

<span data-ttu-id="9444b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9444b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9444b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9444b-110">Child elements</span></span>

|<span data-ttu-id="9444b-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="9444b-111">**Element**</span></span>|<span data-ttu-id="9444b-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="9444b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9444b-113">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="9444b-113">ToFolderId</span></span>](tofolderid.md) <br/> |<span data-ttu-id="9444b-114">移動したフォルダーのコピー先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="9444b-114">Represents the destination folder for a moved folder.</span></span>  <br/> |
|[<span data-ttu-id="9444b-115">FolderIds</span><span class="sxs-lookup"><span data-stu-id="9444b-115">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="9444b-116">[ToFolderId](tofolderid.md)要素で指定されたフォルダーに移動するフォルダーの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9444b-116">Contains an array of folders to move to the folder identified by the [ToFolderId](tofolderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9444b-117">親要素</span><span class="sxs-lookup"><span data-stu-id="9444b-117">Parent elements</span></span>

<span data-ttu-id="9444b-118">なし。</span><span class="sxs-lookup"><span data-stu-id="9444b-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9444b-119">備考</span><span class="sxs-lookup"><span data-stu-id="9444b-119">Remarks</span></span>

<span data-ttu-id="9444b-120">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="9444b-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9444b-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="9444b-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9444b-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="9444b-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9444b-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9444b-123">Schema Name</span></span>  <br/> |<span data-ttu-id="9444b-124">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="9444b-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9444b-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9444b-125">Validation File</span></span>  <br/> |<span data-ttu-id="9444b-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9444b-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9444b-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9444b-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="9444b-128">False</span><span class="sxs-lookup"><span data-stu-id="9444b-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9444b-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="9444b-129">See also</span></span>



[<span data-ttu-id="9444b-130">MoveFolder 操作</span><span class="sxs-lookup"><span data-stu-id="9444b-130">MoveFolder operation</span></span>](movefolder-operation.md)

