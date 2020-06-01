---
title: InPlaceHoldConfigurationOnly
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 921ecc73-b7e2-40a7-8458-68f18dd5a13b
description: InPlaceHoldConfigurationOnly 要素は、インプレースホールド構成を含めるかどうかを指定します。
ms.openlocfilehash: ca364ee7d8a9e2e4a608f8f6c4ca5851fa7d4b64
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466102"
---
# <a name="inplaceholdconfigurationonly"></a><span data-ttu-id="f5e65-103">InPlaceHoldConfigurationOnly</span><span class="sxs-lookup"><span data-stu-id="f5e65-103">InPlaceHoldConfigurationOnly</span></span>

<span data-ttu-id="f5e65-104">**InPlaceHoldConfigurationOnly**要素は、インプレースホールド構成を含めるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f5e65-104">The **InPlaceHoldConfigurationOnly** element specifies whether to include the in-place hold configuration.</span></span> 
  
```XML
<InPlaceHoldConfigurationOnly>true | false</InPlaceHoldConfigurationOnly>
```

 <span data-ttu-id="f5e65-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="f5e65-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f5e65-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f5e65-106">Attributes and elements</span></span>

<span data-ttu-id="f5e65-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f5e65-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f5e65-108">属性</span><span class="sxs-lookup"><span data-stu-id="f5e65-108">Attributes</span></span>

<span data-ttu-id="f5e65-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f5e65-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f5e65-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f5e65-110">Child elements</span></span>

<span data-ttu-id="f5e65-111">なし。</span><span class="sxs-lookup"><span data-stu-id="f5e65-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f5e65-112">親要素</span><span class="sxs-lookup"><span data-stu-id="f5e65-112">Parent elements</span></span>

[<span data-ttu-id="f5e65-113">GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="f5e65-113">GetDiscoverySearchConfiguration</span></span>](getdiscoverysearchconfiguration.md)
  
## <a name="text-value"></a><span data-ttu-id="f5e65-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f5e65-114">Text value</span></span>

<span data-ttu-id="f5e65-115">**InPlaceHoldConfigurationOnly**要素のテキスト値が**true**の場合は、インプレースホールド構成が含まれていることを示します。</span><span class="sxs-lookup"><span data-stu-id="f5e65-115">A text value of **true** for the **InPlaceHoldConfigurationOnly** element indicates that the in-place hold configuration is included.</span></span> <span data-ttu-id="f5e65-116">値が**false**の場合は、インプレースホールド構成が含まれていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="f5e65-116">A value of **false** indicates that the in-place hold configuration is not included.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f5e65-117">注釈</span><span class="sxs-lookup"><span data-stu-id="f5e65-117">Remarks</span></span>

<span data-ttu-id="f5e65-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f5e65-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f5e65-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f5e65-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f5e65-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f5e65-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f5e65-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="f5e65-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f5e65-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f5e65-122">Schema name</span></span>  <br/> |<span data-ttu-id="f5e65-123">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="f5e65-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f5e65-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f5e65-124">Validation file</span></span>  <br/> |<span data-ttu-id="f5e65-125">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="f5e65-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f5e65-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f5e65-126">Can be empty</span></span>  <br/> ||
   

