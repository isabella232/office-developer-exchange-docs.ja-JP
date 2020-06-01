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
description: ResponseMessages 要素には、サービス構成応答メッセージの配列が含まれています。
ms.openlocfilehash: cf271224141ffeb6dc00069abf430ab33d3ca2fa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457453"
---
# <a name="responsemessages-arrayofserviceconfigurationresponsemessagetype"></a><span data-ttu-id="b8982-103">ResponseMessages (ArrayOfServiceConfigurationResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="b8982-103">ResponseMessages (ArrayOfServiceConfigurationResponseMessageType)</span></span>

<span data-ttu-id="b8982-104">**Responsemessages**要素には、サービス構成応答メッセージの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b8982-104">The **ResponseMessages** element contains an array of service configuration response messages.</span></span> 
  
```XML
<ResponseMessages>
   <ServiceConfigurationResponseMessageType/>
</ResponseMessages>
```

 <span data-ttu-id="b8982-105">**ArrayOfServiceConfigurationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="b8982-105">**ArrayOfServiceConfigurationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b8982-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b8982-106">Attributes and elements</span></span>

<span data-ttu-id="b8982-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b8982-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b8982-108">属性</span><span class="sxs-lookup"><span data-stu-id="b8982-108">Attributes</span></span>

<span data-ttu-id="b8982-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b8982-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b8982-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b8982-110">Child elements</span></span>

|<span data-ttu-id="b8982-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="b8982-111">**Element**</span></span>|<span data-ttu-id="b8982-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="b8982-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b8982-113">ServiceConfigurationResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="b8982-113">ServiceConfigurationResponseMessageType</span></span>](serviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="b8982-114">サービス構成の設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="b8982-114">Contains service configuration settings.</span></span> <span data-ttu-id="b8982-115">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="b8982-115">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b8982-116">親要素</span><span class="sxs-lookup"><span data-stu-id="b8982-116">Parent elements</span></span>

|<span data-ttu-id="b8982-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="b8982-117">**Element**</span></span>|<span data-ttu-id="b8982-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="b8982-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b8982-119">GetServiceConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="b8982-119">GetServiceConfigurationResponse</span></span>](getserviceconfigurationresponse.md) <br/> |<span data-ttu-id="b8982-120">GetServiceConfiguration 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="b8982-120">Defines a response to a GetServiceConfiguration request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b8982-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b8982-121">Text value</span></span>

<span data-ttu-id="b8982-122">なし。</span><span class="sxs-lookup"><span data-stu-id="b8982-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b8982-123">注釈</span><span class="sxs-lookup"><span data-stu-id="b8982-123">Remarks</span></span>

<span data-ttu-id="b8982-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b8982-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b8982-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b8982-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b8982-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="b8982-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b8982-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b8982-127">Schema Name</span></span>  <br/> |<span data-ttu-id="b8982-128">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="b8982-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b8982-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b8982-129">Validation File</span></span>  <br/> |<span data-ttu-id="b8982-130">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="b8982-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b8982-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b8982-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="b8982-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="b8982-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b8982-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="b8982-133">See also</span></span>



- [<span data-ttu-id="b8982-134">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="b8982-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

