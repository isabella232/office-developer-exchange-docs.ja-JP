---
title: GetFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetFolder
api_type:
- schema
ms.assetid: 34e4c9ea-adcd-46bd-ae8f-7abb256c585a
description: GetFolder の要素は、Exchange ストア内のメールボックスからフォルダーを取得する要求を定義します。
ms.openlocfilehash: 233da6ce57683350d4a13f6585593ac09438f0e6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760739"
---
# <a name="getfolder"></a><span data-ttu-id="1f15b-103">GetFolder</span><span class="sxs-lookup"><span data-stu-id="1f15b-103">GetFolder</span></span>

<span data-ttu-id="1f15b-104">**GetFolder**の要素は、Exchange ストア内のメールボックスからフォルダーを取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="1f15b-104">The **GetFolder** element defines a request to get a folder from a mailbox in the Exchange store.</span></span> 
  
```xml
<GetFolder>
   <FolderShape/>
   <FolderIds/>
</GetFolder>
```

 <span data-ttu-id="1f15b-105">**GetFolderType**</span><span class="sxs-lookup"><span data-stu-id="1f15b-105">**GetFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1f15b-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="1f15b-106">Attributes and elements</span></span>

<span data-ttu-id="1f15b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1f15b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1f15b-108">属性</span><span class="sxs-lookup"><span data-stu-id="1f15b-108">Attributes</span></span>

<span data-ttu-id="1f15b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1f15b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1f15b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1f15b-110">Child elements</span></span>

|<span data-ttu-id="1f15b-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="1f15b-111">**Element**</span></span>|<span data-ttu-id="1f15b-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="1f15b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1f15b-113">FolderShape</span><span class="sxs-lookup"><span data-stu-id="1f15b-113">FolderShape</span></span>](foldershape.md) <br/> |<span data-ttu-id="1f15b-114">[FolderIds](folderids.md)要素で識別される各フォルダーを取得するプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="1f15b-114">Identifies the properties to get for each folder identified in the [FolderIds](folderids.md) element.</span></span>  <br/> |
|[<span data-ttu-id="1f15b-115">FolderIds</span><span class="sxs-lookup"><span data-stu-id="1f15b-115">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="1f15b-116">Exchange ストア内のメールボックスから取得するフォルダーを識別するために使用されるフォルダー識別子の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1f15b-116">Contains an array of folder identifiers that are used to identify folders to get from a mailbox in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1f15b-117">親要素</span><span class="sxs-lookup"><span data-stu-id="1f15b-117">Parent elements</span></span>

<span data-ttu-id="1f15b-118">なし。</span><span class="sxs-lookup"><span data-stu-id="1f15b-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1f15b-119">備考</span><span class="sxs-lookup"><span data-stu-id="1f15b-119">Remarks</span></span>

<span data-ttu-id="1f15b-120">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="1f15b-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1f15b-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="1f15b-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1f15b-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="1f15b-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1f15b-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1f15b-123">Schema Name</span></span>  <br/> |<span data-ttu-id="1f15b-124">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="1f15b-124">Message schema</span></span>  <br/> |
|<span data-ttu-id="1f15b-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1f15b-125">Validation File</span></span>  <br/> |<span data-ttu-id="1f15b-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1f15b-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1f15b-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1f15b-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="1f15b-128">False</span><span class="sxs-lookup"><span data-stu-id="1f15b-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1f15b-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="1f15b-129">See also</span></span>



<span data-ttu-id="1f15b-130">
  [GetFolder 操作](getfolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="1f15b-130">[GetFolder operation](getfolder-operation.md)</span></span>

