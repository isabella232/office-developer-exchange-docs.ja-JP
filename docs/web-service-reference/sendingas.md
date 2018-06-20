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
description: SendingAs 要素は、ユーザーが送信しようとする電子メール アドレスを表します。
ms.openlocfilehash: a5468ddb8facf99038d319252f7e1c780a888ca1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833338"
---
# <a name="sendingas"></a><span data-ttu-id="2dbcc-103">SendingAs</span><span class="sxs-lookup"><span data-stu-id="2dbcc-103">SendingAs</span></span>

<span data-ttu-id="2dbcc-104">**SendingAs**要素は、ユーザーが送信しようとする電子メール アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="2dbcc-104">The **SendingAs** element represents an e-mail address that a user is trying to send as.</span></span> 
  
```XML
<SendingAs>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</SendingAs>
```

 <span data-ttu-id="2dbcc-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="2dbcc-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2dbcc-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2dbcc-106">Attributes and elements</span></span>

<span data-ttu-id="2dbcc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2dbcc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2dbcc-108">属性</span><span class="sxs-lookup"><span data-stu-id="2dbcc-108">Attributes</span></span>

<span data-ttu-id="2dbcc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2dbcc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2dbcc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2dbcc-110">Child elements</span></span>

|<span data-ttu-id="2dbcc-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="2dbcc-111">**Element**</span></span>|<span data-ttu-id="2dbcc-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="2dbcc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2dbcc-113">名 (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="2dbcc-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="2dbcc-114">メールボックス ユーザーの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="2dbcc-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="2dbcc-115">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="2dbcc-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="2dbcc-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="2dbcc-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="2dbcc-117">メールボックスのユーザーのプライマリ簡易メール転送プロトコル (SMTP) アドレスを定義します。</span><span class="sxs-lookup"><span data-stu-id="2dbcc-117">Defines the primary Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="2dbcc-118">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="2dbcc-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="2dbcc-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="2dbcc-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="2dbcc-120">メールボックスのアドレスの種類を定義します。</span><span class="sxs-lookup"><span data-stu-id="2dbcc-120">Defines the address type for the mailbox.</span></span> <span data-ttu-id="2dbcc-121">既定値は、SMTP です。</span><span class="sxs-lookup"><span data-stu-id="2dbcc-121">The default is SMTP.</span></span> <span data-ttu-id="2dbcc-122">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="2dbcc-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="2dbcc-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="2dbcc-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="2dbcc-124">電子メール ユーザーで表されるメールボックスの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="2dbcc-124">Represents the type of mailbox that is represented by an e-mail user.</span></span> <span data-ttu-id="2dbcc-125">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="2dbcc-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="2dbcc-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="2dbcc-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="2dbcc-127">ユーザーのアドレス帳フォルダーから受信者の連絡先または個人用配布リストの項目の識別子を定義します。</span><span class="sxs-lookup"><span data-stu-id="2dbcc-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="2dbcc-128">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="2dbcc-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2dbcc-129">親要素</span><span class="sxs-lookup"><span data-stu-id="2dbcc-129">Parent elements</span></span>

|<span data-ttu-id="2dbcc-130">**要素**</span><span class="sxs-lookup"><span data-stu-id="2dbcc-130">**Element**</span></span>|<span data-ttu-id="2dbcc-131">**説明**</span><span class="sxs-lookup"><span data-stu-id="2dbcc-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2dbcc-132">GetMailTips</span><span class="sxs-lookup"><span data-stu-id="2dbcc-132">GetMailTips</span></span>](getmailtips.md) <br/> |<span data-ttu-id="2dbcc-133">受信者とメール ヒントの種類を取得するのにが含まれています。</span><span class="sxs-lookup"><span data-stu-id="2dbcc-133">Contains the recipients and types of mail tips to retrieve.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2dbcc-134">テキスト値</span><span class="sxs-lookup"><span data-stu-id="2dbcc-134">Text value</span></span>

<span data-ttu-id="2dbcc-135">なし。</span><span class="sxs-lookup"><span data-stu-id="2dbcc-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2dbcc-136">備考</span><span class="sxs-lookup"><span data-stu-id="2dbcc-136">Remarks</span></span>

<span data-ttu-id="2dbcc-137">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2dbcc-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2dbcc-138">要素情報</span><span class="sxs-lookup"><span data-stu-id="2dbcc-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2dbcc-139">名前空間</span><span class="sxs-lookup"><span data-stu-id="2dbcc-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2dbcc-140">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2dbcc-140">Schema Name</span></span>  <br/> |<span data-ttu-id="2dbcc-141">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="2dbcc-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2dbcc-142">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2dbcc-142">Validation File</span></span>  <br/> |<span data-ttu-id="2dbcc-143">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2dbcc-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2dbcc-144">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="2dbcc-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="2dbcc-145">False</span><span class="sxs-lookup"><span data-stu-id="2dbcc-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2dbcc-146">関連項目</span><span class="sxs-lookup"><span data-stu-id="2dbcc-146">See also</span></span>



- [<span data-ttu-id="2dbcc-147">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="2dbcc-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

