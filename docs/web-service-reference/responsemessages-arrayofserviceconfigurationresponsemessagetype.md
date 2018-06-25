---
title: ResponseMessages (ArrayOfServiceConfigurationResponseMessageType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseMessages
api_type:
- schema
ms.assetid: c7cfa0d1-fcb2-441f-8489-3a549da33b34
description: ResponseMessages 要素には、サービス構成の応答メッセージの配列が含まれています。
ms.openlocfilehash: af8a6db8d6e9d3ec76b532a81ef2a7392dcfde7a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833194"
---
# <a name="responsemessages-arrayofserviceconfigurationresponsemessagetype"></a><span data-ttu-id="fd216-103">ResponseMessages (ArrayOfServiceConfigurationResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="fd216-103">ResponseMessages (ArrayOfServiceConfigurationResponseMessageType)</span></span>

<span data-ttu-id="fd216-104">**ResponseMessages**要素には、サービス構成の応答メッセージの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="fd216-104">The **ResponseMessages** element contains an array of service configuration response messages.</span></span> 
  
```XML
<ResponseMessages>
   <ServiceConfigurationResponseMessageType/>
</ResponseMessages>
```

 <span data-ttu-id="fd216-105">**ArrayOfServiceConfigurationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="fd216-105">**ArrayOfServiceConfigurationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fd216-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="fd216-106">Attributes and elements</span></span>

<span data-ttu-id="fd216-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fd216-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fd216-108">属性</span><span class="sxs-lookup"><span data-stu-id="fd216-108">Attributes</span></span>

<span data-ttu-id="fd216-109">なし。</span><span class="sxs-lookup"><span data-stu-id="fd216-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fd216-110">子要素</span><span class="sxs-lookup"><span data-stu-id="fd216-110">Child elements</span></span>

|<span data-ttu-id="fd216-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="fd216-111">**Element**</span></span>|<span data-ttu-id="fd216-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="fd216-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fd216-113">ServiceConfigurationResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="fd216-113">ServiceConfigurationResponseMessageType</span></span>](serviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="fd216-114">サービス構成の設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="fd216-114">Contains service configuration settings.</span></span> <span data-ttu-id="fd216-115">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="fd216-115">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fd216-116">親要素</span><span class="sxs-lookup"><span data-stu-id="fd216-116">Parent elements</span></span>

|<span data-ttu-id="fd216-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="fd216-117">**Element**</span></span>|<span data-ttu-id="fd216-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="fd216-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fd216-119">GetServiceConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="fd216-119">GetServiceConfigurationResponse</span></span>](getserviceconfigurationresponse.md) <br/> |<span data-ttu-id="fd216-120">GetServiceConfiguration 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="fd216-120">Defines a response to a GetServiceConfiguration request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fd216-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="fd216-121">Text value</span></span>

<span data-ttu-id="fd216-122">なし。</span><span class="sxs-lookup"><span data-stu-id="fd216-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fd216-123">備考</span><span class="sxs-lookup"><span data-stu-id="fd216-123">Remarks</span></span>

<span data-ttu-id="fd216-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="fd216-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fd216-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="fd216-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fd216-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="fd216-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fd216-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fd216-127">Schema Name</span></span>  <br/> |<span data-ttu-id="fd216-128">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="fd216-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fd216-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fd216-129">Validation File</span></span>  <br/> |<span data-ttu-id="fd216-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fd216-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fd216-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="fd216-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="fd216-132">False</span><span class="sxs-lookup"><span data-stu-id="fd216-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fd216-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="fd216-133">See also</span></span>



- [<span data-ttu-id="fd216-134">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="fd216-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

