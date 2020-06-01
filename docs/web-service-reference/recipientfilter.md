---
title: RecipientFilter
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecipientFilter
api_type:
- schema
ms.assetid: 956c287a-a38a-49a7-a877-6d2088dfbc06
description: 受信者 Filter 要素は、指定されたメッセージ追跡レポートで使用する受信者のアドレスを表します。
ms.openlocfilehash: 945adf9155434e0690debfccc7caf70ba0cb94ec
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465808"
---
# <a name="recipientfilter"></a><span data-ttu-id="b215b-103">RecipientFilter</span><span class="sxs-lookup"><span data-stu-id="b215b-103">RecipientFilter</span></span>

<span data-ttu-id="b215b-104">受信者**filter**要素は、指定されたメッセージ追跡レポートで使用する受信者のアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="b215b-104">The **RecipientFilter** element represents a recipient address to use with the specified message tracking report.</span></span> 
  
```XML
 <RecipientFilter>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</RecipientFilter>
```

 <span data-ttu-id="b215b-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="b215b-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b215b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b215b-106">Attributes and elements</span></span>

<span data-ttu-id="b215b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b215b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b215b-108">属性</span><span class="sxs-lookup"><span data-stu-id="b215b-108">Attributes</span></span>

<span data-ttu-id="b215b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b215b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b215b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b215b-110">Child elements</span></span>

|<span data-ttu-id="b215b-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="b215b-111">**Element**</span></span>|<span data-ttu-id="b215b-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="b215b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b215b-113">Name (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="b215b-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="b215b-114">メールボックスユーザーの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="b215b-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="b215b-115">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="b215b-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="b215b-116">EmailAddress (非 Emptystringtype)</span><span class="sxs-lookup"><span data-stu-id="b215b-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="b215b-117">メールボックスユーザーのプライマリ簡易メール転送プロトコル (SMTP) アドレスを定義します。</span><span class="sxs-lookup"><span data-stu-id="b215b-117">Defines the primary Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="b215b-118">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="b215b-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="b215b-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="b215b-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="b215b-120">この受信者のルーティングプロトコルを表します。</span><span class="sxs-lookup"><span data-stu-id="b215b-120">Represents the routing protocol for this recipient.</span></span> <span data-ttu-id="b215b-121">既定値は SMTP です。</span><span class="sxs-lookup"><span data-stu-id="b215b-121">The default value is SMTP.</span></span> <span data-ttu-id="b215b-122">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="b215b-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="b215b-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="b215b-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="b215b-124">電子メールアドレスによって表されるメールボックスの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="b215b-124">Represents the type of mailbox that is represented by the e-mail address.</span></span> <span data-ttu-id="b215b-125">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="b215b-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="b215b-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="b215b-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="b215b-127">ユーザーの連絡先フォルダーにある受信者の連絡先またはプライベート配布リストのアイテム識別子を定義します。</span><span class="sxs-lookup"><span data-stu-id="b215b-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="b215b-128">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="b215b-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b215b-129">親要素</span><span class="sxs-lookup"><span data-stu-id="b215b-129">Parent elements</span></span>

|<span data-ttu-id="b215b-130">**要素**</span><span class="sxs-lookup"><span data-stu-id="b215b-130">**Element**</span></span>|<span data-ttu-id="b215b-131">**説明**</span><span class="sxs-lookup"><span data-stu-id="b215b-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b215b-132">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="b215b-132">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="b215b-133">指定された ID の完全なメッセージ追跡レポートを取得する[Getmessagetrackingreport 操作](getmessagetrackingreport-operation.md)の要求を含みます。</span><span class="sxs-lookup"><span data-stu-id="b215b-133">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b215b-134">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b215b-134">Text value</span></span>

<span data-ttu-id="b215b-135">なし。</span><span class="sxs-lookup"><span data-stu-id="b215b-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b215b-136">注釈</span><span class="sxs-lookup"><span data-stu-id="b215b-136">Remarks</span></span>

<span data-ttu-id="b215b-137">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b215b-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b215b-138">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b215b-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b215b-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="b215b-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b215b-140">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b215b-140">Schema Name</span></span>  <br/> |<span data-ttu-id="b215b-141">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="b215b-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b215b-142">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b215b-142">Validation File</span></span>  <br/> |<span data-ttu-id="b215b-143">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="b215b-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b215b-144">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b215b-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="b215b-145">正しくない</span><span class="sxs-lookup"><span data-stu-id="b215b-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b215b-146">関連項目</span><span class="sxs-lookup"><span data-stu-id="b215b-146">See also</span></span>



[<span data-ttu-id="b215b-147">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="b215b-147">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="b215b-148">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="b215b-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

