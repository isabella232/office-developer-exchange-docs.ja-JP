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
description: MessageTrackingSearchResult 要素には、FindMessageTrackingReportResponse 要素の単一のメッセージの結果が含まれています。
ms.openlocfilehash: 27e70cd9e11b480ab6bbb9b28275f142da7c76ac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466683"
---
# <a name="messagetrackingsearchresult"></a><span data-ttu-id="d6f77-103">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="d6f77-103">MessageTrackingSearchResult</span></span>

<span data-ttu-id="d6f77-104">**MessageTrackingSearchResult**要素には、 [Findmessagetrackingreportresponse](findmessagetrackingreportresponse.md)要素の単一のメッセージの結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d6f77-104">The **MessageTrackingSearchResult** element contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span> 
  
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

 <span data-ttu-id="d6f77-105">**FindMessageTrackingSearchResultType**</span><span class="sxs-lookup"><span data-stu-id="d6f77-105">**FindMessageTrackingSearchResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d6f77-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d6f77-106">Attributes and elements</span></span>

<span data-ttu-id="d6f77-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d6f77-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d6f77-108">属性</span><span class="sxs-lookup"><span data-stu-id="d6f77-108">Attributes</span></span>

<span data-ttu-id="d6f77-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d6f77-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d6f77-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d6f77-110">Child elements</span></span>

|<span data-ttu-id="d6f77-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="d6f77-111">**Element**</span></span>|<span data-ttu-id="d6f77-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d6f77-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d6f77-113">[[件名]](subject.md)</span><span class="sxs-lookup"><span data-stu-id="d6f77-113">[Subject](subject.md)</span></span> <br/> |<span data-ttu-id="d6f77-114">電子メールメッセージの件名を含みます。</span><span class="sxs-lookup"><span data-stu-id="d6f77-114">Contains the e-mail message subject.</span></span>  <br/> |
|[<span data-ttu-id="d6f77-115">Sender (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="d6f77-115">Sender (EmailAddressType)</span></span>](sender-emailaddresstype.md) <br/> |<span data-ttu-id="d6f77-116">電子メールメッセージの送信者のアドレスを含みます。</span><span class="sxs-lookup"><span data-stu-id="d6f77-116">Contains the e-mail message sender's address.</span></span>  <br/> |
|[<span data-ttu-id="d6f77-117">PurportedSender</span><span class="sxs-lookup"><span data-stu-id="d6f77-117">PurportedSender</span></span>](purportedsender.md) <br/> |<span data-ttu-id="d6f77-118">電子メールメッセージの申し立て送信者の連絡先情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d6f77-118">Contains contact information for the alleged sender of an e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="d6f77-119">受信者 (Arrayof受信者 Stype)</span><span class="sxs-lookup"><span data-stu-id="d6f77-119">Recipients (ArrayOfRecipientsType)</span></span>](recipients-arrayofrecipientstype.md) <br/> |<span data-ttu-id="d6f77-120">このメッセージを受信した電子メールアドレスの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d6f77-120">Contains a list of e-mail addresses that received this message.</span></span>  <br/> |
|[<span data-ttu-id="d6f77-121">SubmittedTime</span><span class="sxs-lookup"><span data-stu-id="d6f77-121">SubmittedTime</span></span>](submittedtime.md) <br/> |<span data-ttu-id="d6f77-122">メッセージが送信された日時が含まれます。</span><span class="sxs-lookup"><span data-stu-id="d6f77-122">Contains the time that the message was submitted.</span></span>  <br/> |
|[<span data-ttu-id="d6f77-123">MessageTrackingReportId</span><span class="sxs-lookup"><span data-stu-id="d6f77-123">MessageTrackingReportId</span></span>](messagetrackingreportid.md) <br/> |<span data-ttu-id="d6f77-124">トランスポートデータベース内のメッセージを識別する内部 ID を格納します。</span><span class="sxs-lookup"><span data-stu-id="d6f77-124">Contains an internal ID that identifies the message in the transport database.</span></span>  <br/> |
|[<span data-ttu-id="d6f77-125">PreviousHopServer</span><span class="sxs-lookup"><span data-stu-id="d6f77-125">PreviousHopServer</span></span>](previoushopserver.md) <br/> |<span data-ttu-id="d6f77-126">以前にメッセージを受諾したフォレスト内のサーバーの名前が含まれます。</span><span class="sxs-lookup"><span data-stu-id="d6f77-126">Contains the name of the server in the forest that previously accepted the message.</span></span>  <br/> |
|[<span data-ttu-id="d6f77-127">FirstHopServer</span><span class="sxs-lookup"><span data-stu-id="d6f77-127">FirstHopServer</span></span>](firsthopserver.md) <br/> |<span data-ttu-id="d6f77-128">最初にメッセージを受け入れたフォレスト内のサーバーの名前が含まれます。</span><span class="sxs-lookup"><span data-stu-id="d6f77-128">Contains the name of the server in the forest that first accepted the message.</span></span>  <br/> |
|[<span data-ttu-id="d6f77-129">プロパティ (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="d6f77-129">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="d6f77-130">1つ以上の追跡プロパティの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d6f77-130">Contains a list of one or more tracking properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d6f77-131">親要素</span><span class="sxs-lookup"><span data-stu-id="d6f77-131">Parent elements</span></span>

|<span data-ttu-id="d6f77-132">**要素**</span><span class="sxs-lookup"><span data-stu-id="d6f77-132">**Element**</span></span>|<span data-ttu-id="d6f77-133">**説明**</span><span class="sxs-lookup"><span data-stu-id="d6f77-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d6f77-134">MessageTrackingSearchResults</span><span class="sxs-lookup"><span data-stu-id="d6f77-134">MessageTrackingSearchResults</span></span>](messagetrackingsearchresults.md) <br/> |<span data-ttu-id="d6f77-135">検索条件に一致するメッセージの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d6f77-135">Contains a list of messages that match the search criteria.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d6f77-136">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d6f77-136">Text value</span></span>

<span data-ttu-id="d6f77-137">なし。</span><span class="sxs-lookup"><span data-stu-id="d6f77-137">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d6f77-138">注釈</span><span class="sxs-lookup"><span data-stu-id="d6f77-138">Remarks</span></span>

<span data-ttu-id="d6f77-139">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d6f77-139">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d6f77-140">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d6f77-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d6f77-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="d6f77-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d6f77-142">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d6f77-142">Schema Name</span></span>  <br/> |<span data-ttu-id="d6f77-143">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d6f77-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="d6f77-144">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d6f77-144">Validation File</span></span>  <br/> |<span data-ttu-id="d6f77-145">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d6f77-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d6f77-146">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d6f77-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="d6f77-147">正しくない</span><span class="sxs-lookup"><span data-stu-id="d6f77-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d6f77-148">関連項目</span><span class="sxs-lookup"><span data-stu-id="d6f77-148">See also</span></span>



[<span data-ttu-id="d6f77-149">FindMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="d6f77-149">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)


- [<span data-ttu-id="d6f77-150">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d6f77-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

