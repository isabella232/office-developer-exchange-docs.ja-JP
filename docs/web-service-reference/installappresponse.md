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
ms.openlocfilehash: 0f7690e2df7e71c4e478dec191671af24f96294b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465668"
---
# <a name="installappresponse"></a><span data-ttu-id="9c741-103">InstallAppResponse</span><span class="sxs-lookup"><span data-stu-id="9c741-103">InstallAppResponse</span></span>

<span data-ttu-id="9c741-104">**InstallAppResponse**要素は、 **installapp**要求への応答を指定します。</span><span class="sxs-lookup"><span data-stu-id="9c741-104">The **InstallAppResponse** element specifies the response to an **InstallApp** request.</span></span> 
  
```xml
<InstallAppResponse ResponseClass="">
    <MessageText></MessageText>
    <ResponseCode></ResponseCode>
    <DescriptiveLinkKey></DescriptiveLinkKey>
    <MessageXml></MessageXml>
</InstallAppResponse>
```

 <span data-ttu-id="9c741-105">**InstallAppResponseType**</span><span class="sxs-lookup"><span data-stu-id="9c741-105">**InstallAppResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9c741-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9c741-106">Attributes and elements</span></span>

<span data-ttu-id="9c741-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9c741-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9c741-108">属性</span><span class="sxs-lookup"><span data-stu-id="9c741-108">Attributes</span></span>

|<span data-ttu-id="9c741-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="9c741-109">**Attribute**</span></span>|<span data-ttu-id="9c741-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="9c741-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9c741-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="9c741-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="9c741-112">応答のクラスを示します。</span><span class="sxs-lookup"><span data-stu-id="9c741-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="9c741-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="9c741-113">ResponseClass</span></span>

|<span data-ttu-id="9c741-114">**値**</span><span class="sxs-lookup"><span data-stu-id="9c741-114">**Value**</span></span>|<span data-ttu-id="9c741-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="9c741-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9c741-116">成功</span><span class="sxs-lookup"><span data-stu-id="9c741-116">Success</span></span>  <br/> |<span data-ttu-id="9c741-117">成功を示します。</span><span class="sxs-lookup"><span data-stu-id="9c741-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="9c741-118">警告</span><span class="sxs-lookup"><span data-stu-id="9c741-118">Warning</span></span>  <br/> |<span data-ttu-id="9c741-119">警告を示します。</span><span class="sxs-lookup"><span data-stu-id="9c741-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="9c741-120">Error</span><span class="sxs-lookup"><span data-stu-id="9c741-120">Error</span></span>  <br/> |<span data-ttu-id="9c741-121">エラーを示します。</span><span class="sxs-lookup"><span data-stu-id="9c741-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9c741-122">子要素</span><span class="sxs-lookup"><span data-stu-id="9c741-122">Child elements</span></span>

|<span data-ttu-id="9c741-123">**Element**</span><span class="sxs-lookup"><span data-stu-id="9c741-123">**Element**</span></span>|<span data-ttu-id="9c741-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="9c741-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9c741-125">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="9c741-125">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="9c741-126">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="9c741-126">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="9c741-127">MessageText</span><span class="sxs-lookup"><span data-stu-id="9c741-127">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="9c741-128">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="9c741-128">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="9c741-129">MessageXml</span><span class="sxs-lookup"><span data-stu-id="9c741-129">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="9c741-130">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="9c741-130">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="9c741-131">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="9c741-131">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="9c741-132">要求に関する状態情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="9c741-132">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9c741-133">親要素</span><span class="sxs-lookup"><span data-stu-id="9c741-133">Parent elements</span></span>

|<span data-ttu-id="9c741-134">**要素**</span><span class="sxs-lookup"><span data-stu-id="9c741-134">**Element**</span></span>|<span data-ttu-id="9c741-135">**説明**</span><span class="sxs-lookup"><span data-stu-id="9c741-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9c741-136">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="9c741-136">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="9c741-137">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="9c741-137">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9c741-138">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9c741-138">Text value</span></span>

<span data-ttu-id="9c741-139">なし。</span><span class="sxs-lookup"><span data-stu-id="9c741-139">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9c741-140">注釈</span><span class="sxs-lookup"><span data-stu-id="9c741-140">Remarks</span></span>

<span data-ttu-id="9c741-141">**GetAppManifestsResponseMessage**要素は、exchange Online および exchange 2013 以降のバージョンの Microsoft exchange Server を対象とするクライアントに適用されます。</span><span class="sxs-lookup"><span data-stu-id="9c741-141">The **GetAppManifestsResponseMessage** element is applicable for clients that target Exchange Online and versions of Microsoft Exchange Server starting with Exchange 2013.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="9c741-142">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9c741-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9c741-143">Namespace</span><span class="sxs-lookup"><span data-stu-id="9c741-143">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9c741-144">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9c741-144">Schema Name</span></span>  <br/> |<span data-ttu-id="9c741-145">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="9c741-145">Message schema</span></span>  <br/> |
|<span data-ttu-id="9c741-146">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9c741-146">Validation File</span></span>  <br/> |<span data-ttu-id="9c741-147">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="9c741-147">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9c741-148">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9c741-148">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="9c741-149">関連項目</span><span class="sxs-lookup"><span data-stu-id="9c741-149">See also</span></span>



- [<span data-ttu-id="9c741-150">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="9c741-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

