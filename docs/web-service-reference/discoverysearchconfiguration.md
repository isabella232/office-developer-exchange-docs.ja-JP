---
title: DiscoverySearchConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 085384f9-dca4-4534-82e2-dd782471d0da
description: DiscoverySearchConfiguration 要素は、電子情報開示検索の構成を指定します。
ms.openlocfilehash: 8819d951f35ccc215bdf0128d2a16b60bbf20f2a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529057"
---
# <a name="discoverysearchconfiguration"></a><span data-ttu-id="30930-103">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="30930-103">DiscoverySearchConfiguration</span></span>

<span data-ttu-id="30930-104">**Discoverysearchconfiguration**要素は、電子情報開示検索の構成を指定します。</span><span class="sxs-lookup"><span data-stu-id="30930-104">The **DiscoverySearchConfiguration** element specifies the configuration for eDiscovery search.</span></span> 
  
```XML
<DiscoverySearchConfiguration>
    <SearchId></SearchId>
    <SearchQuery></SearchQuery>
    <SearchableMailboxes></SearchableMailboxes>
</DiscoverySearchConfiguration>
```

 <span data-ttu-id="30930-105">**DiscoverySearchConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="30930-105">**DiscoverySearchConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="30930-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="30930-106">Attributes and elements</span></span>

<span data-ttu-id="30930-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="30930-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="30930-108">属性</span><span class="sxs-lookup"><span data-stu-id="30930-108">Attributes</span></span>

<span data-ttu-id="30930-109">なし。</span><span class="sxs-lookup"><span data-stu-id="30930-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="30930-110">子要素</span><span class="sxs-lookup"><span data-stu-id="30930-110">Child elements</span></span>

|<span data-ttu-id="30930-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="30930-111">**Element**</span></span>|<span data-ttu-id="30930-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="30930-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="30930-113">SearchId</span><span class="sxs-lookup"><span data-stu-id="30930-113">SearchId</span></span>](searchid.md) <br/> |<span data-ttu-id="30930-114">検索の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="30930-114">Specifies the identifier of the search.</span></span>  <br/> |
|[<span data-ttu-id="30930-115">SearchQuery</span><span class="sxs-lookup"><span data-stu-id="30930-115">SearchQuery</span></span>](searchquery.md) <br/> |<span data-ttu-id="30930-116">電子情報開示検索クエリの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="30930-116">Specifies the name of an eDiscovery search query.</span></span>  <br/> |
|[<span data-ttu-id="30930-117">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="30930-117">SearchableMailboxes</span></span>](searchablemailboxes.md) <br/> |<span data-ttu-id="30930-118">**Getsearchablemailbyrequest**から返されるメールボックスの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="30930-118">Contains a list of the mailboxes returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="30930-119">親要素</span><span class="sxs-lookup"><span data-stu-id="30930-119">Parent elements</span></span>

|<span data-ttu-id="30930-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="30930-120">**Element**</span></span>|<span data-ttu-id="30930-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="30930-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="30930-122">DiscoverySearchConfigurations</span><span class="sxs-lookup"><span data-stu-id="30930-122">DiscoverySearchConfigurations</span></span>](discoverysearchconfigurations.md) <br/> |<span data-ttu-id="30930-123">**Discoverysearchconfiguration**要素の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="30930-123">Specifies an array of **DiscoverySearchConfiguration** elements.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="30930-124">注釈</span><span class="sxs-lookup"><span data-stu-id="30930-124">Remarks</span></span>

<span data-ttu-id="30930-125">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="30930-125">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="30930-126">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="30930-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="30930-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="30930-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="30930-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="30930-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="30930-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="30930-129">Schema Name</span></span>  <br/> |<span data-ttu-id="30930-130">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="30930-130">Message schema</span></span>  <br/> |
|<span data-ttu-id="30930-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="30930-131">Validation File</span></span>  <br/> |<span data-ttu-id="30930-132">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="30930-132">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="30930-133">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="30930-133">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="30930-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="30930-134">See also</span></span>

- [<span data-ttu-id="30930-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="30930-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

