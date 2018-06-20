---
title: ArchiveItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2ac58d6f-e019-4352-b82f-8ac67a171e63
description: ArchiveItemResponseMessage 要素は、ArchiveItem の要求に応答メッセージを指定します。
ms.openlocfilehash: a7832e2cb4ec91a0871de5979fd1b418c0626aa6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759434"
---
# <a name="archiveitemresponsemessage"></a><span data-ttu-id="6cac5-103">ArchiveItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="6cac5-103">ArchiveItemResponseMessage</span></span>

<span data-ttu-id="6cac5-104">**ArchiveItemResponseMessage**要素は、 **ArchiveItem**の要求に応答メッセージを指定します。</span><span class="sxs-lookup"><span data-stu-id="6cac5-104">The **ArchiveItemResponseMessage** element specifies the response message to an **ArchiveItem** request.</span></span> 
  
```XML
<ArchiveItemResponseMessage ResponseClass="">
    <MessageText></MessageText>
    <ResponseCode></ResponseCode>
    <DescriptiveLinkKey></DescriptiveLinkKey>
    <MessageXml></MessageXml>
    <Items></Items>
</ArchiveItemResponseMessage>
```

 <span data-ttu-id="6cac5-105">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="6cac5-105">**ItemInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6cac5-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6cac5-106">Attributes and elements</span></span>

<span data-ttu-id="6cac5-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6cac5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6cac5-108">属性</span><span class="sxs-lookup"><span data-stu-id="6cac5-108">Attributes</span></span>

|<span data-ttu-id="6cac5-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="6cac5-109">**Attribute**</span></span>|<span data-ttu-id="6cac5-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="6cac5-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6cac5-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="6cac5-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="6cac5-112">応答のクラスを示します。</span><span class="sxs-lookup"><span data-stu-id="6cac5-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="6cac5-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="6cac5-113">ResponseClass</span></span>

|<span data-ttu-id="6cac5-114">**値**</span><span class="sxs-lookup"><span data-stu-id="6cac5-114">**Value**</span></span>|<span data-ttu-id="6cac5-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="6cac5-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6cac5-116">成功</span><span class="sxs-lookup"><span data-stu-id="6cac5-116">Success</span></span>  <br/> |<span data-ttu-id="6cac5-117">成功を示します。</span><span class="sxs-lookup"><span data-stu-id="6cac5-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="6cac5-118">警告</span><span class="sxs-lookup"><span data-stu-id="6cac5-118">Warning</span></span>  <br/> |<span data-ttu-id="6cac5-119">警告を示します。</span><span class="sxs-lookup"><span data-stu-id="6cac5-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="6cac5-120">エラー</span><span class="sxs-lookup"><span data-stu-id="6cac5-120">Error</span></span>  <br/> |<span data-ttu-id="6cac5-121">エラーを示します。</span><span class="sxs-lookup"><span data-stu-id="6cac5-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6cac5-122">子要素</span><span class="sxs-lookup"><span data-stu-id="6cac5-122">Child elements</span></span>

|<span data-ttu-id="6cac5-123">**要素**</span><span class="sxs-lookup"><span data-stu-id="6cac5-123">**Element**</span></span>|<span data-ttu-id="6cac5-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="6cac5-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6cac5-125">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="6cac5-125">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="6cac5-126">現在使用されていない、将来使用するために予約されています。</span><span class="sxs-lookup"><span data-stu-id="6cac5-126">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="6cac5-127">Items</span><span class="sxs-lookup"><span data-stu-id="6cac5-127">Items</span></span>](items.md) <br/> |<span data-ttu-id="6cac5-128">項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6cac5-128">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="6cac5-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="6cac5-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="6cac5-130">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="6cac5-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="6cac5-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="6cac5-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="6cac5-132">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="6cac5-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="6cac5-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="6cac5-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="6cac5-134">要求に関するステータス情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="6cac5-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6cac5-135">親要素</span><span class="sxs-lookup"><span data-stu-id="6cac5-135">Parent elements</span></span>

|<span data-ttu-id="6cac5-136">**要素**</span><span class="sxs-lookup"><span data-stu-id="6cac5-136">**Element**</span></span>|<span data-ttu-id="6cac5-137">**説明**</span><span class="sxs-lookup"><span data-stu-id="6cac5-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6cac5-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="6cac5-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="6cac5-139">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6cac5-139">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6cac5-140">備考</span><span class="sxs-lookup"><span data-stu-id="6cac5-140">Remarks</span></span>

<span data-ttu-id="6cac5-141">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6cac5-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6cac5-142">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6cac5-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6cac5-143">要素情報</span><span class="sxs-lookup"><span data-stu-id="6cac5-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6cac5-144">名前空間</span><span class="sxs-lookup"><span data-stu-id="6cac5-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6cac5-145">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6cac5-145">Schema Name</span></span>  <br/> |<span data-ttu-id="6cac5-146">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="6cac5-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="6cac5-147">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6cac5-147">Validation File</span></span>  <br/> |<span data-ttu-id="6cac5-148">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6cac5-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6cac5-149">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6cac5-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="6cac5-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="6cac5-150">See also</span></span>

- [<span data-ttu-id="6cac5-151">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="6cac5-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

