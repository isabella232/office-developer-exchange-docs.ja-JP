---
title: GetHoldOnMailboxesResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0f7d0d90-d418-4ce9-8cea-afe8f14728c3
description: GetHoldOnMailboxesResponseMessage 要素は、GetHoldOnMailboxes 要求の応答メッセージを指定します。
ms.openlocfilehash: e1c43f75bfa62b20de9248546e71c92ae5998ed9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760750"
---
# <a name="getholdonmailboxesresponsemessage"></a><span data-ttu-id="ee46d-103">GetHoldOnMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ee46d-103">GetHoldOnMailboxesResponseMessage</span></span>

<span data-ttu-id="ee46d-104">**GetHoldOnMailboxesResponseMessage**要素は、 **GetHoldOnMailboxes**要求の応答メッセージを指定します。</span><span class="sxs-lookup"><span data-stu-id="ee46d-104">The **GetHoldOnMailboxesResponseMessage** element specifies the response message for a **GetHoldOnMailboxes** request.</span></span> 
  
```XML
<GetHoldOnMailboxesResponseMessage ResponseClass=" Success | Warning | Error ">
    <MailboxHoldResult/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetHoldOnMailboxesResponseMessage>
```

 <span data-ttu-id="ee46d-105">**GetHoldOnMailboxesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="ee46d-105">**GetHoldOnMailboxesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ee46d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ee46d-106">Attributes and elements</span></span>

<span data-ttu-id="ee46d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ee46d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ee46d-108">属性</span><span class="sxs-lookup"><span data-stu-id="ee46d-108">Attributes</span></span>

|<span data-ttu-id="ee46d-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="ee46d-109">**Attribute**</span></span>|<span data-ttu-id="ee46d-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="ee46d-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ee46d-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="ee46d-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="ee46d-112">応答のクラスを示します。</span><span class="sxs-lookup"><span data-stu-id="ee46d-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="ee46d-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="ee46d-113">ResponseClass</span></span>

|<span data-ttu-id="ee46d-114">**値**</span><span class="sxs-lookup"><span data-stu-id="ee46d-114">**Value**</span></span>|<span data-ttu-id="ee46d-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="ee46d-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ee46d-116">成功</span><span class="sxs-lookup"><span data-stu-id="ee46d-116">Success</span></span>  <br/> |<span data-ttu-id="ee46d-117">成功を示します。</span><span class="sxs-lookup"><span data-stu-id="ee46d-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="ee46d-118">警告</span><span class="sxs-lookup"><span data-stu-id="ee46d-118">Warning</span></span>  <br/> |<span data-ttu-id="ee46d-119">警告を示します。</span><span class="sxs-lookup"><span data-stu-id="ee46d-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="ee46d-120">エラー</span><span class="sxs-lookup"><span data-stu-id="ee46d-120">Error</span></span>  <br/> |<span data-ttu-id="ee46d-121">エラーを示します。</span><span class="sxs-lookup"><span data-stu-id="ee46d-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ee46d-122">子要素</span><span class="sxs-lookup"><span data-stu-id="ee46d-122">Child elements</span></span>

|<span data-ttu-id="ee46d-123">**要素**</span><span class="sxs-lookup"><span data-stu-id="ee46d-123">**Element**</span></span>|<span data-ttu-id="ee46d-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="ee46d-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ee46d-125">MailboxHoldResult</span><span class="sxs-lookup"><span data-stu-id="ee46d-125">MailboxHoldResult</span></span>](mailboxholdresult.md) <br/> |<span data-ttu-id="ee46d-126">**GetHoldOnMailboxes**要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ee46d-126">Contains the result of the **GetHoldOnMailboxes** request.</span></span>  <br/> |
|[<span data-ttu-id="ee46d-127">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="ee46d-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="ee46d-128">現在使用されていない、将来使用するために予約されています。</span><span class="sxs-lookup"><span data-stu-id="ee46d-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="ee46d-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="ee46d-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="ee46d-130">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="ee46d-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="ee46d-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="ee46d-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="ee46d-132">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="ee46d-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="ee46d-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ee46d-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="ee46d-134">要求に関するステータス情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="ee46d-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ee46d-135">親要素</span><span class="sxs-lookup"><span data-stu-id="ee46d-135">Parent elements</span></span>

|<span data-ttu-id="ee46d-136">**要素**</span><span class="sxs-lookup"><span data-stu-id="ee46d-136">**Element**</span></span>|<span data-ttu-id="ee46d-137">**説明**</span><span class="sxs-lookup"><span data-stu-id="ee46d-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ee46d-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ee46d-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="ee46d-139">Exchange Web サービス (EWS) 要求の応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="ee46d-139">Contains the response messages for an Exchange Web Services (EWS) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ee46d-140">備考</span><span class="sxs-lookup"><span data-stu-id="ee46d-140">Remarks</span></span>

<span data-ttu-id="ee46d-141">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="ee46d-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ee46d-142">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ee46d-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ee46d-143">要素情報</span><span class="sxs-lookup"><span data-stu-id="ee46d-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ee46d-144">名前空間</span><span class="sxs-lookup"><span data-stu-id="ee46d-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ee46d-145">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ee46d-145">Schema Name</span></span>  <br/> |<span data-ttu-id="ee46d-146">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="ee46d-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="ee46d-147">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ee46d-147">Validation File</span></span>  <br/> |<span data-ttu-id="ee46d-148">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ee46d-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ee46d-149">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="ee46d-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="ee46d-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="ee46d-150">See also</span></span>



- [<span data-ttu-id="ee46d-151">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="ee46d-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

