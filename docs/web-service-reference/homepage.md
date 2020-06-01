---
title: HomePage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- HomePage
api_type:
- schema
ms.assetid: eec2c41e-a975-42f6-8150-caf8c6e26462
description: ホームページ要素は、管理フォルダーの既定のホームページとなる URL を指定します。
ms.openlocfilehash: b56a273bab3ec34d03e84ba8f7e2d6feddeb3e88
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460842"
---
# <a name="homepage"></a><span data-ttu-id="0e655-103">HomePage</span><span class="sxs-lookup"><span data-stu-id="0e655-103">HomePage</span></span>

<span data-ttu-id="0e655-104">**ホーム**ページ要素は、管理フォルダーの既定のホームページとなる URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="0e655-104">The **HomePage** element specifies the URL that will be the default home page for the managed folder.</span></span> 
  
```xml
<HomePage/>
```

 <span data-ttu-id="0e655-105">**String**</span><span class="sxs-lookup"><span data-stu-id="0e655-105">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0e655-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0e655-106">Attributes and elements</span></span>

<span data-ttu-id="0e655-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0e655-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0e655-108">属性</span><span class="sxs-lookup"><span data-stu-id="0e655-108">Attributes</span></span>

<span data-ttu-id="0e655-109">なし。</span><span class="sxs-lookup"><span data-stu-id="0e655-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0e655-110">子要素</span><span class="sxs-lookup"><span data-stu-id="0e655-110">Child elements</span></span>

<span data-ttu-id="0e655-111">なし。</span><span class="sxs-lookup"><span data-stu-id="0e655-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0e655-112">親要素</span><span class="sxs-lookup"><span data-stu-id="0e655-112">Parent elements</span></span>

|<span data-ttu-id="0e655-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="0e655-113">**Element**</span></span>|<span data-ttu-id="0e655-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="0e655-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0e655-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="0e655-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="0e655-116">管理フォルダーに関する情報を格納します。</span><span class="sxs-lookup"><span data-stu-id="0e655-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0e655-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="0e655-117">Text value</span></span>

<span data-ttu-id="0e655-118">テキスト値は、URL を表す文字列型 (string) の値です。</span><span class="sxs-lookup"><span data-stu-id="0e655-118">The text value is a string value that represents a URL.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0e655-119">注釈</span><span class="sxs-lookup"><span data-stu-id="0e655-119">Remarks</span></span>

<span data-ttu-id="0e655-120">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="0e655-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0e655-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0e655-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0e655-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="0e655-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0e655-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0e655-123">Schema name</span></span>  <br/> |<span data-ttu-id="0e655-124">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="0e655-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="0e655-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0e655-125">Validation file</span></span>  <br/> |<span data-ttu-id="0e655-126">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="0e655-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0e655-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="0e655-127">Can be empty</span></span>  <br/> |<span data-ttu-id="0e655-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="0e655-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0e655-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="0e655-129">See also</span></span>



[<span data-ttu-id="0e655-130">CreateManagedFolder 操作</span><span class="sxs-lookup"><span data-stu-id="0e655-130">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)


- [<span data-ttu-id="0e655-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="0e655-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="0e655-132">管理フォルダーの追加</span><span class="sxs-lookup"><span data-stu-id="0e655-132">Adding Managed Folders</span></span>](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

