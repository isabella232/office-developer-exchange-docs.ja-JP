---
title: DiscoverySearchConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 085384f9-dca4-4534-82e2-dd782471d0da
description: DiscoverySearchConfiguration 要素は、電子的証拠開示検索の構成を指定します。
ms.openlocfilehash: 11bf90d8fe73bb0b308deb7ae51f1443488f87e2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760087"
---
# <a name="discoverysearchconfiguration"></a><span data-ttu-id="1cd42-103">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="1cd42-103">DiscoverySearchConfiguration</span></span>

<span data-ttu-id="1cd42-104">**DiscoverySearchConfiguration**要素は、電子的証拠開示検索の構成を指定します。</span><span class="sxs-lookup"><span data-stu-id="1cd42-104">The **DiscoverySearchConfiguration** element specifies the configuration for eDiscovery search.</span></span> 
  
```XML
<DiscoverySearchConfiguration>
    <SearchId></SearchId>
    <SearchQuery></SearchQuery>
    <SearchableMailboxes></SearchableMailboxes>
</DiscoverySearchConfiguration>
```

 <span data-ttu-id="1cd42-105">**DiscoverySearchConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="1cd42-105">**DiscoverySearchConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1cd42-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="1cd42-106">Attributes and elements</span></span>

<span data-ttu-id="1cd42-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1cd42-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1cd42-108">属性</span><span class="sxs-lookup"><span data-stu-id="1cd42-108">Attributes</span></span>

<span data-ttu-id="1cd42-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1cd42-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1cd42-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1cd42-110">Child elements</span></span>

|<span data-ttu-id="1cd42-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="1cd42-111">**Element**</span></span>|<span data-ttu-id="1cd42-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="1cd42-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1cd42-113">SearchId</span><span class="sxs-lookup"><span data-stu-id="1cd42-113">SearchId</span></span>](searchid.md) <br/> |<span data-ttu-id="1cd42-114">検索の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="1cd42-114">Specifies the identifier of the search.</span></span>  <br/> |
|[<span data-ttu-id="1cd42-115">SearchQuery</span><span class="sxs-lookup"><span data-stu-id="1cd42-115">SearchQuery</span></span>](searchquery.md) <br/> |<span data-ttu-id="1cd42-116">電子的証拠開示検索クエリの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="1cd42-116">Specifies the name of an eDiscovery search query.</span></span>  <br/> |
|[<span data-ttu-id="1cd42-117">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="1cd42-117">SearchableMailboxes</span></span>](searchablemailboxes.md) <br/> |<span data-ttu-id="1cd42-118">**GetSearchableMailboxes**要求から返されたメールボックスの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1cd42-118">Contains a list of the mailboxes returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1cd42-119">親要素</span><span class="sxs-lookup"><span data-stu-id="1cd42-119">Parent elements</span></span>

|<span data-ttu-id="1cd42-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="1cd42-120">**Element**</span></span>|<span data-ttu-id="1cd42-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="1cd42-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1cd42-122">DiscoverySearchConfigurations</span><span class="sxs-lookup"><span data-stu-id="1cd42-122">DiscoverySearchConfigurations</span></span>](discoverysearchconfigurations.md) <br/> |<span data-ttu-id="1cd42-123">**DiscoverySearchConfiguration**要素の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="1cd42-123">Specifies an array of **DiscoverySearchConfiguration** elements.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1cd42-124">備考</span><span class="sxs-lookup"><span data-stu-id="1cd42-124">Remarks</span></span>

<span data-ttu-id="1cd42-125">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="1cd42-125">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1cd42-126">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="1cd42-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1cd42-127">要素情報</span><span class="sxs-lookup"><span data-stu-id="1cd42-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1cd42-128">名前空間</span><span class="sxs-lookup"><span data-stu-id="1cd42-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1cd42-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1cd42-129">Schema Name</span></span>  <br/> |<span data-ttu-id="1cd42-130">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="1cd42-130">Message schema</span></span>  <br/> |
|<span data-ttu-id="1cd42-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1cd42-131">Validation File</span></span>  <br/> |<span data-ttu-id="1cd42-132">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1cd42-132">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1cd42-133">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="1cd42-133">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="1cd42-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="1cd42-134">See also</span></span>

- [<span data-ttu-id="1cd42-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="1cd42-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

