---
title: StorageQuota
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StorageQuota
api_type:
- schema
ms.assetid: a0ba42c9-321a-4370-b979-e02078bcb070
description: StorageQuota 要素では、管理フォルダーの記憶域のクォータについて説明します。
ms.openlocfilehash: e0bdc98d9fe59a89cc78fe387624fa556a4da556
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833595"
---
# <a name="storagequota"></a><span data-ttu-id="2f860-103">StorageQuota</span><span class="sxs-lookup"><span data-stu-id="2f860-103">StorageQuota</span></span>

<span data-ttu-id="2f860-104">**StorageQuota**要素では、管理フォルダーの記憶域のクォータについて説明します。</span><span class="sxs-lookup"><span data-stu-id="2f860-104">The **StorageQuota** element describes the storage quota for the managed folder.</span></span> 
  
```xml
<StorageQuota/>
```

 <span data-ttu-id="2f860-105">**int**</span><span class="sxs-lookup"><span data-stu-id="2f860-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2f860-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2f860-106">Attributes and elements</span></span>

<span data-ttu-id="2f860-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2f860-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2f860-108">属性</span><span class="sxs-lookup"><span data-stu-id="2f860-108">Attributes</span></span>

<span data-ttu-id="2f860-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2f860-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2f860-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2f860-110">Child elements</span></span>

<span data-ttu-id="2f860-111">なし。</span><span class="sxs-lookup"><span data-stu-id="2f860-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2f860-112">親要素</span><span class="sxs-lookup"><span data-stu-id="2f860-112">Parent elements</span></span>

|<span data-ttu-id="2f860-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="2f860-113">**Element**</span></span>|<span data-ttu-id="2f860-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="2f860-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2f860-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="2f860-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="2f860-116">管理フォルダーに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2f860-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2f860-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="2f860-117">Text value</span></span>

<span data-ttu-id="2f860-118">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="2f860-118">A text value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2f860-119">備考</span><span class="sxs-lookup"><span data-stu-id="2f860-119">Remarks</span></span>

<span data-ttu-id="2f860-120">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="2f860-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2f860-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="2f860-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2f860-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="2f860-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2f860-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2f860-123">Schema name</span></span>  <br/> |<span data-ttu-id="2f860-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="2f860-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="2f860-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2f860-125">Validation file</span></span>  <br/> |<span data-ttu-id="2f860-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2f860-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2f860-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2f860-127">Can be empty</span></span>  <br/> |<span data-ttu-id="2f860-128">False</span><span class="sxs-lookup"><span data-stu-id="2f860-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2f860-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="2f860-129">See also</span></span>



- [<span data-ttu-id="2f860-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="2f860-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="2f860-131">管理フォルダーを追加します。</span><span class="sxs-lookup"><span data-stu-id="2f860-131">Adding Managed Folders</span></span>](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

