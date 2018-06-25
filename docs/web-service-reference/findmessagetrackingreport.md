---
title: FindMessageTrackingReport
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindMessageTrackingReport
api_type:
- schema
ms.assetid: 7ca6e2f7-aae1-4920-b839-73513ba8d4d8
description: FindMessageTrackingReport 要素は、検索するメッセージの種類の条件を指定します。
ms.openlocfilehash: 77545121aa056992248c045af3f3d36566678b94
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760526"
---
# <a name="findmessagetrackingreport"></a><span data-ttu-id="128f4-103">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="128f4-103">FindMessageTrackingReport</span></span>

<span data-ttu-id="128f4-104">**FindMessageTrackingReport**要素は、検索するメッセージの種類の条件を指定します。</span><span class="sxs-lookup"><span data-stu-id="128f4-104">The **FindMessageTrackingReport** element specifies criteria for the types of messages to find.</span></span> 
  
```xml
<FindMessageTrackingReport>
   <Scope/>
   <Domain/>
   <Sender/>
   <PurportedSender/>
   <Recipient/>
   <Subject/>
   <StartDateTime/>
   <EndDateTime/>
   <MessageId/>
   <FederatedDeliveryMailbox/>
   <DiagnosticsLevel/>
   <ServerHint/>
   <Properties/>
</FindMessageTrackingReport>
```

 <span data-ttu-id="128f4-105">**FindMessageTrackingReportRequestType**</span><span class="sxs-lookup"><span data-stu-id="128f4-105">**FindMessageTrackingReportRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="128f4-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="128f4-106">Attributes and elements</span></span>

<span data-ttu-id="128f4-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="128f4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="128f4-108">属性</span><span class="sxs-lookup"><span data-stu-id="128f4-108">Attributes</span></span>

<span data-ttu-id="128f4-109">なし。</span><span class="sxs-lookup"><span data-stu-id="128f4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="128f4-110">子要素</span><span class="sxs-lookup"><span data-stu-id="128f4-110">Child elements</span></span>

|<span data-ttu-id="128f4-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="128f4-111">**Element**</span></span>|<span data-ttu-id="128f4-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="128f4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="128f4-113">スコープ (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="128f4-113">Scope (NonEmptyStringType)</span></span>](scope-nonemptystringtype.md) <br/> |<span data-ttu-id="128f4-114">どの広範なメッセージのレポートを追跡する必要がありますを表します。</span><span class="sxs-lookup"><span data-stu-id="128f4-114">Represents how extensive the message tracking report should be.</span></span>  <br/> |
|[<span data-ttu-id="128f4-115">ドメイン (メッセージの追跡)</span><span class="sxs-lookup"><span data-stu-id="128f4-115">Domain (Message Tracking)</span></span>](domain-message-tracking.md) <br/> |<span data-ttu-id="128f4-116">メッセージ追跡が実行されるドメインの名前が含まれています。</span><span class="sxs-lookup"><span data-stu-id="128f4-116">Contains the name of the domain where the message tracking is executed.</span></span>  <br/> |
|[<span data-ttu-id="128f4-117">送信者 (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="128f4-117">Sender (EmailAddressType)</span></span>](sender-emailaddresstype.md) <br/> |<span data-ttu-id="128f4-118">電子メール メッセージの送信者の連絡先の情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="128f4-118">Contains contact information for the sender of the e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="128f4-119">PurportedSender</span><span class="sxs-lookup"><span data-stu-id="128f4-119">PurportedSender</span></span>](purportedsender.md) <br/> |<span data-ttu-id="128f4-120">申し立ての送信者の電子メール メッセージの連絡先の情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="128f4-120">Contains contact information for the alleged sender of an e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="128f4-121">Recipient</span><span class="sxs-lookup"><span data-stu-id="128f4-121">Recipient</span></span>](recipient.md) <br/> |<span data-ttu-id="128f4-122">メッセージの受信者の電子メール アドレスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="128f4-122">Contains the e-mail address for the recipient of the message.</span></span>  <br/> |
|[<span data-ttu-id="128f4-123">Subject</span><span class="sxs-lookup"><span data-stu-id="128f4-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="128f4-124">電子メール メッセージの件名が含まれています。</span><span class="sxs-lookup"><span data-stu-id="128f4-124">Contains the subject of the e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="128f4-125">StartDateTime</span><span class="sxs-lookup"><span data-stu-id="128f4-125">StartDateTime</span></span>](startdatetime.md) <br/> |<span data-ttu-id="128f4-126">開始の日付と時刻の検索が含まれています。</span><span class="sxs-lookup"><span data-stu-id="128f4-126">Contains the starting date and time for the search.</span></span>  <br/> |
|[<span data-ttu-id="128f4-127">EndDateTime</span><span class="sxs-lookup"><span data-stu-id="128f4-127">EndDateTime</span></span>](enddatetime.md) <br/> |<span data-ttu-id="128f4-128">終了の日付と時刻の検索が含まれています。</span><span class="sxs-lookup"><span data-stu-id="128f4-128">Contains the ending date and time for the search.</span></span>  <br/> |
|[<span data-ttu-id="128f4-129">メッセージ Id</span><span class="sxs-lookup"><span data-stu-id="128f4-129">MessageId</span></span>](messageid.md) <br/> |<span data-ttu-id="128f4-130">検索対象のメッセージの識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="128f4-130">Contains the message identifier for the search.</span></span>  <br/> |
|[<span data-ttu-id="128f4-131">FederatedDeliveryMailbox</span><span class="sxs-lookup"><span data-stu-id="128f4-131">FederatedDeliveryMailbox</span></span>](federateddeliverymailbox.md) <br/> |<span data-ttu-id="128f4-132">設置型の間のメッセージが送信されたメールボックスの名前が含まれています。</span><span class="sxs-lookup"><span data-stu-id="128f4-132">Contains the name of the mailbox where the cross-premise message was sent.</span></span>  <br/> |
|[<span data-ttu-id="128f4-133">DiagnosticsLevel</span><span class="sxs-lookup"><span data-stu-id="128f4-133">DiagnosticsLevel</span></span>](diagnosticslevel.md) <br/> |<span data-ttu-id="128f4-134">診断レポートの詳細のレベルを表します。</span><span class="sxs-lookup"><span data-stu-id="128f4-134">Represents the level of detail for diagnostic reports.</span></span>  <br/> |
|[<span data-ttu-id="128f4-135">ServerHint</span><span class="sxs-lookup"><span data-stu-id="128f4-135">ServerHint</span></span>](serverhint.md) <br/> |<span data-ttu-id="128f4-136">リモート ・ サイトまたはフォレスト内のメッセージを追跡するための開始点を表します。</span><span class="sxs-lookup"><span data-stu-id="128f4-136">Represents the starting point for tracking a message in a remote site or forest.</span></span>  <br/> |
|[<span data-ttu-id="128f4-137">プロパティ (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="128f4-137">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="128f4-138">1 つまたは複数の追跡のプロパティの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="128f4-138">Contains a list of one or more tracking properties.</span></span> <span data-ttu-id="128f4-139">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="128f4-139">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="128f4-140">親要素</span><span class="sxs-lookup"><span data-stu-id="128f4-140">Parent elements</span></span>

<span data-ttu-id="128f4-141">なし。</span><span class="sxs-lookup"><span data-stu-id="128f4-141">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="128f4-142">テキスト値</span><span class="sxs-lookup"><span data-stu-id="128f4-142">Text value</span></span>

<span data-ttu-id="128f4-143">なし。</span><span class="sxs-lookup"><span data-stu-id="128f4-143">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="128f4-144">備考</span><span class="sxs-lookup"><span data-stu-id="128f4-144">Remarks</span></span>

<span data-ttu-id="128f4-145">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="128f4-145">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="128f4-146">要素情報</span><span class="sxs-lookup"><span data-stu-id="128f4-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="128f4-147">名前空間</span><span class="sxs-lookup"><span data-stu-id="128f4-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="128f4-148">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="128f4-148">Schema Name</span></span>  <br/> |<span data-ttu-id="128f4-149">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="128f4-149">Messages schema</span></span>  <br/> |
|<span data-ttu-id="128f4-150">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="128f4-150">Validation File</span></span>  <br/> |<span data-ttu-id="128f4-151">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="128f4-151">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="128f4-152">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="128f4-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="128f4-153">False</span><span class="sxs-lookup"><span data-stu-id="128f4-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="128f4-154">関連項目</span><span class="sxs-lookup"><span data-stu-id="128f4-154">See also</span></span>



[<span data-ttu-id="128f4-155">FindMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="128f4-155">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)


- [<span data-ttu-id="128f4-156">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="128f4-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

