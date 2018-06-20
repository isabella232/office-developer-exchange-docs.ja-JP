---
title: MessageTrackingSearchResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MessageTrackingSearchResult
api_type:
- schema
ms.assetid: 8ea77aa8-b93f-4287-be36-0a9da06e0946
description: MessageTrackingSearchResult 要素には、FindMessageTrackingReportResponse 要素の 1 つのメッセージの結果が含まれています。
ms.openlocfilehash: ad4fb9d9e2266222303bd2015a7afba0bb46721b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832460"
---
# <a name="messagetrackingsearchresult"></a><span data-ttu-id="1394e-103">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="1394e-103">MessageTrackingSearchResult</span></span>

<span data-ttu-id="1394e-104">**MessageTrackingSearchResult**要素には、 [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md)要素の 1 つのメッセージの結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1394e-104">The **MessageTrackingSearchResult** element contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span> 
  
```xml
<MessageTrackingSearchResult>
   <Subject/>
   <Sender/>
   <PurportedSender/>
   <Recipients/>
   <SubmittedTime/>
   <MessageTrackingReportId/>
   <PreviousHopServer/>
   <FirstHopServer/>
   <Properties/>
</MessageTrackingSearchResult>
```

 <span data-ttu-id="1394e-105">**FindMessageTrackingSearchResultType**</span><span class="sxs-lookup"><span data-stu-id="1394e-105">**FindMessageTrackingSearchResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1394e-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="1394e-106">Attributes and elements</span></span>

<span data-ttu-id="1394e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1394e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1394e-108">属性</span><span class="sxs-lookup"><span data-stu-id="1394e-108">Attributes</span></span>

<span data-ttu-id="1394e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1394e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1394e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1394e-110">Child elements</span></span>

|<span data-ttu-id="1394e-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="1394e-111">**Element**</span></span>|<span data-ttu-id="1394e-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="1394e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1394e-113">Subject</span><span class="sxs-lookup"><span data-stu-id="1394e-113">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="1394e-114">電子メール メッセージの件名が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1394e-114">Contains the e-mail message subject.</span></span>  <br/> |
|[<span data-ttu-id="1394e-115">送信者 (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="1394e-115">Sender (EmailAddressType)</span></span>](sender-emailaddresstype.md) <br/> |<span data-ttu-id="1394e-116">電子メール メッセージの送信者のアドレスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="1394e-116">Contains the e-mail message sender's address.</span></span>  <br/> |
|[<span data-ttu-id="1394e-117">PurportedSender</span><span class="sxs-lookup"><span data-stu-id="1394e-117">PurportedSender</span></span>](purportedsender.md) <br/> |<span data-ttu-id="1394e-118">申し立ての送信者の電子メール メッセージの連絡先の情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1394e-118">Contains contact information for the alleged sender of an e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="1394e-119">受信者 (ArrayOfRecipientsType)</span><span class="sxs-lookup"><span data-stu-id="1394e-119">Recipients (ArrayOfRecipientsType)</span></span>](recipients-arrayofrecipientstype.md) <br/> |<span data-ttu-id="1394e-120">このメッセージを受信した電子メール アドレスの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1394e-120">Contains a list of e-mail addresses that received this message.</span></span>  <br/> |
|[<span data-ttu-id="1394e-121">SubmittedTime</span><span class="sxs-lookup"><span data-stu-id="1394e-121">SubmittedTime</span></span>](submittedtime.md) <br/> |<span data-ttu-id="1394e-122">メッセージが送信された時刻が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1394e-122">Contains the time that the message was submitted.</span></span>  <br/> |
|[<span data-ttu-id="1394e-123">MessageTrackingReportId</span><span class="sxs-lookup"><span data-stu-id="1394e-123">MessageTrackingReportId</span></span>](messagetrackingreportid.md) <br/> |<span data-ttu-id="1394e-124">トランスポート データベースのメッセージを識別する内部の ID が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1394e-124">Contains an internal ID that identifies the message in the transport database.</span></span>  <br/> |
|[<span data-ttu-id="1394e-125">PreviousHopServer</span><span class="sxs-lookup"><span data-stu-id="1394e-125">PreviousHopServer</span></span>](previoushopserver.md) <br/> |<span data-ttu-id="1394e-126">以前のメッセージを承諾するフォレスト内のサーバーの名前が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1394e-126">Contains the name of the server in the forest that previously accepted the message.</span></span>  <br/> |
|[<span data-ttu-id="1394e-127">FirstHopServer</span><span class="sxs-lookup"><span data-stu-id="1394e-127">FirstHopServer</span></span>](firsthopserver.md) <br/> |<span data-ttu-id="1394e-128">フォレスト内の最初のメッセージを受け付けでサーバーの名前が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1394e-128">Contains the name of the server in the forest that first accepted the message.</span></span>  <br/> |
|[<span data-ttu-id="1394e-129">プロパティ (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="1394e-129">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="1394e-130">1 つまたは複数の追跡のプロパティの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1394e-130">Contains a list of one or more tracking properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1394e-131">親要素</span><span class="sxs-lookup"><span data-stu-id="1394e-131">Parent elements</span></span>

|<span data-ttu-id="1394e-132">**要素**</span><span class="sxs-lookup"><span data-stu-id="1394e-132">**Element**</span></span>|<span data-ttu-id="1394e-133">**説明**</span><span class="sxs-lookup"><span data-stu-id="1394e-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1394e-134">MessageTrackingSearchResults</span><span class="sxs-lookup"><span data-stu-id="1394e-134">MessageTrackingSearchResults</span></span>](messagetrackingsearchresults.md) <br/> |<span data-ttu-id="1394e-135">検索条件に一致するメッセージの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1394e-135">Contains a list of messages that match the search criteria.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1394e-136">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1394e-136">Text value</span></span>

<span data-ttu-id="1394e-137">なし。</span><span class="sxs-lookup"><span data-stu-id="1394e-137">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1394e-138">備考</span><span class="sxs-lookup"><span data-stu-id="1394e-138">Remarks</span></span>

<span data-ttu-id="1394e-139">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="1394e-139">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1394e-140">要素情報</span><span class="sxs-lookup"><span data-stu-id="1394e-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1394e-141">名前空間</span><span class="sxs-lookup"><span data-stu-id="1394e-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1394e-142">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1394e-142">Schema Name</span></span>  <br/> |<span data-ttu-id="1394e-143">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="1394e-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="1394e-144">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1394e-144">Validation File</span></span>  <br/> |<span data-ttu-id="1394e-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1394e-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1394e-146">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1394e-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="1394e-147">False</span><span class="sxs-lookup"><span data-stu-id="1394e-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1394e-148">関連項目</span><span class="sxs-lookup"><span data-stu-id="1394e-148">See also</span></span>



[<span data-ttu-id="1394e-149">FindMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="1394e-149">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)


- [<span data-ttu-id="1394e-150">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="1394e-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

