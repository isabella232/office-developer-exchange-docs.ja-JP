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
description: FindMessageTrackingReport 要素は、検索するメッセージの種類に関する条件を指定します。
ms.openlocfilehash: d30e5391bb4305cae0004a9788df971a57297cae
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462937"
---
# <a name="findmessagetrackingreport"></a><span data-ttu-id="7098b-103">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="7098b-103">FindMessageTrackingReport</span></span>

<span data-ttu-id="7098b-104">**Findmessagetrackingreport**要素は、検索するメッセージの種類に関する条件を指定します。</span><span class="sxs-lookup"><span data-stu-id="7098b-104">The **FindMessageTrackingReport** element specifies criteria for the types of messages to find.</span></span> 
  
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

 <span data-ttu-id="7098b-105">**FindMessageTrackingReportRequestType**</span><span class="sxs-lookup"><span data-stu-id="7098b-105">**FindMessageTrackingReportRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7098b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7098b-106">Attributes and elements</span></span>

<span data-ttu-id="7098b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7098b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7098b-108">属性</span><span class="sxs-lookup"><span data-stu-id="7098b-108">Attributes</span></span>

<span data-ttu-id="7098b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7098b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7098b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7098b-110">Child elements</span></span>

|<span data-ttu-id="7098b-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="7098b-111">**Element**</span></span>|<span data-ttu-id="7098b-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="7098b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7098b-113">範囲 (非 Emptystringtype)</span><span class="sxs-lookup"><span data-stu-id="7098b-113">Scope (NonEmptyStringType)</span></span>](scope-nonemptystringtype.md) <br/> |<span data-ttu-id="7098b-114">メッセージ追跡レポートの詳細を表します。</span><span class="sxs-lookup"><span data-stu-id="7098b-114">Represents how extensive the message tracking report should be.</span></span>  <br/> |
|[<span data-ttu-id="7098b-115">ドメイン (メッセージ追跡)</span><span class="sxs-lookup"><span data-stu-id="7098b-115">Domain (Message Tracking)</span></span>](domain-message-tracking.md) <br/> |<span data-ttu-id="7098b-116">メッセージ追跡が実行されるドメインの名前が含まれます。</span><span class="sxs-lookup"><span data-stu-id="7098b-116">Contains the name of the domain where the message tracking is executed.</span></span>  <br/> |
|[<span data-ttu-id="7098b-117">Sender (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="7098b-117">Sender (EmailAddressType)</span></span>](sender-emailaddresstype.md) <br/> |<span data-ttu-id="7098b-118">電子メールメッセージの送信者の連絡先情報が保存されています。</span><span class="sxs-lookup"><span data-stu-id="7098b-118">Contains contact information for the sender of the e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="7098b-119">PurportedSender</span><span class="sxs-lookup"><span data-stu-id="7098b-119">PurportedSender</span></span>](purportedsender.md) <br/> |<span data-ttu-id="7098b-120">電子メールメッセージの申し立て送信者の連絡先情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7098b-120">Contains contact information for the alleged sender of an e-mail message.</span></span>  <br/> |
|<span data-ttu-id="7098b-121">[[受信者]](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="7098b-121">[Recipient](recipient.md)</span></span> <br/> |<span data-ttu-id="7098b-122">メッセージの受信者の電子メールアドレスが保存されています。</span><span class="sxs-lookup"><span data-stu-id="7098b-122">Contains the e-mail address for the recipient of the message.</span></span>  <br/> |
|[<span data-ttu-id="7098b-123">件名</span><span class="sxs-lookup"><span data-stu-id="7098b-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="7098b-124">電子メールメッセージの件名を含みます。</span><span class="sxs-lookup"><span data-stu-id="7098b-124">Contains the subject of the e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="7098b-125">StartDateTime</span><span class="sxs-lookup"><span data-stu-id="7098b-125">StartDateTime</span></span>](startdatetime.md) <br/> |<span data-ttu-id="7098b-126">検索の開始日時を格納します。</span><span class="sxs-lookup"><span data-stu-id="7098b-126">Contains the starting date and time for the search.</span></span>  <br/> |
|[<span data-ttu-id="7098b-127">EndDateTime</span><span class="sxs-lookup"><span data-stu-id="7098b-127">EndDateTime</span></span>](enddatetime.md) <br/> |<span data-ttu-id="7098b-128">検索を終了する日付と時刻を含みます。</span><span class="sxs-lookup"><span data-stu-id="7098b-128">Contains the ending date and time for the search.</span></span>  <br/> |
|[<span data-ttu-id="7098b-129">MessageId</span><span class="sxs-lookup"><span data-stu-id="7098b-129">MessageId</span></span>](messageid.md) <br/> |<span data-ttu-id="7098b-130">検索のメッセージ識別子を含みます。</span><span class="sxs-lookup"><span data-stu-id="7098b-130">Contains the message identifier for the search.</span></span>  <br/> |
|[<span data-ttu-id="7098b-131">FederatedDeliveryMailbox</span><span class="sxs-lookup"><span data-stu-id="7098b-131">FederatedDeliveryMailbox</span></span>](federateddeliverymailbox.md) <br/> |<span data-ttu-id="7098b-132">クロスプレミスメッセージが送信されたメールボックスの名前が含まれます。</span><span class="sxs-lookup"><span data-stu-id="7098b-132">Contains the name of the mailbox where the cross-premise message was sent.</span></span>  <br/> |
|[<span data-ttu-id="7098b-133">DiagnosticsLevel</span><span class="sxs-lookup"><span data-stu-id="7098b-133">DiagnosticsLevel</span></span>](diagnosticslevel.md) <br/> |<span data-ttu-id="7098b-134">診断レポートの詳細レベルを表します。</span><span class="sxs-lookup"><span data-stu-id="7098b-134">Represents the level of detail for diagnostic reports.</span></span>  <br/> |
|[<span data-ttu-id="7098b-135">ServerHint</span><span class="sxs-lookup"><span data-stu-id="7098b-135">ServerHint</span></span>](serverhint.md) <br/> |<span data-ttu-id="7098b-136">リモートサイトまたはフォレスト内のメッセージを追跡するための開始点を表します。</span><span class="sxs-lookup"><span data-stu-id="7098b-136">Represents the starting point for tracking a message in a remote site or forest.</span></span>  <br/> |
|[<span data-ttu-id="7098b-137">プロパティ (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="7098b-137">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="7098b-138">1つ以上の追跡プロパティの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7098b-138">Contains a list of one or more tracking properties.</span></span> <span data-ttu-id="7098b-139">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="7098b-139">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7098b-140">親要素</span><span class="sxs-lookup"><span data-stu-id="7098b-140">Parent elements</span></span>

<span data-ttu-id="7098b-141">なし。</span><span class="sxs-lookup"><span data-stu-id="7098b-141">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="7098b-142">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7098b-142">Text value</span></span>

<span data-ttu-id="7098b-143">なし。</span><span class="sxs-lookup"><span data-stu-id="7098b-143">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7098b-144">注釈</span><span class="sxs-lookup"><span data-stu-id="7098b-144">Remarks</span></span>

<span data-ttu-id="7098b-145">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7098b-145">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7098b-146">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7098b-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7098b-147">Namespace</span><span class="sxs-lookup"><span data-stu-id="7098b-147">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7098b-148">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7098b-148">Schema Name</span></span>  <br/> |<span data-ttu-id="7098b-149">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="7098b-149">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7098b-150">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7098b-150">Validation File</span></span>  <br/> |<span data-ttu-id="7098b-151">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="7098b-151">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7098b-152">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7098b-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="7098b-153">正しくない</span><span class="sxs-lookup"><span data-stu-id="7098b-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7098b-154">関連項目</span><span class="sxs-lookup"><span data-stu-id="7098b-154">See also</span></span>



[<span data-ttu-id="7098b-155">FindMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="7098b-155">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)


- [<span data-ttu-id="7098b-156">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="7098b-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

