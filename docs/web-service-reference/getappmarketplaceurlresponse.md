---
title: GetAppMarketplaceUrlResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dc3368ec-78c2-4f8d-8394-4891e90dafd2
description: GetAppMarketplaceUrlResponse 要素は、GetAppMarketplaceUrl 要求に対する応答を指定します。
ms.openlocfilehash: 7ff000908a2f73f41575cae8a7795644dd60565d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530854"
---
# <a name="getappmarketplaceurlresponse"></a><span data-ttu-id="0bd60-103">GetAppMarketplaceUrlResponse</span><span class="sxs-lookup"><span data-stu-id="0bd60-103">GetAppMarketplaceUrlResponse</span></span>

<span data-ttu-id="0bd60-104">**GetAppMarketplaceUrlResponse**要素は、 **GetAppMarketplaceUrl**要求に対する応答を指定します。</span><span class="sxs-lookup"><span data-stu-id="0bd60-104">The **GetAppMarketplaceUrlResponse** element specifies the response to a **GetAppMarketplaceUrl** request.</span></span> 
  
```XML
<GetAppMarketplaceUrlResponse ResponseClass=" Success | Warning | Error ">
    <AppMarketplaceUrl/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetAppMarketplaceUrlResponse>
```

 <span data-ttu-id="0bd60-105">**GetAppMarketplaceUrlResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="0bd60-105">**GetAppMarketplaceUrlResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0bd60-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0bd60-106">Attributes and elements</span></span>

<span data-ttu-id="0bd60-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0bd60-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0bd60-108">属性</span><span class="sxs-lookup"><span data-stu-id="0bd60-108">Attributes</span></span>

|<span data-ttu-id="0bd60-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="0bd60-109">**Attribute**</span></span>|<span data-ttu-id="0bd60-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="0bd60-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0bd60-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="0bd60-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="0bd60-112">応答のクラスを示します。</span><span class="sxs-lookup"><span data-stu-id="0bd60-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="0bd60-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="0bd60-113">ResponseClass</span></span>

|<span data-ttu-id="0bd60-114">**値**</span><span class="sxs-lookup"><span data-stu-id="0bd60-114">**Value**</span></span>|<span data-ttu-id="0bd60-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="0bd60-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0bd60-116">成功</span><span class="sxs-lookup"><span data-stu-id="0bd60-116">Success</span></span>  <br/> |<span data-ttu-id="0bd60-117">成功を示します。</span><span class="sxs-lookup"><span data-stu-id="0bd60-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="0bd60-118">警告</span><span class="sxs-lookup"><span data-stu-id="0bd60-118">Warning</span></span>  <br/> |<span data-ttu-id="0bd60-119">警告を示します。</span><span class="sxs-lookup"><span data-stu-id="0bd60-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="0bd60-120">Error</span><span class="sxs-lookup"><span data-stu-id="0bd60-120">Error</span></span>  <br/> |<span data-ttu-id="0bd60-121">エラーを示します。</span><span class="sxs-lookup"><span data-stu-id="0bd60-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0bd60-122">子要素</span><span class="sxs-lookup"><span data-stu-id="0bd60-122">Child elements</span></span>

|<span data-ttu-id="0bd60-123">**Element**</span><span class="sxs-lookup"><span data-stu-id="0bd60-123">**Element**</span></span>|<span data-ttu-id="0bd60-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="0bd60-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0bd60-125">AppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="0bd60-125">AppMarketplaceUrl</span></span>](appmarketplaceurl.md) <br/> |<span data-ttu-id="0bd60-126">アプリの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="0bd60-126">Specifies the URL for the app.</span></span>  <br/> |
|[<span data-ttu-id="0bd60-127">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="0bd60-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="0bd60-128">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="0bd60-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="0bd60-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="0bd60-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="0bd60-130">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="0bd60-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="0bd60-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="0bd60-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="0bd60-132">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="0bd60-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="0bd60-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0bd60-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="0bd60-134">要求に関する状態情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="0bd60-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0bd60-135">親要素</span><span class="sxs-lookup"><span data-stu-id="0bd60-135">Parent elements</span></span>

|<span data-ttu-id="0bd60-136">**要素**</span><span class="sxs-lookup"><span data-stu-id="0bd60-136">**Element**</span></span>|<span data-ttu-id="0bd60-137">**説明**</span><span class="sxs-lookup"><span data-stu-id="0bd60-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0bd60-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0bd60-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="0bd60-139">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="0bd60-139">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0bd60-140">注釈</span><span class="sxs-lookup"><span data-stu-id="0bd60-140">Remarks</span></span>

<span data-ttu-id="0bd60-141">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="0bd60-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0bd60-142">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="0bd60-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0bd60-143">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0bd60-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0bd60-144">Namespace</span><span class="sxs-lookup"><span data-stu-id="0bd60-144">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0bd60-145">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0bd60-145">Schema Name</span></span>  <br/> |<span data-ttu-id="0bd60-146">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="0bd60-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="0bd60-147">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0bd60-147">Validation File</span></span>  <br/> |<span data-ttu-id="0bd60-148">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="0bd60-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0bd60-149">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="0bd60-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="0bd60-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="0bd60-150">See also</span></span>



- [<span data-ttu-id="0bd60-151">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="0bd60-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

