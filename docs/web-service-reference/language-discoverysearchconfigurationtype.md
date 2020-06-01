---
title: 言語 (DiscoverySearchConfigurationType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 34eab81c-d832-4925-9f76-d69f24b36931
description: Language (DiscoverySearchConfigurationType) 要素は、カルチャ固有の日付範囲の形式に使用されるカルチャを指定します。 検索クエリで使用される言語も指定します。
ms.openlocfilehash: 3cf85525147bec5d6dfc6fe2b2af5916d42c44be
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463287"
---
# <a name="language-discoverysearchconfigurationtype"></a><span data-ttu-id="27d37-104">言語 (DiscoverySearchConfigurationType)</span><span class="sxs-lookup"><span data-stu-id="27d37-104">Language (DiscoverySearchConfigurationType)</span></span>

<span data-ttu-id="27d37-105">**Language (DiscoverySearchConfigurationType)** 要素は、カルチャ固有の日付範囲の形式に使用されるカルチャを指定します。</span><span class="sxs-lookup"><span data-stu-id="27d37-105">The **Language (DiscoverySearchConfigurationType)** element identifies the culture to be used for the culture-specific format of date ranges.</span></span> <span data-ttu-id="27d37-106">検索クエリで使用される言語も指定します。</span><span class="sxs-lookup"><span data-stu-id="27d37-106">It also specifies the language used in a search query.</span></span> 
  
```XML
<Language />
```

 <span data-ttu-id="27d37-107">**string**</span><span class="sxs-lookup"><span data-stu-id="27d37-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="27d37-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="27d37-108">Attributes and elements</span></span>

<span data-ttu-id="27d37-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="27d37-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="27d37-110">属性</span><span class="sxs-lookup"><span data-stu-id="27d37-110">Attributes</span></span>

<span data-ttu-id="27d37-111">なし。</span><span class="sxs-lookup"><span data-stu-id="27d37-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="27d37-112">子要素</span><span class="sxs-lookup"><span data-stu-id="27d37-112">Child elements</span></span>

<span data-ttu-id="27d37-113">なし。</span><span class="sxs-lookup"><span data-stu-id="27d37-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="27d37-114">親要素</span><span class="sxs-lookup"><span data-stu-id="27d37-114">Parent elements</span></span>

[<span data-ttu-id="27d37-115">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="27d37-115">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md)
  
## <a name="text-value"></a><span data-ttu-id="27d37-116">テキスト値</span><span class="sxs-lookup"><span data-stu-id="27d37-116">Text value</span></span>

<span data-ttu-id="27d37-117">**Language (DiscoverySearchConfigurationType)** 要素のテキスト値は、カルチャまたは言語です。</span><span class="sxs-lookup"><span data-stu-id="27d37-117">The text value of the **Language (DiscoverySearchConfigurationType)** element is a culture or language.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="27d37-118">注釈</span><span class="sxs-lookup"><span data-stu-id="27d37-118">Remarks</span></span>

<span data-ttu-id="27d37-119">この要素は、 [Searchmailboxes ボックス操作](searchmailboxes-operation.md)または[SetHoldOnMailboxes 操作](setholdonmailboxes-operation.md)で指定された日付範囲の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="27d37-119">This element specifies the format of date ranges specified in the [SearchMailboxes operation](searchmailboxes-operation.md) or the [SetHoldOnMailboxes operation](setholdonmailboxes-operation.md).</span></span>
  
<span data-ttu-id="27d37-120">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="27d37-120">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="27d37-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="27d37-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="27d37-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="27d37-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="27d37-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="27d37-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="27d37-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="27d37-124">Schema Name</span></span>  <br/> |<span data-ttu-id="27d37-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="27d37-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="27d37-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="27d37-126">Validation File</span></span>  <br/> |<span data-ttu-id="27d37-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="27d37-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="27d37-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="27d37-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="27d37-129">正しい</span><span class="sxs-lookup"><span data-stu-id="27d37-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="27d37-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="27d37-130">See also</span></span>



[<span data-ttu-id="27d37-131">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="27d37-131">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md)


- [<span data-ttu-id="27d37-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="27d37-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

