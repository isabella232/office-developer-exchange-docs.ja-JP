---
title: GetAppMarketplaceUrlResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dc3368ec-78c2-4f8d-8394-4891e90dafd2
description: GetAppMarketplaceUrlResponse 要素は、GetAppMarketplaceUrl 要求への応答を指定します。
ms.openlocfilehash: 553ebfc4615280c77d4a1ef9e5db3e5d10a0f2a4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760634"
---
# <a name="getappmarketplaceurlresponse"></a><span data-ttu-id="b160f-103">GetAppMarketplaceUrlResponse</span><span class="sxs-lookup"><span data-stu-id="b160f-103">GetAppMarketplaceUrlResponse</span></span>

<span data-ttu-id="b160f-104">**GetAppMarketplaceUrlResponse**要素は、 **GetAppMarketplaceUrl**要求への応答を指定します。</span><span class="sxs-lookup"><span data-stu-id="b160f-104">The **GetAppMarketplaceUrlResponse** element specifies the response to a **GetAppMarketplaceUrl** request.</span></span> 
  
```XML
<GetAppMarketplaceUrlResponse ResponseClass=" Success | Warning | Error ">
    <AppMarketplaceUrl/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetAppMarketplaceUrlResponse>
```

 <span data-ttu-id="b160f-105">**GetAppMarketplaceUrlResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="b160f-105">**GetAppMarketplaceUrlResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b160f-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b160f-106">Attributes and elements</span></span>

<span data-ttu-id="b160f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b160f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b160f-108">属性</span><span class="sxs-lookup"><span data-stu-id="b160f-108">Attributes</span></span>

|<span data-ttu-id="b160f-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="b160f-109">**Attribute**</span></span>|<span data-ttu-id="b160f-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="b160f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b160f-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="b160f-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="b160f-112">応答のクラスを示します。</span><span class="sxs-lookup"><span data-stu-id="b160f-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="b160f-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="b160f-113">ResponseClass</span></span>

|<span data-ttu-id="b160f-114">**値**</span><span class="sxs-lookup"><span data-stu-id="b160f-114">**Value**</span></span>|<span data-ttu-id="b160f-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="b160f-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b160f-116">成功</span><span class="sxs-lookup"><span data-stu-id="b160f-116">Success</span></span>  <br/> |<span data-ttu-id="b160f-117">成功を示します。</span><span class="sxs-lookup"><span data-stu-id="b160f-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="b160f-118">警告</span><span class="sxs-lookup"><span data-stu-id="b160f-118">Warning</span></span>  <br/> |<span data-ttu-id="b160f-119">警告を示します。</span><span class="sxs-lookup"><span data-stu-id="b160f-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="b160f-120">エラー</span><span class="sxs-lookup"><span data-stu-id="b160f-120">Error</span></span>  <br/> |<span data-ttu-id="b160f-121">エラーを示します。</span><span class="sxs-lookup"><span data-stu-id="b160f-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b160f-122">子要素</span><span class="sxs-lookup"><span data-stu-id="b160f-122">Child elements</span></span>

|<span data-ttu-id="b160f-123">**要素**</span><span class="sxs-lookup"><span data-stu-id="b160f-123">**Element**</span></span>|<span data-ttu-id="b160f-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="b160f-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b160f-125">AppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="b160f-125">AppMarketplaceUrl</span></span>](appmarketplaceurl.md) <br/> |<span data-ttu-id="b160f-126">アプリケーションの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="b160f-126">Specifies the URL for the app.</span></span>  <br/> |
|[<span data-ttu-id="b160f-127">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="b160f-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="b160f-128">現在使用されていない、将来使用するために予約されています。</span><span class="sxs-lookup"><span data-stu-id="b160f-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="b160f-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="b160f-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="b160f-130">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="b160f-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="b160f-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="b160f-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="b160f-132">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="b160f-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="b160f-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b160f-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="b160f-134">要求に関するステータス情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="b160f-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b160f-135">親要素</span><span class="sxs-lookup"><span data-stu-id="b160f-135">Parent elements</span></span>

|<span data-ttu-id="b160f-136">**要素**</span><span class="sxs-lookup"><span data-stu-id="b160f-136">**Element**</span></span>|<span data-ttu-id="b160f-137">**説明**</span><span class="sxs-lookup"><span data-stu-id="b160f-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b160f-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b160f-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="b160f-139">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="b160f-139">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b160f-140">備考</span><span class="sxs-lookup"><span data-stu-id="b160f-140">Remarks</span></span>

<span data-ttu-id="b160f-141">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b160f-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b160f-142">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b160f-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b160f-143">要素情報</span><span class="sxs-lookup"><span data-stu-id="b160f-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b160f-144">名前空間</span><span class="sxs-lookup"><span data-stu-id="b160f-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b160f-145">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b160f-145">Schema Name</span></span>  <br/> |<span data-ttu-id="b160f-146">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="b160f-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="b160f-147">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b160f-147">Validation File</span></span>  <br/> |<span data-ttu-id="b160f-148">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b160f-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b160f-149">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b160f-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="b160f-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="b160f-150">See also</span></span>



- [<span data-ttu-id="b160f-151">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="b160f-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

