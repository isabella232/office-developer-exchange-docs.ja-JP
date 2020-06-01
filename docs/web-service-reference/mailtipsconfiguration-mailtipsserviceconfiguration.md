---
title: Mailヒント構成 (MailTipsServiceConfiguration)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailTipsConfiguration
api_type:
- schema
ms.assetid: 9a34515e-815b-4c61-b118-d5f66b80238f
description: Mailヒント構成要素には、メールヒントサービスのサービス構成情報が含まれています。
ms.openlocfilehash: 9128ee99545066899c3b27b624f10a9f1bd36c9d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467789"
---
# <a name="mailtipsconfiguration-mailtipsserviceconfiguration"></a><span data-ttu-id="1486e-103">Mailヒント構成 (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="1486e-103">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>

<span data-ttu-id="1486e-104">**Mailヒント構成**要素には、メールヒントサービスのサービス構成情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1486e-104">The **MailTipsConfiguration** element contains service configuration information for the mail tips service.</span></span> 
  
```XML
<MailTipsConfiguration>
   <MailTipsEnabled/>
   <MaxRecipientsPerGetMailTipsRequest/>
   <MaxMessageSize/>
   <LargeAudienceThreshold/>
   <ShowExternalRecipientCount/>
   <InternalDomains/>
</MailTipsConfiguration>
```

 <span data-ttu-id="1486e-105">**MailTipsServiceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="1486e-105">**MailTipsServiceConfiguration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1486e-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1486e-106">Attributes and elements</span></span>

<span data-ttu-id="1486e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1486e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1486e-108">属性</span><span class="sxs-lookup"><span data-stu-id="1486e-108">Attributes</span></span>

<span data-ttu-id="1486e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1486e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1486e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1486e-110">Child elements</span></span>

|<span data-ttu-id="1486e-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="1486e-111">**Element**</span></span>|<span data-ttu-id="1486e-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="1486e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1486e-113">Mailヒント有効</span><span class="sxs-lookup"><span data-stu-id="1486e-113">MailTipsEnabled</span></span>](mailtipsenabled.md) <br/> |<span data-ttu-id="1486e-114">メールヒントサービスが利用可能かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1486e-114">Indicates whether the mail tips service is available.</span></span> <span data-ttu-id="1486e-115">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="1486e-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="1486e-116">Max受信者 Spergetmailヒント要求</span><span class="sxs-lookup"><span data-stu-id="1486e-116">MaxRecipientsPerGetMailTipsRequest</span></span>](maxrecipientspergetmailtipsrequest.md) <br/> |<span data-ttu-id="1486e-117">[Getmailtips ヒント操作](getmailtips-operation.md)に渡すことができる受信者の最大数を示します。</span><span class="sxs-lookup"><span data-stu-id="1486e-117">Indicates the maximum number of recipients that can be passed to the [GetMailTips operation](getmailtips-operation.md).</span></span> <span data-ttu-id="1486e-118">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="1486e-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="1486e-119">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="1486e-119">MaxMessageSize</span></span>](maxmessagesize.md) <br/> |<span data-ttu-id="1486e-120">受信者が受け付けることができる最大メッセージサイズを表します。</span><span class="sxs-lookup"><span data-stu-id="1486e-120">Represents the maximum message size a recipient can accept.</span></span> <span data-ttu-id="1486e-121">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="1486e-121">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="1486e-122">LargeAudienceThreshold</span><span class="sxs-lookup"><span data-stu-id="1486e-122">LargeAudienceThreshold</span></span>](largeaudiencethreshold.md) <br/> |<span data-ttu-id="1486e-123">クライアントの大規模な対象ユーザーのしきい値を表します。</span><span class="sxs-lookup"><span data-stu-id="1486e-123">Represents the large audience threshold for a client.</span></span> <span data-ttu-id="1486e-124">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="1486e-124">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="1486e-125">Showexternal受信者カウント</span><span class="sxs-lookup"><span data-stu-id="1486e-125">ShowExternalRecipientCount</span></span>](showexternalrecipientcount.md) <br/> |<span data-ttu-id="1486e-126">[Getmailtips ヒント操作](getmailtips-operation.md)のコンシューマーが、メッセージの宛先である外部受信者の数を示すメールヒントを表示する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1486e-126">Indicates whether consumers of the [GetMailTips operation](getmailtips-operation.md) have to show mail tips that indicate the number of external recipients to which a message is addressed.</span></span> <span data-ttu-id="1486e-127">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="1486e-127">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="1486e-128">InternalDomains (SmtpDomainList)</span><span class="sxs-lookup"><span data-stu-id="1486e-128">InternalDomains (SmtpDomainList)</span></span>](internaldomains-smtpdomainlist.md) <br/> |<span data-ttu-id="1486e-129">組織の内部 SMTP ドメインのリストを識別します。</span><span class="sxs-lookup"><span data-stu-id="1486e-129">Identifies the list of internal SMTP domains of the organization.</span></span> <span data-ttu-id="1486e-130">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="1486e-130">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1486e-131">親要素</span><span class="sxs-lookup"><span data-stu-id="1486e-131">Parent elements</span></span>

|<span data-ttu-id="1486e-132">**要素**</span><span class="sxs-lookup"><span data-stu-id="1486e-132">**Element**</span></span>|<span data-ttu-id="1486e-133">**説明**</span><span class="sxs-lookup"><span data-stu-id="1486e-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1486e-134">ServiceConfigurationResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="1486e-134">ServiceConfigurationResponseMessageType</span></span>](serviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="1486e-135">サービス構成の設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="1486e-135">Contains service configuration settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1486e-136">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1486e-136">Text value</span></span>

<span data-ttu-id="1486e-137">なし。</span><span class="sxs-lookup"><span data-stu-id="1486e-137">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1486e-138">注釈</span><span class="sxs-lookup"><span data-stu-id="1486e-138">Remarks</span></span>

<span data-ttu-id="1486e-139">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="1486e-139">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1486e-140">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1486e-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1486e-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="1486e-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1486e-142">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1486e-142">Schema Name</span></span>  <br/> |<span data-ttu-id="1486e-143">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="1486e-143">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1486e-144">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1486e-144">Validation File</span></span>  <br/> |<span data-ttu-id="1486e-145">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="1486e-145">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1486e-146">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1486e-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="1486e-147">正しくない</span><span class="sxs-lookup"><span data-stu-id="1486e-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1486e-148">関連項目</span><span class="sxs-lookup"><span data-stu-id="1486e-148">See also</span></span>



- [<span data-ttu-id="1486e-149">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="1486e-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

