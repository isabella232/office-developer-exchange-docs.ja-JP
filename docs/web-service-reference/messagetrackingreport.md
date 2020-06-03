---
title: および search-messagetrackingreport
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
description: MessageTrackingReport 要素には、GetMessageTrackingReport 操作で返される1つのメッセージが含まれています。
ms.openlocfilehash: fc3e56fbb1bee411fa31751f558f520874133076
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463217"
---
# <a name="messagetrackingreport"></a><span data-ttu-id="e7422-103">および search-messagetrackingreport</span><span class="sxs-lookup"><span data-stu-id="e7422-103">MessageTrackingReport</span></span>

<span data-ttu-id="e7422-104">**Messagetrackingreport**要素には、 [getmessagetrackingreport 操作](getmessagetrackingreport-operation.md)で返される1つのメッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e7422-104">The **MessageTrackingReport** element contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>
  
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

 <span data-ttu-id="e7422-105">**MessageTrackingReportType**</span><span class="sxs-lookup"><span data-stu-id="e7422-105">**MessageTrackingReportType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e7422-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e7422-106">Attributes and elements</span></span>

<span data-ttu-id="e7422-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e7422-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e7422-108">属性</span><span class="sxs-lookup"><span data-stu-id="e7422-108">Attributes</span></span>

<span data-ttu-id="e7422-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e7422-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e7422-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e7422-110">Child elements</span></span>

|<span data-ttu-id="e7422-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="e7422-111">**Element**</span></span>|<span data-ttu-id="e7422-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="e7422-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e7422-113">Sender (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="e7422-113">Sender (EmailAddressType)</span></span>](sender-emailaddresstype.md) <br/> |<span data-ttu-id="e7422-114">電子メールメッセージの送信者の連絡先情報が保存されています。</span><span class="sxs-lookup"><span data-stu-id="e7422-114">Contains contact information for the sender of the e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="e7422-115">PurportedSender</span><span class="sxs-lookup"><span data-stu-id="e7422-115">PurportedSender</span></span>](purportedsender.md) <br/> |<span data-ttu-id="e7422-116">電子メールメッセージの申し立て送信者の連絡先情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e7422-116">Contains contact information for the alleged sender of an e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="e7422-117">件名</span><span class="sxs-lookup"><span data-stu-id="e7422-117">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="e7422-118">電子メールメッセージの件名を含みます。</span><span class="sxs-lookup"><span data-stu-id="e7422-118">Contains the subject of the e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="e7422-119">SubmitTime</span><span class="sxs-lookup"><span data-stu-id="e7422-119">SubmitTime</span></span>](submittime.md) <br/> |<span data-ttu-id="e7422-120">電子メールメッセージが送信された時刻を格納します。</span><span class="sxs-lookup"><span data-stu-id="e7422-120">Contains the time of day that the e-mail message was submitted.</span></span>  <br/> |
|[<span data-ttu-id="e7422-121">OriginalRecipients</span><span class="sxs-lookup"><span data-stu-id="e7422-121">OriginalRecipients</span></span>](originalrecipients.md) <br/> |<span data-ttu-id="e7422-122">電子メールメッセージの受信者のリストが保存されています。</span><span class="sxs-lookup"><span data-stu-id="e7422-122">Contains a list of the recipients of the e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="e7422-123">受信者 Trackingevents</span><span class="sxs-lookup"><span data-stu-id="e7422-123">RecipientTrackingEvents</span></span>](recipienttrackingevents.md) <br/> |<span data-ttu-id="e7422-124">受信者の1つまたは複数の追跡イベントのリストを含みます。</span><span class="sxs-lookup"><span data-stu-id="e7422-124">Contains a list of one or more tracking events for the recipients.</span></span>  <br/> |
|[<span data-ttu-id="e7422-125">プロパティ (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="e7422-125">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="e7422-126">1つ以上の追跡プロパティの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e7422-126">Contains a list of one or more tracking properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e7422-127">親要素</span><span class="sxs-lookup"><span data-stu-id="e7422-127">Parent elements</span></span>

|<span data-ttu-id="e7422-128">**要素**</span><span class="sxs-lookup"><span data-stu-id="e7422-128">**Element**</span></span>|<span data-ttu-id="e7422-129">**説明**</span><span class="sxs-lookup"><span data-stu-id="e7422-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e7422-130">GetMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="e7422-130">GetMessageTrackingReportResponse</span></span>](getmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="e7422-131">1つの[Getmessagetrackingreport 操作](getmessagetrackingreport-operation.md)要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e7422-131">Contains the result of a single [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e7422-132">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e7422-132">Text value</span></span>

<span data-ttu-id="e7422-133">なし。</span><span class="sxs-lookup"><span data-stu-id="e7422-133">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e7422-134">注釈</span><span class="sxs-lookup"><span data-stu-id="e7422-134">Remarks</span></span>

<span data-ttu-id="e7422-135">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e7422-135">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e7422-136">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e7422-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e7422-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="e7422-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e7422-138">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e7422-138">Schema Name</span></span>  <br/> |<span data-ttu-id="e7422-139">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="e7422-139">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e7422-140">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e7422-140">Validation File</span></span>  <br/> |<span data-ttu-id="e7422-141">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="e7422-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e7422-142">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e7422-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="e7422-143">正しくない</span><span class="sxs-lookup"><span data-stu-id="e7422-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e7422-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="e7422-144">See also</span></span>



[<span data-ttu-id="e7422-145">FindMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="e7422-145">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)
  
[<span data-ttu-id="e7422-146">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="e7422-146">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="e7422-147">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="e7422-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
  
- [<span data-ttu-id="e7422-148">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="e7422-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

