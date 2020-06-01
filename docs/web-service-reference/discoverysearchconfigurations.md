---
title: DiscoverySearchConfigurations
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f04b14c9-384c-4016-b113-52a49e15e73b
description: Discoverysearchconfigurations 要素は、Discoverysearchconfigurations 要素の配列を指定します。
ms.openlocfilehash: 6af4c8198f2ad73f8b39f9718e11b88aa8075c39
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461381"
---
# <a name="discoverysearchconfigurations"></a><span data-ttu-id="f76a1-103">DiscoverySearchConfigurations</span><span class="sxs-lookup"><span data-stu-id="f76a1-103">DiscoverySearchConfigurations</span></span>

<span data-ttu-id="f76a1-104">**Discoverysearchconfigurations**要素は、 **discoverysearchconfigurations**要素の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="f76a1-104">The **DiscoverySearchConfigurations** element specifies an array of **DiscoverySearchConfiguration** elements.</span></span> 
  
```XML
<DiscoverySearchConfigurations>
    <DiscoverySearchConfiguration></DiscoverySearchConfiguration>
</DiscoverySearchConfigurations>
```

 <span data-ttu-id="f76a1-105">**ArrayOfDiscoverySearchConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="f76a1-105">**ArrayOfDiscoverySearchConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f76a1-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f76a1-106">Attributes and elements</span></span>

<span data-ttu-id="f76a1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f76a1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f76a1-108">属性</span><span class="sxs-lookup"><span data-stu-id="f76a1-108">Attributes</span></span>

<span data-ttu-id="f76a1-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f76a1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f76a1-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f76a1-110">Child elements</span></span>

|<span data-ttu-id="f76a1-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="f76a1-111">**Element**</span></span>|<span data-ttu-id="f76a1-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="f76a1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f76a1-113">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="f76a1-113">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md) <br/> |<span data-ttu-id="f76a1-114">電子情報開示検索の構成を指定します。</span><span class="sxs-lookup"><span data-stu-id="f76a1-114">Specifies the configuration for eDiscovery search.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f76a1-115">親要素</span><span class="sxs-lookup"><span data-stu-id="f76a1-115">Parent elements</span></span>

|<span data-ttu-id="f76a1-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="f76a1-116">**Element**</span></span>|<span data-ttu-id="f76a1-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="f76a1-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f76a1-118">GetDiscoverySearchConfigurationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f76a1-118">GetDiscoverySearchConfigurationResponseMessage</span></span>](getdiscoverysearchconfigurationresponsemessage.md) <br/> |<span data-ttu-id="f76a1-119">**Getdiscoverysearchconfiguration**要求の応答メッセージを指定します。</span><span class="sxs-lookup"><span data-stu-id="f76a1-119">Specifies the response message for a **GetDiscoverySearchConfiguration** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f76a1-120">注釈</span><span class="sxs-lookup"><span data-stu-id="f76a1-120">Remarks</span></span>

<span data-ttu-id="f76a1-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f76a1-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f76a1-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f76a1-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f76a1-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f76a1-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f76a1-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="f76a1-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f76a1-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f76a1-125">Schema Name</span></span>  <br/> |<span data-ttu-id="f76a1-126">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="f76a1-126">Message schema</span></span>  <br/> |
|<span data-ttu-id="f76a1-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f76a1-127">Validation File</span></span>  <br/> |<span data-ttu-id="f76a1-128">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="f76a1-128">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f76a1-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f76a1-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="f76a1-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="f76a1-130">See also</span></span>

- [<span data-ttu-id="f76a1-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="f76a1-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

