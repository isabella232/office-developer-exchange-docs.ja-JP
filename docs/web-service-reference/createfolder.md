---
title: CreateFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateFolder
api_type:
- schema
ms.assetid: 110bada1-517b-4bd6-870d-7086dc879e5d
description: CreateFolder 要素は、Exchange ストア内のフォルダーを作成する要求を定義します。
ms.openlocfilehash: e30af23b8ed8669053b94be460d62fbf7abf24c9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/21/2018
ms.locfileid: "19759811"
---
# <a name="createfolder"></a><span data-ttu-id="e1da6-103">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="e1da6-103">CreateFolder</span></span>

<span data-ttu-id="e1da6-104">**CreateFolder**要素は、Exchange ストア内のフォルダーを作成する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="e1da6-104">The **CreateFolder** element defines a request to create a folder in the Exchange store.</span></span> 
  
```xml
<CreateFolder>
   <ParentFolderId/>
   <Folders/>
</CreateFolder>
```

 <span data-ttu-id="e1da6-105">**CreateFolderType**</span><span class="sxs-lookup"><span data-stu-id="e1da6-105">**CreateFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e1da6-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e1da6-106">Attributes and elements</span></span>

<span data-ttu-id="e1da6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e1da6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e1da6-108">属性</span><span class="sxs-lookup"><span data-stu-id="e1da6-108">Attributes</span></span>

<span data-ttu-id="e1da6-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e1da6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e1da6-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e1da6-110">Child elements</span></span>

|<span data-ttu-id="e1da6-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="e1da6-111">**Element**</span></span>|<span data-ttu-id="e1da6-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="e1da6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e1da6-113">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="e1da6-113">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md) <br/> |<span data-ttu-id="e1da6-114">新しいフォルダーの作成先の場所を識別する要素です。</span><span class="sxs-lookup"><span data-stu-id="e1da6-114">The element that identifies the location where the new folder is created.</span></span>  <br/> |
|[<span data-ttu-id="e1da6-115">フォルダー</span><span class="sxs-lookup"><span data-stu-id="e1da6-115">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="e1da6-116">要素を作成するすべてのフォルダーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e1da6-116">The element that contains all the folders to create.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e1da6-117">親要素</span><span class="sxs-lookup"><span data-stu-id="e1da6-117">Parent elements</span></span>

<span data-ttu-id="e1da6-118">なし。</span><span class="sxs-lookup"><span data-stu-id="e1da6-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e1da6-119">備考</span><span class="sxs-lookup"><span data-stu-id="e1da6-119">Remarks</span></span>

<span data-ttu-id="e1da6-120">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="e1da6-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e1da6-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="e1da6-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e1da6-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="e1da6-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e1da6-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e1da6-123">Schema Name</span></span>  <br/> |<span data-ttu-id="e1da6-124">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="e1da6-124">Message schema</span></span>  <br/> |
|<span data-ttu-id="e1da6-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e1da6-125">Validation File</span></span>  <br/> |<span data-ttu-id="e1da6-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e1da6-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e1da6-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e1da6-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="e1da6-128">False</span><span class="sxs-lookup"><span data-stu-id="e1da6-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e1da6-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="e1da6-129">See also</span></span>



<span data-ttu-id="e1da6-130">
  [CreateFolder 操作](createfolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="e1da6-130">[CreateFolder operation](createfolder-operation.md)</span></span>


[<span data-ttu-id="e1da6-131">フォルダー (Exchange Web サービス) を作成します。</span><span class="sxs-lookup"><span data-stu-id="e1da6-131">Creating Folders (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

