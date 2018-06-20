---
title: TTL (ClientAccessTokenTypeType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cc8f8caa-fced-49b6-9861-d112590b218a
description: TTL 要素では、トークンの値に時刻を示します。
ms.openlocfilehash: 04bd8124c7bd2b02e2ab1cc47ee1d4dca4847079
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839755"
---
# <a name="ttl-clientaccesstokentypetype"></a><span data-ttu-id="6357c-103">TTL (ClientAccessTokenTypeType)</span><span class="sxs-lookup"><span data-stu-id="6357c-103">TTL (ClientAccessTokenTypeType)</span></span>

<span data-ttu-id="6357c-104">**TTL**要素では、トークンの値に時刻を示します。</span><span class="sxs-lookup"><span data-stu-id="6357c-104">The **TTL** element indicates the time to live value for the token.</span></span> 
  
```XML
<TTL></TTL>
```

 <span data-ttu-id="6357c-105">**整数**</span><span class="sxs-lookup"><span data-stu-id="6357c-105">**integer**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6357c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6357c-106">Attributes and elements</span></span>

<span data-ttu-id="6357c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6357c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6357c-108">属性</span><span class="sxs-lookup"><span data-stu-id="6357c-108">Attributes</span></span>

<span data-ttu-id="6357c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6357c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6357c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6357c-110">Child elements</span></span>

<span data-ttu-id="6357c-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6357c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6357c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6357c-112">Parent elements</span></span>

<span data-ttu-id="6357c-113">[TokenRequest](tokenrequest.md) | [トークン](token.md)</span><span class="sxs-lookup"><span data-stu-id="6357c-113">[TokenRequest](tokenrequest.md) | [Token](token.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="6357c-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6357c-114">Text value</span></span>

<span data-ttu-id="6357c-115">**TTL**要素のテキスト値は、トークンが有効である期間を示します。</span><span class="sxs-lookup"><span data-stu-id="6357c-115">The text value for the **TTL** element indicates how long the token remains valid.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="6357c-116">備考</span><span class="sxs-lookup"><span data-stu-id="6357c-116">Remarks</span></span>

<span data-ttu-id="6357c-117">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6357c-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6357c-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6357c-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6357c-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="6357c-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6357c-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="6357c-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6357c-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6357c-121">Schema name</span></span>  <br/> |<span data-ttu-id="6357c-122">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="6357c-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="6357c-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6357c-123">Validation file</span></span>  <br/> |<span data-ttu-id="6357c-124">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6357c-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6357c-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6357c-125">Can be empty</span></span>  <br/> |<span data-ttu-id="6357c-126">false</span><span class="sxs-lookup"><span data-stu-id="6357c-126">false</span></span>  <br/> |
   

