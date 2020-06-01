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
ms.openlocfilehash: 31832c11181bdca482e88419dd46ff1eacf77ea6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462951"
---
# <a name="getholdonmailboxesresponsemessage"></a><span data-ttu-id="aaca6-103">GetHoldOnMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="aaca6-103">GetHoldOnMailboxesResponseMessage</span></span>

<span data-ttu-id="aaca6-104">**GetHoldOnMailboxesResponseMessage**要素は、 **GetHoldOnMailboxes**要求の応答メッセージを指定します。</span><span class="sxs-lookup"><span data-stu-id="aaca6-104">The **GetHoldOnMailboxesResponseMessage** element specifies the response message for a **GetHoldOnMailboxes** request.</span></span> 
  
```XML
<GetHoldOnMailboxesResponseMessage ResponseClass=" Success | Warning | Error ">
    <MailboxHoldResult/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetHoldOnMailboxesResponseMessage>
```

 <span data-ttu-id="aaca6-105">**GetHoldOnMailboxesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="aaca6-105">**GetHoldOnMailboxesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aaca6-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="aaca6-106">Attributes and elements</span></span>

<span data-ttu-id="aaca6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="aaca6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aaca6-108">属性</span><span class="sxs-lookup"><span data-stu-id="aaca6-108">Attributes</span></span>

|<span data-ttu-id="aaca6-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="aaca6-109">**Attribute**</span></span>|<span data-ttu-id="aaca6-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="aaca6-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="aaca6-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="aaca6-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="aaca6-112">応答のクラスを示します。</span><span class="sxs-lookup"><span data-stu-id="aaca6-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="aaca6-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="aaca6-113">ResponseClass</span></span>

|<span data-ttu-id="aaca6-114">**値**</span><span class="sxs-lookup"><span data-stu-id="aaca6-114">**Value**</span></span>|<span data-ttu-id="aaca6-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="aaca6-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="aaca6-116">Success</span><span class="sxs-lookup"><span data-stu-id="aaca6-116">Success</span></span>  <br/> |<span data-ttu-id="aaca6-117">成功を示します。</span><span class="sxs-lookup"><span data-stu-id="aaca6-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="aaca6-118">警告</span><span class="sxs-lookup"><span data-stu-id="aaca6-118">Warning</span></span>  <br/> |<span data-ttu-id="aaca6-119">警告を示します。</span><span class="sxs-lookup"><span data-stu-id="aaca6-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="aaca6-120">Error</span><span class="sxs-lookup"><span data-stu-id="aaca6-120">Error</span></span>  <br/> |<span data-ttu-id="aaca6-121">エラーを示します。</span><span class="sxs-lookup"><span data-stu-id="aaca6-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="aaca6-122">子要素</span><span class="sxs-lookup"><span data-stu-id="aaca6-122">Child elements</span></span>

|<span data-ttu-id="aaca6-123">**Element**</span><span class="sxs-lookup"><span data-stu-id="aaca6-123">**Element**</span></span>|<span data-ttu-id="aaca6-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="aaca6-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aaca6-125">MailboxHoldResult</span><span class="sxs-lookup"><span data-stu-id="aaca6-125">MailboxHoldResult</span></span>](mailboxholdresult.md) <br/> |<span data-ttu-id="aaca6-126">**GetHoldOnMailboxes**要求の結果が含まれます。</span><span class="sxs-lookup"><span data-stu-id="aaca6-126">Contains the result of the **GetHoldOnMailboxes** request.</span></span>  <br/> |
|[<span data-ttu-id="aaca6-127">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="aaca6-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="aaca6-128">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="aaca6-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="aaca6-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="aaca6-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="aaca6-130">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="aaca6-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="aaca6-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="aaca6-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="aaca6-132">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="aaca6-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="aaca6-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="aaca6-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="aaca6-134">要求に関する状態情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="aaca6-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aaca6-135">親要素</span><span class="sxs-lookup"><span data-stu-id="aaca6-135">Parent elements</span></span>

|<span data-ttu-id="aaca6-136">**要素**</span><span class="sxs-lookup"><span data-stu-id="aaca6-136">**Element**</span></span>|<span data-ttu-id="aaca6-137">**説明**</span><span class="sxs-lookup"><span data-stu-id="aaca6-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aaca6-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="aaca6-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="aaca6-139">Exchange Web サービス (EWS) 要求に対する応答メッセージが保存されています。</span><span class="sxs-lookup"><span data-stu-id="aaca6-139">Contains the response messages for an Exchange Web Services (EWS) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="aaca6-140">注釈</span><span class="sxs-lookup"><span data-stu-id="aaca6-140">Remarks</span></span>

<span data-ttu-id="aaca6-141">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="aaca6-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="aaca6-142">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="aaca6-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aaca6-143">要素の情報</span><span class="sxs-lookup"><span data-stu-id="aaca6-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aaca6-144">Namespace</span><span class="sxs-lookup"><span data-stu-id="aaca6-144">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="aaca6-145">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="aaca6-145">Schema Name</span></span>  <br/> |<span data-ttu-id="aaca6-146">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="aaca6-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="aaca6-147">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="aaca6-147">Validation File</span></span>  <br/> |<span data-ttu-id="aaca6-148">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="aaca6-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="aaca6-149">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="aaca6-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="aaca6-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="aaca6-150">See also</span></span>



- [<span data-ttu-id="aaca6-151">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="aaca6-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

