---
title: MessageTrackingReport
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MessageTrackingReport
api_type:
- schema
ms.assetid: 2740bcf6-f86d-4756-a0f2-24ed6e9b75f7
description: MessageTrackingReport 要素には、GetMessageTrackingReport の操作で返される 1 つのメッセージが含まれています。
ms.openlocfilehash: d01e0fbf099d096c7f255a8e94070e330577e6ca
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832457"
---
# <a name="messagetrackingreport"></a><span data-ttu-id="93260-103">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="93260-103">MessageTrackingReport</span></span>

<span data-ttu-id="93260-104">**MessageTrackingReport**要素には、 [GetMessageTrackingReport の操作](getmessagetrackingreport-operation.md)で返される 1 つのメッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="93260-104">The **MessageTrackingReport** element contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>
  
```XML
<MessageTrackingReport>
   <Sender/>
   <PurportedSender/>
   <Subject/>
   <SubmitTime/>
   <OriginalRecipients/>
   <RecipientTrackingEvents/>
   <Properties/>
</MessageTrackingReport>
```

 <span data-ttu-id="93260-105">**MessageTrackingReportType**</span><span class="sxs-lookup"><span data-stu-id="93260-105">**MessageTrackingReportType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="93260-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="93260-106">Attributes and elements</span></span>

<span data-ttu-id="93260-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="93260-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="93260-108">属性</span><span class="sxs-lookup"><span data-stu-id="93260-108">Attributes</span></span>

<span data-ttu-id="93260-109">なし。</span><span class="sxs-lookup"><span data-stu-id="93260-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="93260-110">子要素</span><span class="sxs-lookup"><span data-stu-id="93260-110">Child elements</span></span>

|<span data-ttu-id="93260-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="93260-111">**Element**</span></span>|<span data-ttu-id="93260-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="93260-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93260-113">送信者 (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="93260-113">Sender (EmailAddressType)</span></span>](sender-emailaddresstype.md) <br/> |<span data-ttu-id="93260-114">電子メール メッセージの送信者の連絡先の情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="93260-114">Contains contact information for the sender of the e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="93260-115">PurportedSender</span><span class="sxs-lookup"><span data-stu-id="93260-115">PurportedSender</span></span>](purportedsender.md) <br/> |<span data-ttu-id="93260-116">申し立ての送信者の電子メール メッセージの連絡先の情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="93260-116">Contains contact information for the alleged sender of an e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="93260-117">Subject</span><span class="sxs-lookup"><span data-stu-id="93260-117">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="93260-118">電子メール メッセージの件名が含まれています。</span><span class="sxs-lookup"><span data-stu-id="93260-118">Contains the subject of the e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="93260-119">SubmitTime</span><span class="sxs-lookup"><span data-stu-id="93260-119">SubmitTime</span></span>](submittime.md) <br/> |<span data-ttu-id="93260-120">電子メール メッセージが送信された時刻が含まれています。</span><span class="sxs-lookup"><span data-stu-id="93260-120">Contains the time of day that the e-mail message was submitted.</span></span>  <br/> |
|[<span data-ttu-id="93260-121">OriginalRecipients</span><span class="sxs-lookup"><span data-stu-id="93260-121">OriginalRecipients</span></span>](originalrecipients.md) <br/> |<span data-ttu-id="93260-122">電子メール メッセージの受信者の一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="93260-122">Contains a list of the recipients of the e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="93260-123">RecipientTrackingEvents</span><span class="sxs-lookup"><span data-stu-id="93260-123">RecipientTrackingEvents</span></span>](recipienttrackingevents.md) <br/> |<span data-ttu-id="93260-124">受信者の 1 つまたは複数の追跡イベントのリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="93260-124">Contains a list of one or more tracking events for the recipients.</span></span>  <br/> |
|[<span data-ttu-id="93260-125">プロパティ (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="93260-125">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="93260-126">1 つまたは複数の追跡のプロパティの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="93260-126">Contains a list of one or more tracking properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="93260-127">親要素</span><span class="sxs-lookup"><span data-stu-id="93260-127">Parent elements</span></span>

|<span data-ttu-id="93260-128">**要素**</span><span class="sxs-lookup"><span data-stu-id="93260-128">**Element**</span></span>|<span data-ttu-id="93260-129">**説明**</span><span class="sxs-lookup"><span data-stu-id="93260-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93260-130">GetMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="93260-130">GetMessageTrackingReportResponse</span></span>](getmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="93260-131">1 つの結果が含まれています[GetMessageTrackingReport の操作](getmessagetrackingreport-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="93260-131">Contains the result of a single [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="93260-132">テキスト値</span><span class="sxs-lookup"><span data-stu-id="93260-132">Text value</span></span>

<span data-ttu-id="93260-133">なし。</span><span class="sxs-lookup"><span data-stu-id="93260-133">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="93260-134">備考</span><span class="sxs-lookup"><span data-stu-id="93260-134">Remarks</span></span>

<span data-ttu-id="93260-135">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="93260-135">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="93260-136">要素情報</span><span class="sxs-lookup"><span data-stu-id="93260-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="93260-137">名前空間</span><span class="sxs-lookup"><span data-stu-id="93260-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="93260-138">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="93260-138">Schema Name</span></span>  <br/> |<span data-ttu-id="93260-139">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="93260-139">Messages schema</span></span>  <br/> |
|<span data-ttu-id="93260-140">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="93260-140">Validation File</span></span>  <br/> |<span data-ttu-id="93260-141">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="93260-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="93260-142">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="93260-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="93260-143">False</span><span class="sxs-lookup"><span data-stu-id="93260-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="93260-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="93260-144">See also</span></span>



[<span data-ttu-id="93260-145">FindMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="93260-145">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)
  
[<span data-ttu-id="93260-146">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="93260-146">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="93260-147">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="93260-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
  
- [<span data-ttu-id="93260-148">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="93260-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

