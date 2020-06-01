---
title: サポートされている apiversion
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d9264e74-eba7-4279-b193-af7e5130268d
description: ApiVersionSupported 要素には、クライアントでサポートされている JavaScript API for Office のバージョンが含まれています。
ms.openlocfilehash: 0129a33624b48d309ad0814af6eaa655b2c4e6f9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/01/2020
ms.locfileid: "44466060"
---
# <a name="apiversionsupported"></a><span data-ttu-id="03ebc-103">サポートされている apiversion</span><span class="sxs-lookup"><span data-stu-id="03ebc-103">ApiVersionSupported</span></span>

<span data-ttu-id="03ebc-104">**Apiversionsupported**要素には、クライアントでサポートされている JavaScript API for Office のバージョンが含まれています。</span><span class="sxs-lookup"><span data-stu-id="03ebc-104">The **ApiVersionSupported** element contains the version of the JavaScript API for Office supported by the client.</span></span> 
  
```XML
<ApiVersionSupported />
```

 <span data-ttu-id="03ebc-105">**string**</span><span class="sxs-lookup"><span data-stu-id="03ebc-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="03ebc-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="03ebc-106">Attributes and elements</span></span>

<span data-ttu-id="03ebc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="03ebc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="03ebc-108">属性</span><span class="sxs-lookup"><span data-stu-id="03ebc-108">Attributes</span></span>

<span data-ttu-id="03ebc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="03ebc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="03ebc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="03ebc-110">Child elements</span></span>

<span data-ttu-id="03ebc-111">なし。</span><span class="sxs-lookup"><span data-stu-id="03ebc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="03ebc-112">親要素</span><span class="sxs-lookup"><span data-stu-id="03ebc-112">Parent elements</span></span>

[<span data-ttu-id="03ebc-113">Getappmanifests が</span><span class="sxs-lookup"><span data-stu-id="03ebc-113">GetAppManifests</span></span>](getappmanifests.md)
  
## <a name="text-value"></a><span data-ttu-id="03ebc-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="03ebc-114">Text value</span></span>

<span data-ttu-id="03ebc-115">**Apiversionsupported**要素のテキスト値には、クライアントでサポートされている JavaScript API for Office のバージョンが含まれています。</span><span class="sxs-lookup"><span data-stu-id="03ebc-115">The text value of the **ApiVersionSupported** element contains the version of the JavaScript API for Office supported by the client.</span></span> <span data-ttu-id="03ebc-116">この値は、応答でクライアントに返されるアプリケーションマニフェストを示します。</span><span class="sxs-lookup"><span data-stu-id="03ebc-116">This value indicates which app manifests should be returned to the client in the response.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="03ebc-117">注釈</span><span class="sxs-lookup"><span data-stu-id="03ebc-117">Remarks</span></span>

<span data-ttu-id="03ebc-118">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="03ebc-118">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="03ebc-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="03ebc-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="03ebc-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="03ebc-120">Namespace</span></span>  <br/> | https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="03ebc-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="03ebc-121">Schema Name</span></span>  <br/> |<span data-ttu-id="03ebc-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="03ebc-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="03ebc-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="03ebc-123">Validation File</span></span>  <br/> |<span data-ttu-id="03ebc-124">該当なし</span><span class="sxs-lookup"><span data-stu-id="03ebc-124">Not applicable</span></span>  <br/> |
|<span data-ttu-id="03ebc-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="03ebc-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="03ebc-126">正しくない</span><span class="sxs-lookup"><span data-stu-id="03ebc-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="03ebc-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="03ebc-127">See also</span></span>

- [<span data-ttu-id="03ebc-128">Getappmanifests が</span><span class="sxs-lookup"><span data-stu-id="03ebc-128">GetAppManifests</span></span>](getappmanifests.md)
- [<span data-ttu-id="03ebc-129">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="03ebc-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

