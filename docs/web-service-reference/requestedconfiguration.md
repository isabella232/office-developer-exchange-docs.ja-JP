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
description: RequestedConfiguration 要素には、要求されたサービスの構成が含まれています。
ms.openlocfilehash: 1edc6394360250c9a9810fe614c975cb48eba3f0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833130"
---
# <a name="requestedconfiguration"></a><span data-ttu-id="c40e7-103">RequestedConfiguration</span><span class="sxs-lookup"><span data-stu-id="c40e7-103">RequestedConfiguration</span></span>

<span data-ttu-id="c40e7-104">**RequestedConfiguration**要素には、要求されたサービスの構成が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c40e7-104">The **RequestedConfiguration** element contains the requested service configurations.</span></span> 
  
```XML
<RequestedConfiguration>
   <ConfigurationName/>
</RequestedConfiguration>
```

 <span data-ttu-id="c40e7-105">**ArrayOfServiceConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="c40e7-105">**ArrayOfServiceConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c40e7-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="c40e7-106">Attributes and elements</span></span>

<span data-ttu-id="c40e7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c40e7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c40e7-108">属性</span><span class="sxs-lookup"><span data-stu-id="c40e7-108">Attributes</span></span>

<span data-ttu-id="c40e7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c40e7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c40e7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c40e7-110">Child elements</span></span>

|<span data-ttu-id="c40e7-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="c40e7-111">**Element**</span></span>|<span data-ttu-id="c40e7-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="c40e7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c40e7-113">ConfigurationName</span><span class="sxs-lookup"><span data-stu-id="c40e7-113">ConfigurationName</span></span>](configurationname.md) <br/> |<span data-ttu-id="c40e7-114">要求されたサービスの構成の名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="c40e7-114">Specifies the requested service configurations by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c40e7-115">親要素</span><span class="sxs-lookup"><span data-stu-id="c40e7-115">Parent elements</span></span>

|<span data-ttu-id="c40e7-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="c40e7-116">**Element**</span></span>|<span data-ttu-id="c40e7-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="c40e7-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c40e7-118">GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="c40e7-118">GetServiceConfiguration</span></span>](getserviceconfiguration.md) <br/> |<span data-ttu-id="c40e7-119">GetServiceConfiguration 要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="c40e7-119">Defines a GetServiceConfiguration request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c40e7-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c40e7-120">Text value</span></span>

<span data-ttu-id="c40e7-121">なし。</span><span class="sxs-lookup"><span data-stu-id="c40e7-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c40e7-122">備考</span><span class="sxs-lookup"><span data-stu-id="c40e7-122">Remarks</span></span>

<span data-ttu-id="c40e7-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="c40e7-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c40e7-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="c40e7-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c40e7-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="c40e7-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c40e7-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c40e7-126">Schema Name</span></span>  <br/> |<span data-ttu-id="c40e7-127">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="c40e7-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c40e7-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c40e7-128">Validation File</span></span>  <br/> |<span data-ttu-id="c40e7-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c40e7-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c40e7-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c40e7-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="c40e7-131">False</span><span class="sxs-lookup"><span data-stu-id="c40e7-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c40e7-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="c40e7-132">See also</span></span>



- [<span data-ttu-id="c40e7-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="c40e7-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

