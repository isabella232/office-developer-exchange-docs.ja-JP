---
title: 絞り込み条件
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8395b45f-3b94-4473-82ac-2a12c4309170
description: 絞り込み条件要素では、検索の絞り込み条件を指定します。
ms.openlocfilehash: aad1874760e02b2226cbe1a5bb700013d3816cc0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833038"
---
# <a name="refiner"></a><span data-ttu-id="f57b6-103">絞り込み条件</span><span class="sxs-lookup"><span data-stu-id="f57b6-103">Refiner</span></span>

<span data-ttu-id="f57b6-104">**絞り込み条件**要素では、検索の絞り込み条件を指定します。</span><span class="sxs-lookup"><span data-stu-id="f57b6-104">The **Refiner** element specifies a search refiner.</span></span> 
  
```XML
<Refiner>
   <Name/>
   <Value/>
   <Count/>
   <Token/>
</Refiner>
```

 <span data-ttu-id="f57b6-105">**SearchRefinerItemType**</span><span class="sxs-lookup"><span data-stu-id="f57b6-105">**SearchRefinerItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f57b6-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f57b6-106">Attributes and elements</span></span>

<span data-ttu-id="f57b6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f57b6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f57b6-108">属性</span><span class="sxs-lookup"><span data-stu-id="f57b6-108">Attributes</span></span>

<span data-ttu-id="f57b6-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f57b6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f57b6-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f57b6-110">Child elements</span></span>

<span data-ttu-id="f57b6-111">[名 (文字列)](name-string.md) | [値](value.md) | [数](count.md) | [トークン (文字列)](token-string.md)</span><span class="sxs-lookup"><span data-stu-id="f57b6-111">[Name (string)](name-string.md) | [Value](value.md) | [Count](count.md) | [Token (String)](token-string.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f57b6-112">親要素</span><span class="sxs-lookup"><span data-stu-id="f57b6-112">Parent elements</span></span>

[<span data-ttu-id="f57b6-113">絞り込み条件</span><span class="sxs-lookup"><span data-stu-id="f57b6-113">Refiners</span></span>](refiners.md)
  
## <a name="remarks"></a><span data-ttu-id="f57b6-114">備考</span><span class="sxs-lookup"><span data-stu-id="f57b6-114">Remarks</span></span>

<span data-ttu-id="f57b6-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f57b6-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f57b6-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f57b6-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f57b6-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="f57b6-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f57b6-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="f57b6-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f57b6-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f57b6-119">Schema name</span></span>  <br/> |<span data-ttu-id="f57b6-120">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="f57b6-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="f57b6-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f57b6-121">Validation file</span></span>  <br/> |<span data-ttu-id="f57b6-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f57b6-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f57b6-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f57b6-123">Can be empty</span></span>  <br/> ||
   

