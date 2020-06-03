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
description: FolderSize 要素は、管理フォルダーのすべてのコンテンツの合計サイズを示します。
ms.openlocfilehash: 8ed493cfb0c2cabd02d28354c115a73662992473
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461339"
---
# <a name="foldersize"></a><span data-ttu-id="3baef-103">FolderSize</span><span class="sxs-lookup"><span data-stu-id="3baef-103">FolderSize</span></span>

<span data-ttu-id="3baef-104">**Foldersize**要素は、管理フォルダーのすべてのコンテンツの合計サイズを示します。</span><span class="sxs-lookup"><span data-stu-id="3baef-104">The **FolderSize** element describes the total size of all the contents of a managed folder.</span></span> 
  
```xml
<FolderSize/>
```

 <span data-ttu-id="3baef-105">**int**</span><span class="sxs-lookup"><span data-stu-id="3baef-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3baef-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="3baef-106">Attributes and elements</span></span>

<span data-ttu-id="3baef-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3baef-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3baef-108">属性</span><span class="sxs-lookup"><span data-stu-id="3baef-108">Attributes</span></span>

<span data-ttu-id="3baef-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3baef-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3baef-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3baef-110">Child elements</span></span>

<span data-ttu-id="3baef-111">なし。</span><span class="sxs-lookup"><span data-stu-id="3baef-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3baef-112">親要素</span><span class="sxs-lookup"><span data-stu-id="3baef-112">Parent elements</span></span>

|<span data-ttu-id="3baef-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="3baef-113">**Element**</span></span>|<span data-ttu-id="3baef-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="3baef-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3baef-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="3baef-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="3baef-116">管理フォルダーに関する情報を格納します。</span><span class="sxs-lookup"><span data-stu-id="3baef-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3baef-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3baef-117">Text value</span></span>

<span data-ttu-id="3baef-118">Text 値は、フォルダーの合計サイズをメガバイト単位で表します。</span><span class="sxs-lookup"><span data-stu-id="3baef-118">The text value represents the total size of the folder in megabytes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3baef-119">注釈</span><span class="sxs-lookup"><span data-stu-id="3baef-119">Remarks</span></span>

<span data-ttu-id="3baef-120">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="3baef-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3baef-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="3baef-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3baef-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="3baef-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3baef-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3baef-123">Schema name</span></span>  <br/> |<span data-ttu-id="3baef-124">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="3baef-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="3baef-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3baef-125">Validation file</span></span>  <br/> |<span data-ttu-id="3baef-126">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="3baef-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3baef-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="3baef-127">Can be empty</span></span>  <br/> |<span data-ttu-id="3baef-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="3baef-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3baef-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="3baef-129">See also</span></span>



[<span data-ttu-id="3baef-130">CreateManagedFolder 操作</span><span class="sxs-lookup"><span data-stu-id="3baef-130">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)


- [<span data-ttu-id="3baef-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="3baef-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

