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
description: Recipient 要素は、イベントが発生した受信者を表します。
ms.openlocfilehash: eb7e85acf3c2b898b3f0bff4b63168d344e1daa8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465857"
---
# <a name="recipient"></a><span data-ttu-id="30e31-103">Recipient</span><span class="sxs-lookup"><span data-stu-id="30e31-103">Recipient</span></span>

<span data-ttu-id="30e31-104">**Recipient**要素は、イベントが発生した受信者を表します。</span><span class="sxs-lookup"><span data-stu-id="30e31-104">The **Recipient** element represents the recipient for whom the event occurred.</span></span> 
  
```XML
<Recipient>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Recipient>
```

 <span data-ttu-id="30e31-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="30e31-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="30e31-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="30e31-106">Attributes and elements</span></span>

<span data-ttu-id="30e31-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="30e31-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="30e31-108">属性</span><span class="sxs-lookup"><span data-stu-id="30e31-108">Attributes</span></span>

<span data-ttu-id="30e31-109">なし。</span><span class="sxs-lookup"><span data-stu-id="30e31-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="30e31-110">子要素</span><span class="sxs-lookup"><span data-stu-id="30e31-110">Child elements</span></span>

|<span data-ttu-id="30e31-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="30e31-111">**Element**</span></span>|<span data-ttu-id="30e31-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="30e31-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="30e31-113">Name (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="30e31-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="30e31-114">メールボックスユーザーの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="30e31-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="30e31-115">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="30e31-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="30e31-116">EmailAddress (非 Emptystringtype)</span><span class="sxs-lookup"><span data-stu-id="30e31-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="30e31-117">メールボックスユーザーのプライマリ簡易メール転送プロトコル (SMTP) アドレスを定義します。</span><span class="sxs-lookup"><span data-stu-id="30e31-117">Defines the primary Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="30e31-118">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="30e31-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="30e31-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="30e31-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="30e31-120">メールボックスに使用されるルーティングを定義します。</span><span class="sxs-lookup"><span data-stu-id="30e31-120">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="30e31-121">既定値は SMTP です。</span><span class="sxs-lookup"><span data-stu-id="30e31-121">The default value is SMTP.</span></span> <span data-ttu-id="30e31-122">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="30e31-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="30e31-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="30e31-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="30e31-124">電子メールアドレスによって表されるメールボックスの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="30e31-124">Represents the type of mailbox that is represented by the e-mail address.</span></span> <span data-ttu-id="30e31-125">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="30e31-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="30e31-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="30e31-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="30e31-127">ユーザーの連絡先フォルダーにある受信者の連絡先またはプライベート配布リストのアイテム識別子を定義します。</span><span class="sxs-lookup"><span data-stu-id="30e31-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="30e31-128">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="30e31-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="30e31-129">親要素</span><span class="sxs-lookup"><span data-stu-id="30e31-129">Parent elements</span></span>

|<span data-ttu-id="30e31-130">**要素**</span><span class="sxs-lookup"><span data-stu-id="30e31-130">**Element**</span></span>|<span data-ttu-id="30e31-131">**説明**</span><span class="sxs-lookup"><span data-stu-id="30e31-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="30e31-132">受信者 Trackingイベント</span><span class="sxs-lookup"><span data-stu-id="30e31-132">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="30e31-133">受信者に対する1つのイベントに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="30e31-133">Contains information for a single event for a recipient.</span></span>  <br/> |
|[<span data-ttu-id="30e31-134">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="30e31-134">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="30e31-135">検索するメッセージの種類の条件を指定します。</span><span class="sxs-lookup"><span data-stu-id="30e31-135">Specifies criteria for the types of messages to find.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="30e31-136">テキスト値</span><span class="sxs-lookup"><span data-stu-id="30e31-136">Text value</span></span>

<span data-ttu-id="30e31-137">なし。</span><span class="sxs-lookup"><span data-stu-id="30e31-137">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="30e31-138">注釈</span><span class="sxs-lookup"><span data-stu-id="30e31-138">Remarks</span></span>

<span data-ttu-id="30e31-139">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="30e31-139">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="30e31-140">要素の情報</span><span class="sxs-lookup"><span data-stu-id="30e31-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="30e31-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="30e31-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="30e31-142">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="30e31-142">Schema Name</span></span>  <br/> |<span data-ttu-id="30e31-143">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="30e31-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="30e31-144">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="30e31-144">Validation File</span></span>  <br/> |<span data-ttu-id="30e31-145">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="30e31-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="30e31-146">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="30e31-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="30e31-147">正しくない</span><span class="sxs-lookup"><span data-stu-id="30e31-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="30e31-148">関連項目</span><span class="sxs-lookup"><span data-stu-id="30e31-148">See also</span></span>



- [<span data-ttu-id="30e31-149">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="30e31-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

