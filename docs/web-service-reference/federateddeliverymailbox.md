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
description: FederatedDeliveryMailbox 要素は、クロスプレミスメッセージが送信されたメールボックスを表します。
ms.openlocfilehash: d493ed81e82237b7257e8c469f4552d931b73aa6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461948"
---
# <a name="federateddeliverymailbox"></a><span data-ttu-id="08f1e-103">FederatedDeliveryMailbox</span><span class="sxs-lookup"><span data-stu-id="08f1e-103">FederatedDeliveryMailbox</span></span>

<span data-ttu-id="08f1e-104">**FederatedDeliveryMailbox**要素は、クロスプレミスメッセージが送信されたメールボックスを表します。</span><span class="sxs-lookup"><span data-stu-id="08f1e-104">The **FederatedDeliveryMailbox** element represents the mailbox to which a cross-premise message was sent.</span></span> 
  
```XML
<FederatedDeliveryMailbox>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</FederatedDeliveryMailbox>
```

 <span data-ttu-id="08f1e-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="08f1e-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="08f1e-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="08f1e-106">Attributes and elements</span></span>

<span data-ttu-id="08f1e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="08f1e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="08f1e-108">属性</span><span class="sxs-lookup"><span data-stu-id="08f1e-108">Attributes</span></span>

<span data-ttu-id="08f1e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="08f1e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="08f1e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="08f1e-110">Child elements</span></span>

|<span data-ttu-id="08f1e-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="08f1e-111">**Element**</span></span>|<span data-ttu-id="08f1e-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="08f1e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="08f1e-113">Name (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="08f1e-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="08f1e-114">メールボックスユーザーの名前を定義します。</span><span class="sxs-lookup"><span data-stu-id="08f1e-114">Defines the name of the mailbox user.</span></span> <span data-ttu-id="08f1e-115">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="08f1e-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="08f1e-116">EmailAddress (非 Emptystringtype)</span><span class="sxs-lookup"><span data-stu-id="08f1e-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="08f1e-117">メールボックスユーザーの簡易メール転送プロトコル (SMTP) アドレスを定義します。</span><span class="sxs-lookup"><span data-stu-id="08f1e-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="08f1e-118">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="08f1e-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="08f1e-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="08f1e-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="08f1e-120">メールボックスに使用されるルーティングを定義します。</span><span class="sxs-lookup"><span data-stu-id="08f1e-120">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="08f1e-121">既定値は SMTP です。</span><span class="sxs-lookup"><span data-stu-id="08f1e-121">The default is SMTP.</span></span> <span data-ttu-id="08f1e-122">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="08f1e-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="08f1e-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="08f1e-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="08f1e-124">メールボックスユーザーのメールボックスの種類を定義します。</span><span class="sxs-lookup"><span data-stu-id="08f1e-124">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="08f1e-125">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="08f1e-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="08f1e-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="08f1e-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="08f1e-127">ユーザーの連絡先フォルダーにある受信者の連絡先またはプライベート配布リストのアイテム識別子を定義します。</span><span class="sxs-lookup"><span data-stu-id="08f1e-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="08f1e-128">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="08f1e-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="08f1e-129">親要素</span><span class="sxs-lookup"><span data-stu-id="08f1e-129">Parent elements</span></span>

|<span data-ttu-id="08f1e-130">**要素**</span><span class="sxs-lookup"><span data-stu-id="08f1e-130">**Element**</span></span>|<span data-ttu-id="08f1e-131">**説明**</span><span class="sxs-lookup"><span data-stu-id="08f1e-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="08f1e-132">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="08f1e-132">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="08f1e-133">検索するメッセージの種類に関する条件を含みます。</span><span class="sxs-lookup"><span data-stu-id="08f1e-133">Contains criteria for the types of messages to find.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="08f1e-134">テキスト値</span><span class="sxs-lookup"><span data-stu-id="08f1e-134">Text value</span></span>

<span data-ttu-id="08f1e-135">なし。</span><span class="sxs-lookup"><span data-stu-id="08f1e-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="08f1e-136">注釈</span><span class="sxs-lookup"><span data-stu-id="08f1e-136">Remarks</span></span>

<span data-ttu-id="08f1e-137">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="08f1e-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="08f1e-138">要素の情報</span><span class="sxs-lookup"><span data-stu-id="08f1e-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="08f1e-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="08f1e-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="08f1e-140">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="08f1e-140">Schema Name</span></span>  <br/> |<span data-ttu-id="08f1e-141">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="08f1e-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="08f1e-142">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="08f1e-142">Validation File</span></span>  <br/> |<span data-ttu-id="08f1e-143">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="08f1e-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="08f1e-144">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="08f1e-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="08f1e-145">正しくない</span><span class="sxs-lookup"><span data-stu-id="08f1e-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="08f1e-146">関連項目</span><span class="sxs-lookup"><span data-stu-id="08f1e-146">See also</span></span>



- [<span data-ttu-id="08f1e-147">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="08f1e-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

