---
title: DiscoverySearchConfigurations
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f04b14c9-384c-4016-b113-52a49e15e73b
description: DiscoverySearchConfigurations 要素は、DiscoverySearchConfiguration 要素の配列を指定します。
ms.openlocfilehash: a95bb35b88114e8e72e22de424679993fd4eef2a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760096"
---
# <a name="discoverysearchconfigurations"></a><span data-ttu-id="6587b-103">DiscoverySearchConfigurations</span><span class="sxs-lookup"><span data-stu-id="6587b-103">DiscoverySearchConfigurations</span></span>

<span data-ttu-id="6587b-104">**DiscoverySearchConfigurations**要素は、 **DiscoverySearchConfiguration**要素の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="6587b-104">The **DiscoverySearchConfigurations** element specifies an array of **DiscoverySearchConfiguration** elements.</span></span> 
  
```XML
<DiscoverySearchConfigurations>
    <DiscoverySearchConfiguration></DiscoverySearchConfiguration>
</DiscoverySearchConfigurations>
```

 <span data-ttu-id="6587b-105">**ArrayOfDiscoverySearchConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="6587b-105">**ArrayOfDiscoverySearchConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6587b-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6587b-106">Attributes and elements</span></span>

<span data-ttu-id="6587b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6587b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6587b-108">属性</span><span class="sxs-lookup"><span data-stu-id="6587b-108">Attributes</span></span>

<span data-ttu-id="6587b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6587b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6587b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6587b-110">Child elements</span></span>

|<span data-ttu-id="6587b-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="6587b-111">**Element**</span></span>|<span data-ttu-id="6587b-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="6587b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6587b-113">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="6587b-113">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md) <br/> |<span data-ttu-id="6587b-114">電子的証拠開示検索の構成を指定します。</span><span class="sxs-lookup"><span data-stu-id="6587b-114">Specifies the configuration for eDiscovery search.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6587b-115">親要素</span><span class="sxs-lookup"><span data-stu-id="6587b-115">Parent elements</span></span>

|<span data-ttu-id="6587b-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="6587b-116">**Element**</span></span>|<span data-ttu-id="6587b-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="6587b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6587b-118">GetDiscoverySearchConfigurationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="6587b-118">GetDiscoverySearchConfigurationResponseMessage</span></span>](getdiscoverysearchconfigurationresponsemessage.md) <br/> |<span data-ttu-id="6587b-119">**GetDiscoverySearchConfiguration**要求の応答メッセージを指定します。</span><span class="sxs-lookup"><span data-stu-id="6587b-119">Specifies the response message for a **GetDiscoverySearchConfiguration** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6587b-120">備考</span><span class="sxs-lookup"><span data-stu-id="6587b-120">Remarks</span></span>

<span data-ttu-id="6587b-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6587b-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6587b-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6587b-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6587b-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="6587b-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6587b-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="6587b-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6587b-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6587b-125">Schema Name</span></span>  <br/> |<span data-ttu-id="6587b-126">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="6587b-126">Message schema</span></span>  <br/> |
|<span data-ttu-id="6587b-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6587b-127">Validation File</span></span>  <br/> |<span data-ttu-id="6587b-128">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6587b-128">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6587b-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6587b-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="6587b-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="6587b-130">See also</span></span>

- [<span data-ttu-id="6587b-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="6587b-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

