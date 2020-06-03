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
description: CreateFolder 要素は、Exchange ストア内にフォルダーを作成するための要求を定義します。
ms.openlocfilehash: c2a971a6b827553a1632c2a86e4d36e3b83a2de3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457544"
---
# <a name="createfolder"></a><span data-ttu-id="9628e-103">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="9628e-103">CreateFolder</span></span>

<span data-ttu-id="9628e-104">**CreateFolder**要素は、Exchange ストア内にフォルダーを作成するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="9628e-104">The **CreateFolder** element defines a request to create a folder in the Exchange store.</span></span> 
  
```xml
<CreateFolder>
   <ParentFolderId/>
   <Folders/>
</CreateFolder>
```

 <span data-ttu-id="9628e-105">**CreateFolderType**</span><span class="sxs-lookup"><span data-stu-id="9628e-105">**CreateFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9628e-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9628e-106">Attributes and elements</span></span>

<span data-ttu-id="9628e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9628e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9628e-108">属性</span><span class="sxs-lookup"><span data-stu-id="9628e-108">Attributes</span></span>

<span data-ttu-id="9628e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9628e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9628e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9628e-110">Child elements</span></span>

|<span data-ttu-id="9628e-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="9628e-111">**Element**</span></span>|<span data-ttu-id="9628e-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="9628e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9628e-113">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="9628e-113">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md) <br/> |<span data-ttu-id="9628e-114">新しいフォルダーが作成される場所を識別する要素。</span><span class="sxs-lookup"><span data-stu-id="9628e-114">The element that identifies the location where the new folder is created.</span></span>  <br/> |
|[<span data-ttu-id="9628e-115">フォルダー</span><span class="sxs-lookup"><span data-stu-id="9628e-115">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="9628e-116">作成するすべてのフォルダーを含む要素。</span><span class="sxs-lookup"><span data-stu-id="9628e-116">The element that contains all the folders to create.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9628e-117">親要素</span><span class="sxs-lookup"><span data-stu-id="9628e-117">Parent elements</span></span>

<span data-ttu-id="9628e-118">なし。</span><span class="sxs-lookup"><span data-stu-id="9628e-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9628e-119">注釈</span><span class="sxs-lookup"><span data-stu-id="9628e-119">Remarks</span></span>

<span data-ttu-id="9628e-120">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="9628e-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9628e-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9628e-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9628e-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="9628e-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9628e-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9628e-123">Schema Name</span></span>  <br/> |<span data-ttu-id="9628e-124">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="9628e-124">Message schema</span></span>  <br/> |
|<span data-ttu-id="9628e-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9628e-125">Validation File</span></span>  <br/> |<span data-ttu-id="9628e-126">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="9628e-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9628e-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9628e-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="9628e-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="9628e-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9628e-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="9628e-129">See also</span></span>



[<span data-ttu-id="9628e-130">CreateFolder 操作</span><span class="sxs-lookup"><span data-stu-id="9628e-130">CreateFolder operation</span></span>](createfolder-operation.md)


[<span data-ttu-id="9628e-131">フォルダーの作成 (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="9628e-131">Creating Folders (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

