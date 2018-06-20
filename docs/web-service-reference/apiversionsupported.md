---
title: ApiVersionSupported
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d9264e74-eba7-4279-b193-af7e5130268d
description: ApiVersionSupported 要素には、JavaScript API のクライアントでサポートされている Office のバージョンが含まれています。
ms.openlocfilehash: 41c3eacff65d797dfe7e8b587c50c35d8938664f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759326"
---
# <a name="apiversionsupported"></a><span data-ttu-id="504d8-103">ApiVersionSupported</span><span class="sxs-lookup"><span data-stu-id="504d8-103">ApiVersionSupported</span></span>

<span data-ttu-id="504d8-104">**ApiVersionSupported**要素には、JavaScript API のクライアントでサポートされている Office のバージョンが含まれています。</span><span class="sxs-lookup"><span data-stu-id="504d8-104">The **ApiVersionSupported** element contains the version of the JavaScript API for Office supported by the client.</span></span> 
  
```XML
<ApiVersionSupported />
```

 <span data-ttu-id="504d8-105">**string**</span><span class="sxs-lookup"><span data-stu-id="504d8-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="504d8-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="504d8-106">Attributes and elements</span></span>

<span data-ttu-id="504d8-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="504d8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="504d8-108">属性</span><span class="sxs-lookup"><span data-stu-id="504d8-108">Attributes</span></span>

<span data-ttu-id="504d8-109">なし。</span><span class="sxs-lookup"><span data-stu-id="504d8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="504d8-110">子要素</span><span class="sxs-lookup"><span data-stu-id="504d8-110">Child elements</span></span>

<span data-ttu-id="504d8-111">なし。</span><span class="sxs-lookup"><span data-stu-id="504d8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="504d8-112">親要素</span><span class="sxs-lookup"><span data-stu-id="504d8-112">Parent elements</span></span>

[<span data-ttu-id="504d8-113">GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="504d8-113">GetAppManifests</span></span>](getappmanifests.md)
  
## <a name="text-value"></a><span data-ttu-id="504d8-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="504d8-114">Text value</span></span>

<span data-ttu-id="504d8-115">**ApiVersionSupported**要素のテキスト値には、JavaScript API のクライアントでサポートされている Office のバージョンが含まれています。</span><span class="sxs-lookup"><span data-stu-id="504d8-115">The text value of the **ApiVersionSupported** element contains the version of the JavaScript API for Office supported by the client.</span></span> <span data-ttu-id="504d8-116">この値は、アプリケーション マニフェストは、応答でクライアントに返される必要がありますを示します。</span><span class="sxs-lookup"><span data-stu-id="504d8-116">This value indicates which app manifests should be returned to the client in the response.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="504d8-117">備考</span><span class="sxs-lookup"><span data-stu-id="504d8-117">Remarks</span></span>

<span data-ttu-id="504d8-118">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="504d8-118">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="504d8-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="504d8-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="504d8-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="504d8-120">Namespace</span></span>  <br/> | http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="504d8-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="504d8-121">Schema Name</span></span>  <br/> |<span data-ttu-id="504d8-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="504d8-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="504d8-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="504d8-123">Validation File</span></span>  <br/> |<span data-ttu-id="504d8-124">該当しない</span><span class="sxs-lookup"><span data-stu-id="504d8-124">Not applicable</span></span>  <br/> |
|<span data-ttu-id="504d8-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="504d8-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="504d8-126">False</span><span class="sxs-lookup"><span data-stu-id="504d8-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="504d8-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="504d8-127">See also</span></span>

- [<span data-ttu-id="504d8-128">GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="504d8-128">GetAppManifests</span></span>](getappmanifests.md)
- [<span data-ttu-id="504d8-129">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="504d8-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

