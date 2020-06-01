---
title: RecipientAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecipientAddress
api_type:
- schema
ms.assetid: 9ae6351a-2c60-4715-a489-5681a13641f9
description: '[受信者アドレス] 要素は、受信者のメールボックスを表します。'
ms.openlocfilehash: f4b6edd034dd91471e6496f6b0cca65bd3ffb69a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465850"
---
# <a name="recipientaddress"></a><span data-ttu-id="267cc-103">RecipientAddress</span><span class="sxs-lookup"><span data-stu-id="267cc-103">RecipientAddress</span></span>

<span data-ttu-id="267cc-104">[受信者**アドレス**] 要素は、受信者のメールボックスを表します。</span><span class="sxs-lookup"><span data-stu-id="267cc-104">The **RecipientAddress** element represents the mailbox of the recipient.</span></span> 
  
```xml
<RecipientAddress>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</RecipientAddress>
```

 <span data-ttu-id="267cc-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="267cc-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="267cc-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="267cc-106">Attributes and elements</span></span>

<span data-ttu-id="267cc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="267cc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="267cc-108">属性</span><span class="sxs-lookup"><span data-stu-id="267cc-108">Attributes</span></span>

<span data-ttu-id="267cc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="267cc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="267cc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="267cc-110">Child elements</span></span>

|<span data-ttu-id="267cc-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="267cc-111">**Element**</span></span>|<span data-ttu-id="267cc-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="267cc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="267cc-113">Name (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="267cc-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="267cc-114">メールボックスユーザーの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="267cc-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="267cc-115">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="267cc-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="267cc-116">EmailAddress (非 Emptystringtype)</span><span class="sxs-lookup"><span data-stu-id="267cc-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="267cc-117">メールボックスユーザーの簡易メール転送プロトコル (SMTP) アドレスを定義します。</span><span class="sxs-lookup"><span data-stu-id="267cc-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="267cc-118">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="267cc-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="267cc-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="267cc-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="267cc-120">受信者のルーティングプロトコルを表します。</span><span class="sxs-lookup"><span data-stu-id="267cc-120">Represents the routing protocol for the recipient.</span></span> <span data-ttu-id="267cc-121">既定値は SMTP です。</span><span class="sxs-lookup"><span data-stu-id="267cc-121">The default is SMTP.</span></span> <span data-ttu-id="267cc-122">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="267cc-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="267cc-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="267cc-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="267cc-124">電子メールアドレスによって表されるメールボックスの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="267cc-124">Represents the type of mailbox that is represented by the e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="267cc-125">ItemId</span><span class="sxs-lookup"><span data-stu-id="267cc-125">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="267cc-126">ユーザーの連絡先フォルダーにある受信者の連絡先またはプライベート配布リストのアイテム識別子を定義します。</span><span class="sxs-lookup"><span data-stu-id="267cc-126">Defines the item identifier of a contact or private distribution list for recipients from a user's contacts folder.</span></span> <span data-ttu-id="267cc-127">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="267cc-127">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="267cc-128">親要素</span><span class="sxs-lookup"><span data-stu-id="267cc-128">Parent elements</span></span>

|<span data-ttu-id="267cc-129">**要素**</span><span class="sxs-lookup"><span data-stu-id="267cc-129">**Element**</span></span>|<span data-ttu-id="267cc-130">**説明**</span><span class="sxs-lookup"><span data-stu-id="267cc-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="267cc-131">メールヒント</span><span class="sxs-lookup"><span data-stu-id="267cc-131">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="267cc-132">さまざまな種類のメールヒントの値を表します。</span><span class="sxs-lookup"><span data-stu-id="267cc-132">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="267cc-133">注釈</span><span class="sxs-lookup"><span data-stu-id="267cc-133">Remarks</span></span>

<span data-ttu-id="267cc-134">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="267cc-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="267cc-135">要素の情報</span><span class="sxs-lookup"><span data-stu-id="267cc-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="267cc-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="267cc-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="267cc-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="267cc-137">Schema Name</span></span>  <br/> |<span data-ttu-id="267cc-138">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="267cc-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="267cc-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="267cc-139">Validation File</span></span>  <br/> |<span data-ttu-id="267cc-140">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="267cc-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="267cc-141">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="267cc-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="267cc-142">正しくない</span><span class="sxs-lookup"><span data-stu-id="267cc-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="267cc-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="267cc-143">See also</span></span>



- [<span data-ttu-id="267cc-144">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="267cc-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

