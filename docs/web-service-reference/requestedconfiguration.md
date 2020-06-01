---
title: RequestedConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RequestedConfiguration
api_type:
- schema
ms.assetid: 24921387-f676-49e6-8d7a-ef3115024866
description: RequestedConfiguration 要素には、要求されたサービス構成が含まれています。
ms.openlocfilehash: bbc503e6d6f7c56c785365924106bc2468965d0b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457152"
---
# <a name="requestedconfiguration"></a><span data-ttu-id="2cb61-103">RequestedConfiguration</span><span class="sxs-lookup"><span data-stu-id="2cb61-103">RequestedConfiguration</span></span>

<span data-ttu-id="2cb61-104">**Requestedconfiguration**要素には、要求されたサービス構成が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2cb61-104">The **RequestedConfiguration** element contains the requested service configurations.</span></span> 
  
```XML
<RequestedConfiguration>
   <ConfigurationName/>
</RequestedConfiguration>
```

 <span data-ttu-id="2cb61-105">**ArrayOfServiceConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="2cb61-105">**ArrayOfServiceConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2cb61-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="2cb61-106">Attributes and elements</span></span>

<span data-ttu-id="2cb61-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2cb61-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2cb61-108">属性</span><span class="sxs-lookup"><span data-stu-id="2cb61-108">Attributes</span></span>

<span data-ttu-id="2cb61-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2cb61-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2cb61-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2cb61-110">Child elements</span></span>

|<span data-ttu-id="2cb61-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="2cb61-111">**Element**</span></span>|<span data-ttu-id="2cb61-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="2cb61-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2cb61-113">ConfigurationName</span><span class="sxs-lookup"><span data-stu-id="2cb61-113">ConfigurationName</span></span>](configurationname.md) <br/> |<span data-ttu-id="2cb61-114">要求されたサービス構成を名前で指定します。</span><span class="sxs-lookup"><span data-stu-id="2cb61-114">Specifies the requested service configurations by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2cb61-115">親要素</span><span class="sxs-lookup"><span data-stu-id="2cb61-115">Parent elements</span></span>

|<span data-ttu-id="2cb61-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="2cb61-116">**Element**</span></span>|<span data-ttu-id="2cb61-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="2cb61-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2cb61-118">GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="2cb61-118">GetServiceConfiguration</span></span>](getserviceconfiguration.md) <br/> |<span data-ttu-id="2cb61-119">GetServiceConfiguration 要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="2cb61-119">Defines a GetServiceConfiguration request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2cb61-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="2cb61-120">Text value</span></span>

<span data-ttu-id="2cb61-121">なし。</span><span class="sxs-lookup"><span data-stu-id="2cb61-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2cb61-122">注釈</span><span class="sxs-lookup"><span data-stu-id="2cb61-122">Remarks</span></span>

<span data-ttu-id="2cb61-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2cb61-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2cb61-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="2cb61-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2cb61-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="2cb61-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2cb61-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2cb61-126">Schema Name</span></span>  <br/> |<span data-ttu-id="2cb61-127">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="2cb61-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2cb61-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2cb61-128">Validation File</span></span>  <br/> |<span data-ttu-id="2cb61-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="2cb61-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2cb61-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="2cb61-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="2cb61-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="2cb61-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2cb61-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="2cb61-132">See also</span></span>



- [<span data-ttu-id="2cb61-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="2cb61-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

