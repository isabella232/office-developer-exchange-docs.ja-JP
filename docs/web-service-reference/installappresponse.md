---
title: InstallAppResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c5e0582d-c1e1-453b-93ed-c31165c82697
description: InstallAppResponse 要素は、InstallApp 要求への応答を指定します。
ms.openlocfilehash: 8e8da720b3a38e979b3d83810bb798350822146c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831942"
---
# <a name="installappresponse"></a><span data-ttu-id="31e23-103">InstallAppResponse</span><span class="sxs-lookup"><span data-stu-id="31e23-103">InstallAppResponse</span></span>

<span data-ttu-id="31e23-104">**InstallAppResponse**要素は、 **InstallApp**要求への応答を指定します。</span><span class="sxs-lookup"><span data-stu-id="31e23-104">The **InstallAppResponse** element specifies the response to an **InstallApp** request.</span></span> 
  
```xml
<InstallAppResponse ResponseClass="">
    <MessageText></MessageText>
    <ResponseCode></ResponseCode>
    <DescriptiveLinkKey></DescriptiveLinkKey>
    <MessageXml></MessageXml>
</InstallAppResponse>
```

 <span data-ttu-id="31e23-105">**InstallAppResponseType**</span><span class="sxs-lookup"><span data-stu-id="31e23-105">**InstallAppResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="31e23-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="31e23-106">Attributes and elements</span></span>

<span data-ttu-id="31e23-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="31e23-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="31e23-108">属性</span><span class="sxs-lookup"><span data-stu-id="31e23-108">Attributes</span></span>

|<span data-ttu-id="31e23-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="31e23-109">**Attribute**</span></span>|<span data-ttu-id="31e23-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="31e23-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="31e23-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="31e23-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="31e23-112">応答のクラスを示します。</span><span class="sxs-lookup"><span data-stu-id="31e23-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="31e23-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="31e23-113">ResponseClass</span></span>

|<span data-ttu-id="31e23-114">**値**</span><span class="sxs-lookup"><span data-stu-id="31e23-114">**Value**</span></span>|<span data-ttu-id="31e23-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="31e23-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="31e23-116">成功</span><span class="sxs-lookup"><span data-stu-id="31e23-116">Success</span></span>  <br/> |<span data-ttu-id="31e23-117">成功を示します。</span><span class="sxs-lookup"><span data-stu-id="31e23-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="31e23-118">警告</span><span class="sxs-lookup"><span data-stu-id="31e23-118">Warning</span></span>  <br/> |<span data-ttu-id="31e23-119">警告を示します。</span><span class="sxs-lookup"><span data-stu-id="31e23-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="31e23-120">エラー</span><span class="sxs-lookup"><span data-stu-id="31e23-120">Error</span></span>  <br/> |<span data-ttu-id="31e23-121">エラーを示します。</span><span class="sxs-lookup"><span data-stu-id="31e23-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="31e23-122">子要素</span><span class="sxs-lookup"><span data-stu-id="31e23-122">Child elements</span></span>

|<span data-ttu-id="31e23-123">**要素**</span><span class="sxs-lookup"><span data-stu-id="31e23-123">**Element**</span></span>|<span data-ttu-id="31e23-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="31e23-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="31e23-125">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="31e23-125">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="31e23-126">現在使用されていない、将来使用するために予約されています。</span><span class="sxs-lookup"><span data-stu-id="31e23-126">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="31e23-127">MessageText</span><span class="sxs-lookup"><span data-stu-id="31e23-127">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="31e23-128">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="31e23-128">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="31e23-129">MessageXml</span><span class="sxs-lookup"><span data-stu-id="31e23-129">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="31e23-130">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="31e23-130">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="31e23-131">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="31e23-131">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="31e23-132">要求に関するステータス情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="31e23-132">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="31e23-133">親要素</span><span class="sxs-lookup"><span data-stu-id="31e23-133">Parent elements</span></span>

|<span data-ttu-id="31e23-134">**要素**</span><span class="sxs-lookup"><span data-stu-id="31e23-134">**Element**</span></span>|<span data-ttu-id="31e23-135">**説明**</span><span class="sxs-lookup"><span data-stu-id="31e23-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="31e23-136">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="31e23-136">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="31e23-137">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="31e23-137">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="31e23-138">テキスト値</span><span class="sxs-lookup"><span data-stu-id="31e23-138">Text value</span></span>

<span data-ttu-id="31e23-139">なし。</span><span class="sxs-lookup"><span data-stu-id="31e23-139">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="31e23-140">備考</span><span class="sxs-lookup"><span data-stu-id="31e23-140">Remarks</span></span>

<span data-ttu-id="31e23-141">**GetAppManifestsResponseMessage**要素は、オンラインの Exchange および Exchange 2013 を起動する Microsoft Exchange Server のバージョンを対象とするクライアントに適用されます。</span><span class="sxs-lookup"><span data-stu-id="31e23-141">The **GetAppManifestsResponseMessage** element is applicable for clients that target Exchange Online and versions of Microsoft Exchange Server starting with Exchange 2013.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="31e23-142">要素情報</span><span class="sxs-lookup"><span data-stu-id="31e23-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="31e23-143">名前空間</span><span class="sxs-lookup"><span data-stu-id="31e23-143">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="31e23-144">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="31e23-144">Schema Name</span></span>  <br/> |<span data-ttu-id="31e23-145">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="31e23-145">Message schema</span></span>  <br/> |
|<span data-ttu-id="31e23-146">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="31e23-146">Validation File</span></span>  <br/> |<span data-ttu-id="31e23-147">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="31e23-147">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="31e23-148">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="31e23-148">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="31e23-149">関連項目</span><span class="sxs-lookup"><span data-stu-id="31e23-149">See also</span></span>



- [<span data-ttu-id="31e23-150">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="31e23-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

