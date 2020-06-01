---
title: Address (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Address
api_type:
- schema
ms.assetid: 518641c8-7f6f-496c-86f9-341e7c1bb44c
description: Address 要素は、完全に解決された電子メールアドレスを表します。
ms.openlocfilehash: 591bc675165ec80f69407bd8ee19d16c9ddff15a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464904"
---
# <a name="address-emailaddresstype"></a><span data-ttu-id="acf67-103">Address (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="acf67-103">Address (EmailAddressType)</span></span>

<span data-ttu-id="acf67-104">**Address**要素は、完全に解決された電子メールアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="acf67-104">The **Address** element represents a fully resolved e-mail address.</span></span> 
  
```XML
<Address>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Address >
```

 <span data-ttu-id="acf67-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="acf67-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="acf67-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="acf67-106">Attributes and elements</span></span>

<span data-ttu-id="acf67-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="acf67-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="acf67-108">属性</span><span class="sxs-lookup"><span data-stu-id="acf67-108">Attributes</span></span>

<span data-ttu-id="acf67-109">なし。</span><span class="sxs-lookup"><span data-stu-id="acf67-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="acf67-110">子要素</span><span class="sxs-lookup"><span data-stu-id="acf67-110">Child elements</span></span>

|<span data-ttu-id="acf67-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="acf67-111">**Element**</span></span>|<span data-ttu-id="acf67-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="acf67-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="acf67-113">Name (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="acf67-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="acf67-114">メールボックスユーザーの名前を定義します。</span><span class="sxs-lookup"><span data-stu-id="acf67-114">Defines the name of the mailbox user.</span></span> <span data-ttu-id="acf67-115">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="acf67-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="acf67-116">EmailAddress (非 Emptystringtype)</span><span class="sxs-lookup"><span data-stu-id="acf67-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="acf67-117">メールボックスユーザーの簡易メール転送プロトコル (SMTP) アドレスを定義します。</span><span class="sxs-lookup"><span data-stu-id="acf67-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="acf67-118">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="acf67-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="acf67-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="acf67-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="acf67-120">メールボックスに使用されるルーティングを定義します。</span><span class="sxs-lookup"><span data-stu-id="acf67-120">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="acf67-121">既定値は SMTP です。</span><span class="sxs-lookup"><span data-stu-id="acf67-121">The default is SMTP.</span></span> <span data-ttu-id="acf67-122">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="acf67-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="acf67-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="acf67-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="acf67-124">メールボックスユーザーのメールボックスの種類を定義します。</span><span class="sxs-lookup"><span data-stu-id="acf67-124">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="acf67-125">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="acf67-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="acf67-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="acf67-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="acf67-127">ユーザーの連絡先フォルダーにある受信者の連絡先またはプライベート配布リストのアイテム識別子を定義します。</span><span class="sxs-lookup"><span data-stu-id="acf67-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="acf67-128">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="acf67-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="acf67-129">親要素</span><span class="sxs-lookup"><span data-stu-id="acf67-129">Parent elements</span></span>

|<span data-ttu-id="acf67-130">**要素**</span><span class="sxs-lookup"><span data-stu-id="acf67-130">**Element**</span></span>|<span data-ttu-id="acf67-131">**説明**</span><span class="sxs-lookup"><span data-stu-id="acf67-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="acf67-132">OriginalRecipients</span><span class="sxs-lookup"><span data-stu-id="acf67-132">OriginalRecipients</span></span>](originalrecipients.md) <br/> |<span data-ttu-id="acf67-133">追跡対象メッセージの元の受信者を表す電子メールアドレスのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="acf67-133">Contains a collection of e-mail addresses that represent the original recipients of a tracked message.</span></span>  <br/> |
|[<span data-ttu-id="acf67-134">RoomLists</span><span class="sxs-lookup"><span data-stu-id="acf67-134">RoomLists</span></span>](roomlists.md) <br/> |<span data-ttu-id="acf67-135">組織内の会議室のリストが保存されています。</span><span class="sxs-lookup"><span data-stu-id="acf67-135">Contains a list of meeting rooms in an organization.</span></span>  <br/> |
|[<span data-ttu-id="acf67-136">住所</span><span class="sxs-lookup"><span data-stu-id="acf67-136">SentToAddresses</span></span>](senttoaddresses.md) <br/> |<span data-ttu-id="acf67-137">条件または例外を適用するために、受信メッセージが送信された電子メールアドレスの一覧が含まれます。</span><span class="sxs-lookup"><span data-stu-id="acf67-137">Contains a list of e-mail addresses that incoming messages have to have been sent to in order for the condition or exception to apply.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="acf67-138">テキスト値</span><span class="sxs-lookup"><span data-stu-id="acf67-138">Text value</span></span>

<span data-ttu-id="acf67-139">なし。</span><span class="sxs-lookup"><span data-stu-id="acf67-139">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="acf67-140">注釈</span><span class="sxs-lookup"><span data-stu-id="acf67-140">Remarks</span></span>

<span data-ttu-id="acf67-141">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="acf67-141">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="acf67-142">要素の情報</span><span class="sxs-lookup"><span data-stu-id="acf67-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="acf67-143">Namespace</span><span class="sxs-lookup"><span data-stu-id="acf67-143">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="acf67-144">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="acf67-144">Schema Name</span></span>  <br/> |<span data-ttu-id="acf67-145">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="acf67-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="acf67-146">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="acf67-146">Validation File</span></span>  <br/> |<span data-ttu-id="acf67-147">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="acf67-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="acf67-148">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="acf67-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="acf67-149">正しくない</span><span class="sxs-lookup"><span data-stu-id="acf67-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="acf67-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="acf67-150">See also</span></span>

- [<span data-ttu-id="acf67-151">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="acf67-151">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md) 
- [<span data-ttu-id="acf67-152">GetRoomLists 操作</span><span class="sxs-lookup"><span data-stu-id="acf67-152">GetRoomLists operation</span></span>](getroomlists-operation.md)
- [<span data-ttu-id="acf67-153">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="acf67-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

