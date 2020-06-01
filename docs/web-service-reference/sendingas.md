---
title: SendingAs
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendingAs
api_type:
- schema
ms.assetid: b43ce19f-9ab0-4946-acb2-c5aafead9d35
description: SendingAs 要素は、ユーザーが送信しようとしている電子メールアドレスを表します。
ms.openlocfilehash: cd11bd60cbbe3434fcc1b0b9a1cfe0de9f0b1e21
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462137"
---
# <a name="sendingas"></a><span data-ttu-id="68854-103">SendingAs</span><span class="sxs-lookup"><span data-stu-id="68854-103">SendingAs</span></span>

<span data-ttu-id="68854-104">**SendingAs**要素は、ユーザーが送信しようとしている電子メールアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="68854-104">The **SendingAs** element represents an e-mail address that a user is trying to send as.</span></span> 
  
```XML
<SendingAs>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</SendingAs>
```

 <span data-ttu-id="68854-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="68854-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="68854-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="68854-106">Attributes and elements</span></span>

<span data-ttu-id="68854-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="68854-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="68854-108">属性</span><span class="sxs-lookup"><span data-stu-id="68854-108">Attributes</span></span>

<span data-ttu-id="68854-109">なし。</span><span class="sxs-lookup"><span data-stu-id="68854-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="68854-110">子要素</span><span class="sxs-lookup"><span data-stu-id="68854-110">Child elements</span></span>

|<span data-ttu-id="68854-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="68854-111">**Element**</span></span>|<span data-ttu-id="68854-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="68854-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="68854-113">Name (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="68854-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="68854-114">メールボックスユーザーの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="68854-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="68854-115">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="68854-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="68854-116">EmailAddress (非 Emptystringtype)</span><span class="sxs-lookup"><span data-stu-id="68854-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="68854-117">メールボックスユーザーのプライマリ簡易メール転送プロトコル (SMTP) アドレスを定義します。</span><span class="sxs-lookup"><span data-stu-id="68854-117">Defines the primary Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="68854-118">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="68854-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="68854-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="68854-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="68854-120">メールボックスのアドレスの種類を定義します。</span><span class="sxs-lookup"><span data-stu-id="68854-120">Defines the address type for the mailbox.</span></span> <span data-ttu-id="68854-121">既定値は SMTP です。</span><span class="sxs-lookup"><span data-stu-id="68854-121">The default is SMTP.</span></span> <span data-ttu-id="68854-122">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="68854-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="68854-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="68854-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="68854-124">電子メールユーザーによって表されるメールボックスの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="68854-124">Represents the type of mailbox that is represented by an e-mail user.</span></span> <span data-ttu-id="68854-125">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="68854-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="68854-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="68854-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="68854-127">ユーザーの連絡先フォルダーにある受信者の連絡先またはプライベート配布リストのアイテム識別子を定義します。</span><span class="sxs-lookup"><span data-stu-id="68854-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="68854-128">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="68854-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="68854-129">親要素</span><span class="sxs-lookup"><span data-stu-id="68854-129">Parent elements</span></span>

|<span data-ttu-id="68854-130">**要素**</span><span class="sxs-lookup"><span data-stu-id="68854-130">**Element**</span></span>|<span data-ttu-id="68854-131">**説明**</span><span class="sxs-lookup"><span data-stu-id="68854-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="68854-132">GetMailTips</span><span class="sxs-lookup"><span data-stu-id="68854-132">GetMailTips</span></span>](getmailtips.md) <br/> |<span data-ttu-id="68854-133">取得するメールヒントの受信者と種類が含まれています。</span><span class="sxs-lookup"><span data-stu-id="68854-133">Contains the recipients and types of mail tips to retrieve.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="68854-134">テキスト値</span><span class="sxs-lookup"><span data-stu-id="68854-134">Text value</span></span>

<span data-ttu-id="68854-135">なし。</span><span class="sxs-lookup"><span data-stu-id="68854-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="68854-136">注釈</span><span class="sxs-lookup"><span data-stu-id="68854-136">Remarks</span></span>

<span data-ttu-id="68854-137">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="68854-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="68854-138">要素の情報</span><span class="sxs-lookup"><span data-stu-id="68854-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="68854-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="68854-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="68854-140">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="68854-140">Schema Name</span></span>  <br/> |<span data-ttu-id="68854-141">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="68854-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="68854-142">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="68854-142">Validation File</span></span>  <br/> |<span data-ttu-id="68854-143">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="68854-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="68854-144">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="68854-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="68854-145">正しくない</span><span class="sxs-lookup"><span data-stu-id="68854-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="68854-146">関連項目</span><span class="sxs-lookup"><span data-stu-id="68854-146">See also</span></span>



- [<span data-ttu-id="68854-147">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="68854-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

