---
title: GetSearchableMailboxesResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f45865fd-4626-4d80-84f6-7989339fdd85
description: GetSearchableMailboxesResponseMessage 要素は、GetSearchableMailboxes 要求の応答メッセージを指定します。
ms.openlocfilehash: 2a4d1fe357656fe29d8572e7f32a4bc2e4a6131e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760858"
---
# <a name="getsearchablemailboxesresponsemessage"></a><span data-ttu-id="33148-103">GetSearchableMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="33148-103">GetSearchableMailboxesResponseMessage</span></span>

<span data-ttu-id="33148-104">**GetSearchableMailboxesResponseMessage**要素は、 **GetSearchableMailboxes**要求の応答メッセージを指定します。</span><span class="sxs-lookup"><span data-stu-id="33148-104">The **GetSearchableMailboxesResponseMessage** element specifies the response message for a **GetSearchableMailboxes** request.</span></span> 
  
```XML
<GetSearchableMailboxesResponseMessage ResponseClass=" Success | Warning | Error ">
    <SearchableMailboxes/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetSearchablemailboxesResponseMessage>
```

 <span data-ttu-id="33148-105">**GetSearchableMailboxesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="33148-105">**GetSearchableMailboxesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="33148-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="33148-106">Attributes and elements</span></span>

<span data-ttu-id="33148-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="33148-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="33148-108">属性</span><span class="sxs-lookup"><span data-stu-id="33148-108">Attributes</span></span>

|<span data-ttu-id="33148-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="33148-109">**Attribute**</span></span>|<span data-ttu-id="33148-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="33148-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="33148-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="33148-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="33148-112">応答のクラスを示します。</span><span class="sxs-lookup"><span data-stu-id="33148-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="33148-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="33148-113">ResponseClass</span></span>

|<span data-ttu-id="33148-114">**値**</span><span class="sxs-lookup"><span data-stu-id="33148-114">**Value**</span></span>|<span data-ttu-id="33148-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="33148-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="33148-116">成功</span><span class="sxs-lookup"><span data-stu-id="33148-116">Success</span></span>  <br/> |<span data-ttu-id="33148-117">成功を示します。</span><span class="sxs-lookup"><span data-stu-id="33148-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="33148-118">警告</span><span class="sxs-lookup"><span data-stu-id="33148-118">Warning</span></span>  <br/> |<span data-ttu-id="33148-119">警告を示します。</span><span class="sxs-lookup"><span data-stu-id="33148-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="33148-120">エラー</span><span class="sxs-lookup"><span data-stu-id="33148-120">Error</span></span>  <br/> |<span data-ttu-id="33148-121">エラーを示します。</span><span class="sxs-lookup"><span data-stu-id="33148-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="33148-122">子要素</span><span class="sxs-lookup"><span data-stu-id="33148-122">Child elements</span></span>

|<span data-ttu-id="33148-123">**要素**</span><span class="sxs-lookup"><span data-stu-id="33148-123">**Element**</span></span>|<span data-ttu-id="33148-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="33148-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="33148-125">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="33148-125">SearchableMailboxes</span></span>](searchablemailboxes.md) <br/> |<span data-ttu-id="33148-126">**GetSearchableMailboxes**要求から返されたメールボックスの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="33148-126">Contains an array of the mailboxes returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
|[<span data-ttu-id="33148-127">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="33148-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="33148-128">現在使用されていない、将来使用するために予約されています。</span><span class="sxs-lookup"><span data-stu-id="33148-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="33148-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="33148-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="33148-130">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="33148-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="33148-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="33148-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="33148-132">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="33148-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="33148-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="33148-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="33148-134">要求に関するステータス情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="33148-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="33148-135">親要素</span><span class="sxs-lookup"><span data-stu-id="33148-135">Parent elements</span></span>

|<span data-ttu-id="33148-136">**要素**</span><span class="sxs-lookup"><span data-stu-id="33148-136">**Element**</span></span>|<span data-ttu-id="33148-137">**説明**</span><span class="sxs-lookup"><span data-stu-id="33148-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="33148-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="33148-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="33148-139">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="33148-139">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="33148-140">備考</span><span class="sxs-lookup"><span data-stu-id="33148-140">Remarks</span></span>

<span data-ttu-id="33148-141">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="33148-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="33148-142">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="33148-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="33148-143">要素情報</span><span class="sxs-lookup"><span data-stu-id="33148-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="33148-144">名前空間</span><span class="sxs-lookup"><span data-stu-id="33148-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="33148-145">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="33148-145">Schema Name</span></span>  <br/> |<span data-ttu-id="33148-146">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="33148-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="33148-147">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="33148-147">Validation File</span></span>  <br/> |<span data-ttu-id="33148-148">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="33148-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="33148-149">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="33148-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="33148-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="33148-150">See also</span></span>



- [<span data-ttu-id="33148-151">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="33148-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

