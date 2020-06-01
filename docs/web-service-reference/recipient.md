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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465857"
---
# <a name="recipient"></a><span data-ttu-id="12107-103">Recipient</span><span class="sxs-lookup"><span data-stu-id="12107-103">Recipient</span></span>

<span data-ttu-id="12107-104">**Recipient**要素は、イベントが発生した受信者を表します。</span><span class="sxs-lookup"><span data-stu-id="12107-104">The **Recipient** element represents the recipient for whom the event occurred.</span></span> 
  
```XML
<Recipient>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Recipient>
```

 <span data-ttu-id="12107-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="12107-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="12107-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="12107-106">Attributes and elements</span></span>

<span data-ttu-id="12107-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="12107-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="12107-108">属性</span><span class="sxs-lookup"><span data-stu-id="12107-108">Attributes</span></span>

<span data-ttu-id="12107-109">なし。</span><span class="sxs-lookup"><span data-stu-id="12107-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="12107-110">子要素</span><span class="sxs-lookup"><span data-stu-id="12107-110">Child elements</span></span>

|<span data-ttu-id="12107-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="12107-111">**Element**</span></span>|<span data-ttu-id="12107-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="12107-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="12107-113">Name (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="12107-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="12107-114">メールボックスユーザーの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="12107-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="12107-115">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="12107-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="12107-116">EmailAddress (非 Emptystringtype)</span><span class="sxs-lookup"><span data-stu-id="12107-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="12107-117">メールボックスユーザーのプライマリ簡易メール転送プロトコル (SMTP) アドレスを定義します。</span><span class="sxs-lookup"><span data-stu-id="12107-117">Defines the primary Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="12107-118">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="12107-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="12107-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="12107-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="12107-120">メールボックスに使用されるルーティングを定義します。</span><span class="sxs-lookup"><span data-stu-id="12107-120">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="12107-121">既定値は SMTP です。</span><span class="sxs-lookup"><span data-stu-id="12107-121">The default value is SMTP.</span></span> <span data-ttu-id="12107-122">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="12107-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="12107-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="12107-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="12107-124">電子メールアドレスによって表されるメールボックスの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="12107-124">Represents the type of mailbox that is represented by the e-mail address.</span></span> <span data-ttu-id="12107-125">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="12107-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="12107-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="12107-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="12107-127">ユーザーの連絡先フォルダーにある受信者の連絡先またはプライベート配布リストのアイテム識別子を定義します。</span><span class="sxs-lookup"><span data-stu-id="12107-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="12107-128">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="12107-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="12107-129">親要素</span><span class="sxs-lookup"><span data-stu-id="12107-129">Parent elements</span></span>

|<span data-ttu-id="12107-130">**要素**</span><span class="sxs-lookup"><span data-stu-id="12107-130">**Element**</span></span>|<span data-ttu-id="12107-131">**説明**</span><span class="sxs-lookup"><span data-stu-id="12107-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="12107-132">受信者 Trackingイベント</span><span class="sxs-lookup"><span data-stu-id="12107-132">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="12107-133">受信者に対する1つのイベントに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="12107-133">Contains information for a single event for a recipient.</span></span>  <br/> |
|[<span data-ttu-id="12107-134">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="12107-134">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="12107-135">検索するメッセージの種類の条件を指定します。</span><span class="sxs-lookup"><span data-stu-id="12107-135">Specifies criteria for the types of messages to find.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="12107-136">テキスト値</span><span class="sxs-lookup"><span data-stu-id="12107-136">Text value</span></span>

<span data-ttu-id="12107-137">なし。</span><span class="sxs-lookup"><span data-stu-id="12107-137">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="12107-138">注釈</span><span class="sxs-lookup"><span data-stu-id="12107-138">Remarks</span></span>

<span data-ttu-id="12107-139">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="12107-139">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="12107-140">要素の情報</span><span class="sxs-lookup"><span data-stu-id="12107-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="12107-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="12107-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="12107-142">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="12107-142">Schema Name</span></span>  <br/> |<span data-ttu-id="12107-143">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="12107-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="12107-144">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="12107-144">Validation File</span></span>  <br/> |<span data-ttu-id="12107-145">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="12107-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="12107-146">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="12107-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="12107-147">正しくない</span><span class="sxs-lookup"><span data-stu-id="12107-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="12107-148">関連項目</span><span class="sxs-lookup"><span data-stu-id="12107-148">See also</span></span>



- [<span data-ttu-id="12107-149">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="12107-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

