---
title: FindMailboxStatisticsByKeywordsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d3835800-8887-43db-9a8a-fe3cfea7a863
description: FindMailboxStatisticsByKeywordsResponseMessage 要素は、FindMailboxStatisticsByKeywords 要求の応答メッセージを指定します。
ms.openlocfilehash: 9479252ed53335d07a6402707bc69e5eaadfa7c8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760524"
---
# <a name="findmailboxstatisticsbykeywordsresponsemessage"></a><span data-ttu-id="dcd3b-103">FindMailboxStatisticsByKeywordsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="dcd3b-103">FindMailboxStatisticsByKeywordsResponseMessage</span></span>

<span data-ttu-id="dcd3b-104">**FindMailboxStatisticsByKeywordsResponseMessage**要素は、 **FindMailboxStatisticsByKeywords**要求の応答メッセージを指定します。</span><span class="sxs-lookup"><span data-stu-id="dcd3b-104">The **FindMailboxStatisticsByKeywordsResponseMessage** element specifies the response message for a **FindMailboxStatisticsByKeywords** request.</span></span> 
  
```XML
<FindMailboxStatisticsByKeywordsResponseMessage ResponseClass=" Success | Warning | Error ">
    <MailboxStatisticsSearchResult/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</FindMailboxStatisticsByKeywordsResponseMessage>
```

 <span data-ttu-id="dcd3b-105">**FindMailboxStatisticsByKeywordsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="dcd3b-105">**FindMailboxStatisticsByKeywordsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dcd3b-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="dcd3b-106">Attributes and elements</span></span>

<span data-ttu-id="dcd3b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="dcd3b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dcd3b-108">属性</span><span class="sxs-lookup"><span data-stu-id="dcd3b-108">Attributes</span></span>

|<span data-ttu-id="dcd3b-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="dcd3b-109">**Attribute**</span></span>|<span data-ttu-id="dcd3b-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="dcd3b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="dcd3b-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="dcd3b-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="dcd3b-112">応答クラスを指定します。</span><span class="sxs-lookup"><span data-stu-id="dcd3b-112">Specifies the response class.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="dcd3b-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="dcd3b-113">ResponseClass</span></span>

|<span data-ttu-id="dcd3b-114">**値**</span><span class="sxs-lookup"><span data-stu-id="dcd3b-114">**Value**</span></span>|<span data-ttu-id="dcd3b-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="dcd3b-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="dcd3b-116">成功</span><span class="sxs-lookup"><span data-stu-id="dcd3b-116">Success</span></span>  <br/> |<span data-ttu-id="dcd3b-117">成功を示します。</span><span class="sxs-lookup"><span data-stu-id="dcd3b-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="dcd3b-118">警告</span><span class="sxs-lookup"><span data-stu-id="dcd3b-118">Warning</span></span>  <br/> |<span data-ttu-id="dcd3b-119">警告を示します。</span><span class="sxs-lookup"><span data-stu-id="dcd3b-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="dcd3b-120">エラー</span><span class="sxs-lookup"><span data-stu-id="dcd3b-120">Error</span></span>  <br/> |<span data-ttu-id="dcd3b-121">エラーを示します。</span><span class="sxs-lookup"><span data-stu-id="dcd3b-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="dcd3b-122">子要素</span><span class="sxs-lookup"><span data-stu-id="dcd3b-122">Child elements</span></span>

|<span data-ttu-id="dcd3b-123">**要素**</span><span class="sxs-lookup"><span data-stu-id="dcd3b-123">**Element**</span></span>|<span data-ttu-id="dcd3b-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="dcd3b-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dcd3b-125">MailboxStatisticsSearchResult</span><span class="sxs-lookup"><span data-stu-id="dcd3b-125">MailboxStatisticsSearchResult</span></span>](mailboxstatisticssearchresult.md) <br/> |<span data-ttu-id="dcd3b-126">メールボックス検索の結果を指定します。</span><span class="sxs-lookup"><span data-stu-id="dcd3b-126">Specifies the result of a mailbox search.</span></span>  <br/> |
|[<span data-ttu-id="dcd3b-127">MessageText</span><span class="sxs-lookup"><span data-stu-id="dcd3b-127">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="dcd3b-128">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="dcd3b-128">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="dcd3b-129">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="dcd3b-129">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="dcd3b-130">要求に関するステータス情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="dcd3b-130">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="dcd3b-131">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="dcd3b-131">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="dcd3b-132">現在使用されていない、将来使用するために予約されています。</span><span class="sxs-lookup"><span data-stu-id="dcd3b-132">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="dcd3b-133">MessageXml</span><span class="sxs-lookup"><span data-stu-id="dcd3b-133">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="dcd3b-134">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="dcd3b-134">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dcd3b-135">親要素</span><span class="sxs-lookup"><span data-stu-id="dcd3b-135">Parent elements</span></span>

|<span data-ttu-id="dcd3b-136">**要素**</span><span class="sxs-lookup"><span data-stu-id="dcd3b-136">**Element**</span></span>|<span data-ttu-id="dcd3b-137">**説明**</span><span class="sxs-lookup"><span data-stu-id="dcd3b-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dcd3b-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="dcd3b-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="dcd3b-139">応答メッセージの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="dcd3b-139">Specifies an array of response messages.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dcd3b-140">備考</span><span class="sxs-lookup"><span data-stu-id="dcd3b-140">Remarks</span></span>

<span data-ttu-id="dcd3b-141">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="dcd3b-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="dcd3b-142">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="dcd3b-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dcd3b-143">要素情報</span><span class="sxs-lookup"><span data-stu-id="dcd3b-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dcd3b-144">名前空間</span><span class="sxs-lookup"><span data-stu-id="dcd3b-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="dcd3b-145">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="dcd3b-145">Schema Name</span></span>  <br/> |<span data-ttu-id="dcd3b-146">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="dcd3b-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="dcd3b-147">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="dcd3b-147">Validation File</span></span>  <br/> |<span data-ttu-id="dcd3b-148">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="dcd3b-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dcd3b-149">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="dcd3b-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="dcd3b-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="dcd3b-150">See also</span></span>



- [<span data-ttu-id="dcd3b-151">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="dcd3b-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

