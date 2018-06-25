---
title: FolderSize
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderSize
api_type:
- schema
ms.assetid: 27e5f0cd-e23a-4ddd-943a-9f17bf0fd87b
description: FolderSize 要素では、管理対象フォルダーのすべての内容の合計サイズについて説明します。
ms.openlocfilehash: 314c75e6ab824caed4c6a1c6f5b62a43f86ba939
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760579"
---
# <a name="foldersize"></a><span data-ttu-id="3eb50-103">FolderSize</span><span class="sxs-lookup"><span data-stu-id="3eb50-103">FolderSize</span></span>

<span data-ttu-id="3eb50-104">**FolderSize**要素では、管理対象フォルダーのすべての内容の合計サイズについて説明します。</span><span class="sxs-lookup"><span data-stu-id="3eb50-104">The **FolderSize** element describes the total size of all the contents of a managed folder.</span></span> 
  
```xml
<FolderSize/>
```

 <span data-ttu-id="3eb50-105">**int**</span><span class="sxs-lookup"><span data-stu-id="3eb50-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3eb50-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="3eb50-106">Attributes and elements</span></span>

<span data-ttu-id="3eb50-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3eb50-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3eb50-108">属性</span><span class="sxs-lookup"><span data-stu-id="3eb50-108">Attributes</span></span>

<span data-ttu-id="3eb50-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3eb50-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3eb50-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3eb50-110">Child elements</span></span>

<span data-ttu-id="3eb50-111">なし。</span><span class="sxs-lookup"><span data-stu-id="3eb50-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3eb50-112">親要素</span><span class="sxs-lookup"><span data-stu-id="3eb50-112">Parent elements</span></span>

|<span data-ttu-id="3eb50-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="3eb50-113">**Element**</span></span>|<span data-ttu-id="3eb50-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="3eb50-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3eb50-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="3eb50-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="3eb50-116">管理フォルダーに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3eb50-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3eb50-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3eb50-117">Text value</span></span>

<span data-ttu-id="3eb50-118">テキスト値はメガバイト単位でのフォルダーの合計サイズを表します。</span><span class="sxs-lookup"><span data-stu-id="3eb50-118">The text value represents the total size of the folder in megabytes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3eb50-119">備考</span><span class="sxs-lookup"><span data-stu-id="3eb50-119">Remarks</span></span>

<span data-ttu-id="3eb50-120">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="3eb50-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3eb50-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="3eb50-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3eb50-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="3eb50-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3eb50-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3eb50-123">Schema name</span></span>  <br/> |<span data-ttu-id="3eb50-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="3eb50-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="3eb50-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3eb50-125">Validation file</span></span>  <br/> |<span data-ttu-id="3eb50-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3eb50-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3eb50-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="3eb50-127">Can be empty</span></span>  <br/> |<span data-ttu-id="3eb50-128">False</span><span class="sxs-lookup"><span data-stu-id="3eb50-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3eb50-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="3eb50-129">See also</span></span>



[<span data-ttu-id="3eb50-130">CreateManagedFolder 操作</span><span class="sxs-lookup"><span data-stu-id="3eb50-130">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)


- [<span data-ttu-id="3eb50-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="3eb50-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

