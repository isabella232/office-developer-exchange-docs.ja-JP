---
title: 言語 (DiscoverySearchConfigurationType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 34eab81c-d832-4925-9f76-d69f24b36931
description: (DiscoverySearchConfigurationType) の言語要素は、カルチャに固有の形式の日付の範囲に使用するカルチャを識別します。 また、検索クエリで使用する言語を指定します。
ms.openlocfilehash: 1e904ac4d7f525b2d12cfe83f0da33b9ed474066
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832197"
---
# <a name="language-discoverysearchconfigurationtype"></a><span data-ttu-id="18108-104">言語 (DiscoverySearchConfigurationType)</span><span class="sxs-lookup"><span data-stu-id="18108-104">Language (DiscoverySearchConfigurationType)</span></span>

<span data-ttu-id="18108-105">**(DiscoverySearchConfigurationType) の言語**要素は、カルチャに固有の形式の日付の範囲に使用するカルチャを識別します。</span><span class="sxs-lookup"><span data-stu-id="18108-105">The **Language (DiscoverySearchConfigurationType)** element identifies the culture to be used for the culture-specific format of date ranges.</span></span> <span data-ttu-id="18108-106">また、検索クエリで使用する言語を指定します。</span><span class="sxs-lookup"><span data-stu-id="18108-106">It also specifies the language used in a search query.</span></span> 
  
```XML
<Language />
```

 <span data-ttu-id="18108-107">**string**</span><span class="sxs-lookup"><span data-stu-id="18108-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="18108-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="18108-108">Attributes and elements</span></span>

<span data-ttu-id="18108-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="18108-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="18108-110">属性</span><span class="sxs-lookup"><span data-stu-id="18108-110">Attributes</span></span>

<span data-ttu-id="18108-111">なし。</span><span class="sxs-lookup"><span data-stu-id="18108-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="18108-112">子要素</span><span class="sxs-lookup"><span data-stu-id="18108-112">Child elements</span></span>

<span data-ttu-id="18108-113">なし。</span><span class="sxs-lookup"><span data-stu-id="18108-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="18108-114">親要素</span><span class="sxs-lookup"><span data-stu-id="18108-114">Parent elements</span></span>

[<span data-ttu-id="18108-115">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="18108-115">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md)
  
## <a name="text-value"></a><span data-ttu-id="18108-116">テキスト値</span><span class="sxs-lookup"><span data-stu-id="18108-116">Text value</span></span>

<span data-ttu-id="18108-117">**言語 (DiscoverySearchConfigurationType)** の要素のテキスト値は、カルチャまたは言語です。</span><span class="sxs-lookup"><span data-stu-id="18108-117">The text value of the **Language (DiscoverySearchConfigurationType)** element is a culture or language.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="18108-118">備考</span><span class="sxs-lookup"><span data-stu-id="18108-118">Remarks</span></span>

<span data-ttu-id="18108-119">この要素は、 [SearchMailboxes 操作](searchmailboxes-operation.md)または[SetHoldOnMailboxes 操作](setholdonmailboxes-operation.md)で指定された日付範囲の書式を指定します。</span><span class="sxs-lookup"><span data-stu-id="18108-119">This element specifies the format of date ranges specified in the [SearchMailboxes operation](searchmailboxes-operation.md) or the [SetHoldOnMailboxes operation](setholdonmailboxes-operation.md).</span></span>
  
<span data-ttu-id="18108-120">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="18108-120">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="18108-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="18108-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="18108-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="18108-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="18108-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="18108-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="18108-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="18108-124">Schema Name</span></span>  <br/> |<span data-ttu-id="18108-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="18108-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="18108-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="18108-126">Validation File</span></span>  <br/> |<span data-ttu-id="18108-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="18108-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="18108-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="18108-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="18108-129">True</span><span class="sxs-lookup"><span data-stu-id="18108-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="18108-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="18108-130">See also</span></span>



[<span data-ttu-id="18108-131">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="18108-131">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md)


- [<span data-ttu-id="18108-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="18108-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

