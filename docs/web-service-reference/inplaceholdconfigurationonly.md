---
title: InPlaceHoldConfigurationOnly
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 921ecc73-b7e2-40a7-8458-68f18dd5a13b
description: InPlaceHoldConfigurationOnly 要素を含めるかどうかと、インプレース保持構成を指定します。
ms.openlocfilehash: 3ad020a10e43d8f54e3d603906c856e01b1956eb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831934"
---
# <a name="inplaceholdconfigurationonly"></a><span data-ttu-id="7e8b9-103">InPlaceHoldConfigurationOnly</span><span class="sxs-lookup"><span data-stu-id="7e8b9-103">InPlaceHoldConfigurationOnly</span></span>

<span data-ttu-id="7e8b9-104">**InPlaceHoldConfigurationOnly**要素を含めるかどうかと、インプレース保持構成を指定します。</span><span class="sxs-lookup"><span data-stu-id="7e8b9-104">The **InPlaceHoldConfigurationOnly** element specifies whether to include the in-place hold configuration.</span></span> 
  
```XML
<InPlaceHoldConfigurationOnly>true | false</InPlaceHoldConfigurationOnly>
```

 <span data-ttu-id="7e8b9-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="7e8b9-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7e8b9-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7e8b9-106">Attributes and elements</span></span>

<span data-ttu-id="7e8b9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7e8b9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7e8b9-108">属性</span><span class="sxs-lookup"><span data-stu-id="7e8b9-108">Attributes</span></span>

<span data-ttu-id="7e8b9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7e8b9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7e8b9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7e8b9-110">Child elements</span></span>

<span data-ttu-id="7e8b9-111">なし。</span><span class="sxs-lookup"><span data-stu-id="7e8b9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7e8b9-112">親要素</span><span class="sxs-lookup"><span data-stu-id="7e8b9-112">Parent elements</span></span>

[<span data-ttu-id="7e8b9-113">GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="7e8b9-113">GetDiscoverySearchConfiguration</span></span>](getdiscoverysearchconfiguration.md)
  
## <a name="text-value"></a><span data-ttu-id="7e8b9-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7e8b9-114">Text value</span></span>

<span data-ttu-id="7e8b9-115">の**場合は true** 、 **InPlaceHoldConfigurationOnly**要素のテキスト値は、埋め込み先の保留中の構成が含まれていることを示します。</span><span class="sxs-lookup"><span data-stu-id="7e8b9-115">A text value of **true** for the **InPlaceHoldConfigurationOnly** element indicates that the in-place hold configuration is included.</span></span> <span data-ttu-id="7e8b9-116">**False**の値は、埋め込み先の保留中の構成が含まれていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="7e8b9-116">A value of **false** indicates that the in-place hold configuration is not included.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="7e8b9-117">備考</span><span class="sxs-lookup"><span data-stu-id="7e8b9-117">Remarks</span></span>

<span data-ttu-id="7e8b9-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="7e8b9-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7e8b9-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7e8b9-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7e8b9-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="7e8b9-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7e8b9-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="7e8b9-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7e8b9-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7e8b9-122">Schema name</span></span>  <br/> |<span data-ttu-id="7e8b9-123">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="7e8b9-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7e8b9-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7e8b9-124">Validation file</span></span>  <br/> |<span data-ttu-id="7e8b9-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7e8b9-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7e8b9-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="7e8b9-126">Can be empty</span></span>  <br/> ||
   

