---
title: ArchiveItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2ac58d6f-e019-4352-b82f-8ac67a171e63
description: ArchiveItemResponseMessage 要素は、アーカイブアイテム要求への応答メッセージを指定します。
ms.openlocfilehash: 24d09d63cab6805194e35031d8590290573de0a9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463392"
---
# <a name="archiveitemresponsemessage"></a><span data-ttu-id="45e0c-103">ArchiveItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="45e0c-103">ArchiveItemResponseMessage</span></span>

<span data-ttu-id="45e0c-104">**ArchiveItemResponseMessage**要素は、**アーカイブアイテム**要求への応答メッセージを指定します。</span><span class="sxs-lookup"><span data-stu-id="45e0c-104">The **ArchiveItemResponseMessage** element specifies the response message to an **ArchiveItem** request.</span></span> 
  
```XML
<ArchiveItemResponseMessage ResponseClass="">
    <MessageText></MessageText>
    <ResponseCode></ResponseCode>
    <DescriptiveLinkKey></DescriptiveLinkKey>
    <MessageXml></MessageXml>
    <Items></Items>
</ArchiveItemResponseMessage>
```

 <span data-ttu-id="45e0c-105">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="45e0c-105">**ItemInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="45e0c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="45e0c-106">Attributes and elements</span></span>

<span data-ttu-id="45e0c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="45e0c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="45e0c-108">属性</span><span class="sxs-lookup"><span data-stu-id="45e0c-108">Attributes</span></span>

|<span data-ttu-id="45e0c-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="45e0c-109">**Attribute**</span></span>|<span data-ttu-id="45e0c-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="45e0c-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="45e0c-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="45e0c-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="45e0c-112">応答のクラスを示します。</span><span class="sxs-lookup"><span data-stu-id="45e0c-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="45e0c-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="45e0c-113">ResponseClass</span></span>

|<span data-ttu-id="45e0c-114">**値**</span><span class="sxs-lookup"><span data-stu-id="45e0c-114">**Value**</span></span>|<span data-ttu-id="45e0c-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="45e0c-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="45e0c-116">成功</span><span class="sxs-lookup"><span data-stu-id="45e0c-116">Success</span></span>  <br/> |<span data-ttu-id="45e0c-117">成功を示します。</span><span class="sxs-lookup"><span data-stu-id="45e0c-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="45e0c-118">警告</span><span class="sxs-lookup"><span data-stu-id="45e0c-118">Warning</span></span>  <br/> |<span data-ttu-id="45e0c-119">警告を示します。</span><span class="sxs-lookup"><span data-stu-id="45e0c-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="45e0c-120">Error</span><span class="sxs-lookup"><span data-stu-id="45e0c-120">Error</span></span>  <br/> |<span data-ttu-id="45e0c-121">エラーを示します。</span><span class="sxs-lookup"><span data-stu-id="45e0c-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="45e0c-122">子要素</span><span class="sxs-lookup"><span data-stu-id="45e0c-122">Child elements</span></span>

|<span data-ttu-id="45e0c-123">**Element**</span><span class="sxs-lookup"><span data-stu-id="45e0c-123">**Element**</span></span>|<span data-ttu-id="45e0c-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="45e0c-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="45e0c-125">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="45e0c-125">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="45e0c-126">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="45e0c-126">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="45e0c-127">Items</span><span class="sxs-lookup"><span data-stu-id="45e0c-127">Items</span></span>](items.md) <br/> |<span data-ttu-id="45e0c-128">項目の配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="45e0c-128">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="45e0c-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="45e0c-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="45e0c-130">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="45e0c-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="45e0c-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="45e0c-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="45e0c-132">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="45e0c-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="45e0c-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="45e0c-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="45e0c-134">要求に関する状態情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="45e0c-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="45e0c-135">親要素</span><span class="sxs-lookup"><span data-stu-id="45e0c-135">Parent elements</span></span>

|<span data-ttu-id="45e0c-136">**要素**</span><span class="sxs-lookup"><span data-stu-id="45e0c-136">**Element**</span></span>|<span data-ttu-id="45e0c-137">**説明**</span><span class="sxs-lookup"><span data-stu-id="45e0c-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="45e0c-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="45e0c-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="45e0c-139">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="45e0c-139">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="45e0c-140">注釈</span><span class="sxs-lookup"><span data-stu-id="45e0c-140">Remarks</span></span>

<span data-ttu-id="45e0c-141">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="45e0c-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="45e0c-142">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="45e0c-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="45e0c-143">要素の情報</span><span class="sxs-lookup"><span data-stu-id="45e0c-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="45e0c-144">Namespace</span><span class="sxs-lookup"><span data-stu-id="45e0c-144">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="45e0c-145">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="45e0c-145">Schema Name</span></span>  <br/> |<span data-ttu-id="45e0c-146">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="45e0c-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="45e0c-147">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="45e0c-147">Validation File</span></span>  <br/> |<span data-ttu-id="45e0c-148">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="45e0c-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="45e0c-149">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="45e0c-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="45e0c-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="45e0c-150">See also</span></span>

- [<span data-ttu-id="45e0c-151">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="45e0c-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

