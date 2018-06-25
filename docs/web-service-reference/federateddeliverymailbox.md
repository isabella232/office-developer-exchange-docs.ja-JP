---
title: FederatedDeliveryMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FederatedDeliveryMailbox
api_type:
- schema
ms.assetid: cd56bcc0-d24a-4e8b-87bd-999bf69234b7
description: FederatedDeliveryMailbox 要素は、設置型の間のメッセージの送付先となるメールボックスを表します。
ms.openlocfilehash: 4a9250455f8de3ede25f2b5ba9433690137ca1d3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760467"
---
# <a name="federateddeliverymailbox"></a><span data-ttu-id="ad261-103">FederatedDeliveryMailbox</span><span class="sxs-lookup"><span data-stu-id="ad261-103">FederatedDeliveryMailbox</span></span>

<span data-ttu-id="ad261-104">**FederatedDeliveryMailbox**要素は、設置型の間のメッセージの送付先となるメールボックスを表します。</span><span class="sxs-lookup"><span data-stu-id="ad261-104">The **FederatedDeliveryMailbox** element represents the mailbox to which a cross-premise message was sent.</span></span> 
  
```XML
<FederatedDeliveryMailbox>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</FederatedDeliveryMailbox>
```

 <span data-ttu-id="ad261-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="ad261-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ad261-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ad261-106">Attributes and elements</span></span>

<span data-ttu-id="ad261-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ad261-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ad261-108">属性</span><span class="sxs-lookup"><span data-stu-id="ad261-108">Attributes</span></span>

<span data-ttu-id="ad261-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ad261-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ad261-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ad261-110">Child elements</span></span>

|<span data-ttu-id="ad261-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="ad261-111">**Element**</span></span>|<span data-ttu-id="ad261-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="ad261-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad261-113">名 (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="ad261-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="ad261-114">メールボックス ユーザーの名前を定義します。</span><span class="sxs-lookup"><span data-stu-id="ad261-114">Defines the name of the mailbox user.</span></span> <span data-ttu-id="ad261-115">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="ad261-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="ad261-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="ad261-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="ad261-117">メールボックスのユーザーの簡易メール転送プロトコル (SMTP) アドレスを定義します。</span><span class="sxs-lookup"><span data-stu-id="ad261-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="ad261-118">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="ad261-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="ad261-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="ad261-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="ad261-120">メールボックスに使用されるルーティングを定義します。</span><span class="sxs-lookup"><span data-stu-id="ad261-120">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="ad261-121">既定値は、SMTP です。</span><span class="sxs-lookup"><span data-stu-id="ad261-121">The default is SMTP.</span></span> <span data-ttu-id="ad261-122">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="ad261-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="ad261-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="ad261-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="ad261-124">メールボックスのユーザーのメールボックスの種類を定義します。</span><span class="sxs-lookup"><span data-stu-id="ad261-124">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="ad261-125">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="ad261-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="ad261-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="ad261-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="ad261-127">ユーザーのアドレス帳フォルダーから受信者の連絡先または個人用配布リストの項目の識別子を定義します。</span><span class="sxs-lookup"><span data-stu-id="ad261-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="ad261-128">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="ad261-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ad261-129">親要素</span><span class="sxs-lookup"><span data-stu-id="ad261-129">Parent elements</span></span>

|<span data-ttu-id="ad261-130">**要素**</span><span class="sxs-lookup"><span data-stu-id="ad261-130">**Element**</span></span>|<span data-ttu-id="ad261-131">**説明**</span><span class="sxs-lookup"><span data-stu-id="ad261-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad261-132">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="ad261-132">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="ad261-133">検索するメッセージの種類の条件が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ad261-133">Contains criteria for the types of messages to find.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ad261-134">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ad261-134">Text value</span></span>

<span data-ttu-id="ad261-135">なし。</span><span class="sxs-lookup"><span data-stu-id="ad261-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ad261-136">備考</span><span class="sxs-lookup"><span data-stu-id="ad261-136">Remarks</span></span>

<span data-ttu-id="ad261-137">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ad261-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ad261-138">要素情報</span><span class="sxs-lookup"><span data-stu-id="ad261-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ad261-139">名前空間</span><span class="sxs-lookup"><span data-stu-id="ad261-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ad261-140">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ad261-140">Schema Name</span></span>  <br/> |<span data-ttu-id="ad261-141">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="ad261-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ad261-142">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ad261-142">Validation File</span></span>  <br/> |<span data-ttu-id="ad261-143">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ad261-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ad261-144">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ad261-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="ad261-145">False</span><span class="sxs-lookup"><span data-stu-id="ad261-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ad261-146">関連項目</span><span class="sxs-lookup"><span data-stu-id="ad261-146">See also</span></span>



- [<span data-ttu-id="ad261-147">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="ad261-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

