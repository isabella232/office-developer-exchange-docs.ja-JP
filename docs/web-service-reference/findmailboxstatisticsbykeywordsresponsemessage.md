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
ms.openlocfilehash: 704eebbf82db2871ab36be8e5b30c88c6959baa5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44525977"
---
# <a name="findmailboxstatisticsbykeywordsresponsemessage"></a><span data-ttu-id="933e5-103">FindMailboxStatisticsByKeywordsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="933e5-103">FindMailboxStatisticsByKeywordsResponseMessage</span></span>

<span data-ttu-id="933e5-104">**FindMailboxStatisticsByKeywordsResponseMessage**要素は、 **FindMailboxStatisticsByKeywords**要求の応答メッセージを指定します。</span><span class="sxs-lookup"><span data-stu-id="933e5-104">The **FindMailboxStatisticsByKeywordsResponseMessage** element specifies the response message for a **FindMailboxStatisticsByKeywords** request.</span></span> 
  
```XML
<FindMailboxStatisticsByKeywordsResponseMessage ResponseClass=" Success | Warning | Error ">
    <MailboxStatisticsSearchResult/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</FindMailboxStatisticsByKeywordsResponseMessage>
```

 <span data-ttu-id="933e5-105">**FindMailboxStatisticsByKeywordsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="933e5-105">**FindMailboxStatisticsByKeywordsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="933e5-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="933e5-106">Attributes and elements</span></span>

<span data-ttu-id="933e5-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="933e5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="933e5-108">属性</span><span class="sxs-lookup"><span data-stu-id="933e5-108">Attributes</span></span>

|<span data-ttu-id="933e5-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="933e5-109">**Attribute**</span></span>|<span data-ttu-id="933e5-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="933e5-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="933e5-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="933e5-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="933e5-112">Response クラスを指定します。</span><span class="sxs-lookup"><span data-stu-id="933e5-112">Specifies the response class.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="933e5-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="933e5-113">ResponseClass</span></span>

|<span data-ttu-id="933e5-114">**値**</span><span class="sxs-lookup"><span data-stu-id="933e5-114">**Value**</span></span>|<span data-ttu-id="933e5-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="933e5-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="933e5-116">成功</span><span class="sxs-lookup"><span data-stu-id="933e5-116">Success</span></span>  <br/> |<span data-ttu-id="933e5-117">成功を示します。</span><span class="sxs-lookup"><span data-stu-id="933e5-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="933e5-118">警告</span><span class="sxs-lookup"><span data-stu-id="933e5-118">Warning</span></span>  <br/> |<span data-ttu-id="933e5-119">警告を示します。</span><span class="sxs-lookup"><span data-stu-id="933e5-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="933e5-120">Error</span><span class="sxs-lookup"><span data-stu-id="933e5-120">Error</span></span>  <br/> |<span data-ttu-id="933e5-121">エラーを示します。</span><span class="sxs-lookup"><span data-stu-id="933e5-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="933e5-122">子要素</span><span class="sxs-lookup"><span data-stu-id="933e5-122">Child elements</span></span>

|<span data-ttu-id="933e5-123">**Element**</span><span class="sxs-lookup"><span data-stu-id="933e5-123">**Element**</span></span>|<span data-ttu-id="933e5-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="933e5-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="933e5-125">MailboxStatisticsSearchResult</span><span class="sxs-lookup"><span data-stu-id="933e5-125">MailboxStatisticsSearchResult</span></span>](mailboxstatisticssearchresult.md) <br/> |<span data-ttu-id="933e5-126">メールボックス検索の結果を指定します。</span><span class="sxs-lookup"><span data-stu-id="933e5-126">Specifies the result of a mailbox search.</span></span>  <br/> |
|[<span data-ttu-id="933e5-127">MessageText</span><span class="sxs-lookup"><span data-stu-id="933e5-127">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="933e5-128">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="933e5-128">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="933e5-129">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="933e5-129">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="933e5-130">要求に関する状態情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="933e5-130">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="933e5-131">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="933e5-131">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="933e5-132">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="933e5-132">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="933e5-133">MessageXml</span><span class="sxs-lookup"><span data-stu-id="933e5-133">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="933e5-134">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="933e5-134">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="933e5-135">親要素</span><span class="sxs-lookup"><span data-stu-id="933e5-135">Parent elements</span></span>

|<span data-ttu-id="933e5-136">**要素**</span><span class="sxs-lookup"><span data-stu-id="933e5-136">**Element**</span></span>|<span data-ttu-id="933e5-137">**説明**</span><span class="sxs-lookup"><span data-stu-id="933e5-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="933e5-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="933e5-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="933e5-139">応答メッセージの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="933e5-139">Specifies an array of response messages.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="933e5-140">注釈</span><span class="sxs-lookup"><span data-stu-id="933e5-140">Remarks</span></span>

<span data-ttu-id="933e5-141">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="933e5-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="933e5-142">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="933e5-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="933e5-143">要素の情報</span><span class="sxs-lookup"><span data-stu-id="933e5-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="933e5-144">Namespace</span><span class="sxs-lookup"><span data-stu-id="933e5-144">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="933e5-145">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="933e5-145">Schema Name</span></span>  <br/> |<span data-ttu-id="933e5-146">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="933e5-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="933e5-147">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="933e5-147">Validation File</span></span>  <br/> |<span data-ttu-id="933e5-148">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="933e5-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="933e5-149">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="933e5-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="933e5-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="933e5-150">See also</span></span>



- [<span data-ttu-id="933e5-151">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="933e5-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

