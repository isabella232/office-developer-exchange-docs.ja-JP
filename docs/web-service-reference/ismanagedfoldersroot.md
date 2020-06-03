---
title: Ismanagedフォルダーのルート
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsManagedFoldersRoot
api_type:
- schema
ms.assetid: 00823fb9-bf8b-49bb-8e1b-d698c6d4063f
description: Ismanagedfolders ルート要素は、管理フォルダーがすべての管理フォルダーのルートであるかどうかを示します。
ms.openlocfilehash: 4373dba9dce92de8e175948d889f0806e100fa6c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466025"
---
# <a name="ismanagedfoldersroot"></a><span data-ttu-id="cbe65-103">Ismanagedフォルダーのルート</span><span class="sxs-lookup"><span data-stu-id="cbe65-103">IsManagedFoldersRoot</span></span>

<span data-ttu-id="cbe65-104">**Ismanagedfolders ルート**要素は、管理フォルダーがすべての管理フォルダーのルートであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cbe65-104">The **IsManagedFoldersRoot** element indicates whether the managed folder is the root for all managed folders.</span></span> 
  
```xml
<IsManagedFoldersRoot/>
```

 <span data-ttu-id="cbe65-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="cbe65-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cbe65-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="cbe65-106">Attributes and elements</span></span>

<span data-ttu-id="cbe65-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cbe65-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cbe65-108">属性</span><span class="sxs-lookup"><span data-stu-id="cbe65-108">Attributes</span></span>

<span data-ttu-id="cbe65-109">なし。</span><span class="sxs-lookup"><span data-stu-id="cbe65-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cbe65-110">子要素</span><span class="sxs-lookup"><span data-stu-id="cbe65-110">Child elements</span></span>

<span data-ttu-id="cbe65-111">なし。</span><span class="sxs-lookup"><span data-stu-id="cbe65-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cbe65-112">親要素</span><span class="sxs-lookup"><span data-stu-id="cbe65-112">Parent elements</span></span>

|<span data-ttu-id="cbe65-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="cbe65-113">**Element**</span></span>|<span data-ttu-id="cbe65-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="cbe65-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cbe65-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="cbe65-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="cbe65-116">管理フォルダーに関する情報を格納します。</span><span class="sxs-lookup"><span data-stu-id="cbe65-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cbe65-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="cbe65-117">Text value</span></span>

<span data-ttu-id="cbe65-118">この要素が存在する場合は、ブール値を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="cbe65-118">A text value that represents a Boolean value is required if this element is present.</span></span> <span data-ttu-id="cbe65-119">値が**true の場合**は、フォルダーが管理フォルダーのルートフォルダーであることを示します。値が**false**の場合は、フォルダーが管理フォルダーのルートフォルダーではないことを示します。</span><span class="sxs-lookup"><span data-stu-id="cbe65-119">A value of **true** indicates that the folder is the root folder of the managed folder; a value of **false** indicates that the folder is not the root folder of the managed folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="cbe65-120">注釈</span><span class="sxs-lookup"><span data-stu-id="cbe65-120">Remarks</span></span>

<span data-ttu-id="cbe65-121">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="cbe65-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cbe65-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="cbe65-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cbe65-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="cbe65-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cbe65-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="cbe65-124">Schema name</span></span>  <br/> |<span data-ttu-id="cbe65-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="cbe65-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="cbe65-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="cbe65-126">Validation file</span></span>  <br/> |<span data-ttu-id="cbe65-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="cbe65-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cbe65-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="cbe65-128">Can be empty</span></span>  <br/> |<span data-ttu-id="cbe65-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="cbe65-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cbe65-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="cbe65-130">See also</span></span>



- [<span data-ttu-id="cbe65-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="cbe65-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

