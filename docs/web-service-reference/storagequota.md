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
description: StorageQuota 要素は、管理フォルダーの記憶域のクォータを示します。
ms.openlocfilehash: c979b02c2c4df511eae96125847ed765ba3ed92c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468237"
---
# <a name="storagequota"></a><span data-ttu-id="09892-103">StorageQuota</span><span class="sxs-lookup"><span data-stu-id="09892-103">StorageQuota</span></span>

<span data-ttu-id="09892-104">**StorageQuota**要素は、管理フォルダーの記憶域のクォータを示します。</span><span class="sxs-lookup"><span data-stu-id="09892-104">The **StorageQuota** element describes the storage quota for the managed folder.</span></span> 
  
```xml
<StorageQuota/>
```

 <span data-ttu-id="09892-105">**int**</span><span class="sxs-lookup"><span data-stu-id="09892-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="09892-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="09892-106">Attributes and elements</span></span>

<span data-ttu-id="09892-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="09892-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="09892-108">属性</span><span class="sxs-lookup"><span data-stu-id="09892-108">Attributes</span></span>

<span data-ttu-id="09892-109">なし。</span><span class="sxs-lookup"><span data-stu-id="09892-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="09892-110">子要素</span><span class="sxs-lookup"><span data-stu-id="09892-110">Child elements</span></span>

<span data-ttu-id="09892-111">なし。</span><span class="sxs-lookup"><span data-stu-id="09892-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="09892-112">親要素</span><span class="sxs-lookup"><span data-stu-id="09892-112">Parent elements</span></span>

|<span data-ttu-id="09892-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="09892-113">**Element**</span></span>|<span data-ttu-id="09892-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="09892-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="09892-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="09892-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="09892-116">管理フォルダーに関する情報を格納します。</span><span class="sxs-lookup"><span data-stu-id="09892-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="09892-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="09892-117">Text value</span></span>

<span data-ttu-id="09892-118">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="09892-118">A text value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="09892-119">注釈</span><span class="sxs-lookup"><span data-stu-id="09892-119">Remarks</span></span>

<span data-ttu-id="09892-120">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="09892-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="09892-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="09892-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="09892-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="09892-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="09892-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="09892-123">Schema name</span></span>  <br/> |<span data-ttu-id="09892-124">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="09892-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="09892-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="09892-125">Validation file</span></span>  <br/> |<span data-ttu-id="09892-126">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="09892-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="09892-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="09892-127">Can be empty</span></span>  <br/> |<span data-ttu-id="09892-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="09892-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="09892-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="09892-129">See also</span></span>



- [<span data-ttu-id="09892-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="09892-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="09892-131">管理フォルダーの追加</span><span class="sxs-lookup"><span data-stu-id="09892-131">Adding Managed Folders</span></span>](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

