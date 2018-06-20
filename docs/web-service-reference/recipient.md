---
title: Recipient
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Recipient
api_type:
- schema
ms.assetid: 52adbb30-3bfd-48aa-9ea8-9f7d3b4bee44
description: 受信者要素は、イベントが発生した対象となる受信者を表します。
ms.openlocfilehash: e8e8f9d6031d27c7441017c85eb26a143258b183
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832971"
---
# <a name="recipient"></a><span data-ttu-id="63af9-103">Recipient</span><span class="sxs-lookup"><span data-stu-id="63af9-103">Recipient</span></span>

<span data-ttu-id="63af9-104">**受信者**要素は、イベントが発生した対象となる受信者を表します。</span><span class="sxs-lookup"><span data-stu-id="63af9-104">The **Recipient** element represents the recipient for whom the event occurred.</span></span> 
  
```XML
<Recipient>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Recipient>
```

 <span data-ttu-id="63af9-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="63af9-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="63af9-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="63af9-106">Attributes and elements</span></span>

<span data-ttu-id="63af9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="63af9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="63af9-108">属性</span><span class="sxs-lookup"><span data-stu-id="63af9-108">Attributes</span></span>

<span data-ttu-id="63af9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="63af9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="63af9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="63af9-110">Child elements</span></span>

|<span data-ttu-id="63af9-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="63af9-111">**Element**</span></span>|<span data-ttu-id="63af9-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="63af9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="63af9-113">名 (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="63af9-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="63af9-114">メールボックス ユーザーの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="63af9-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="63af9-115">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="63af9-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="63af9-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="63af9-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="63af9-117">メールボックスのユーザーのプライマリ簡易メール転送プロトコル (SMTP) アドレスを定義します。</span><span class="sxs-lookup"><span data-stu-id="63af9-117">Defines the primary Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="63af9-118">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="63af9-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="63af9-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="63af9-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="63af9-120">メールボックスに使用されるルーティングを定義します。</span><span class="sxs-lookup"><span data-stu-id="63af9-120">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="63af9-121">既定値は、SMTP です。</span><span class="sxs-lookup"><span data-stu-id="63af9-121">The default value is SMTP.</span></span> <span data-ttu-id="63af9-122">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="63af9-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="63af9-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="63af9-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="63af9-124">電子メール アドレスで表されるメールボックスの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="63af9-124">Represents the type of mailbox that is represented by the e-mail address.</span></span> <span data-ttu-id="63af9-125">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="63af9-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="63af9-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="63af9-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="63af9-127">ユーザーのアドレス帳フォルダーから受信者の連絡先または個人用配布リストの項目の識別子を定義します。</span><span class="sxs-lookup"><span data-stu-id="63af9-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="63af9-128">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="63af9-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="63af9-129">親要素</span><span class="sxs-lookup"><span data-stu-id="63af9-129">Parent elements</span></span>

|<span data-ttu-id="63af9-130">**要素**</span><span class="sxs-lookup"><span data-stu-id="63af9-130">**Element**</span></span>|<span data-ttu-id="63af9-131">**説明**</span><span class="sxs-lookup"><span data-stu-id="63af9-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="63af9-132">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="63af9-132">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="63af9-133">受信者の 1 つのイベントの情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="63af9-133">Contains information for a single event for a recipient.</span></span>  <br/> |
|[<span data-ttu-id="63af9-134">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="63af9-134">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="63af9-135">検索するメッセージの種類の条件を指定します。</span><span class="sxs-lookup"><span data-stu-id="63af9-135">Specifies criteria for the types of messages to find.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="63af9-136">テキスト値</span><span class="sxs-lookup"><span data-stu-id="63af9-136">Text value</span></span>

<span data-ttu-id="63af9-137">なし。</span><span class="sxs-lookup"><span data-stu-id="63af9-137">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="63af9-138">備考</span><span class="sxs-lookup"><span data-stu-id="63af9-138">Remarks</span></span>

<span data-ttu-id="63af9-139">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="63af9-139">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="63af9-140">要素情報</span><span class="sxs-lookup"><span data-stu-id="63af9-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="63af9-141">名前空間</span><span class="sxs-lookup"><span data-stu-id="63af9-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="63af9-142">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="63af9-142">Schema Name</span></span>  <br/> |<span data-ttu-id="63af9-143">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="63af9-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="63af9-144">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="63af9-144">Validation File</span></span>  <br/> |<span data-ttu-id="63af9-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="63af9-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="63af9-146">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="63af9-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="63af9-147">False</span><span class="sxs-lookup"><span data-stu-id="63af9-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="63af9-148">関連項目</span><span class="sxs-lookup"><span data-stu-id="63af9-148">See also</span></span>



- [<span data-ttu-id="63af9-149">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="63af9-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

