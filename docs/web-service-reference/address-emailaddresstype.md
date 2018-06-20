---
title: アドレス (EmailAddressType)
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
description: アドレス要素は、完全に解決された電子メール アドレスを表します。
ms.openlocfilehash: 2a2d409edcc3a04bf82c6da0080183becfc9b25b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759365"
---
# <a name="address-emailaddresstype"></a><span data-ttu-id="45828-103">アドレス (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="45828-103">Address (EmailAddressType)</span></span>

<span data-ttu-id="45828-104">**アドレス**要素は、完全に解決された電子メール アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="45828-104">The **Address** element represents a fully resolved e-mail address.</span></span> 
  
```XML
<Address>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Address >
```

 <span data-ttu-id="45828-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="45828-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="45828-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="45828-106">Attributes and elements</span></span>

<span data-ttu-id="45828-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="45828-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="45828-108">属性</span><span class="sxs-lookup"><span data-stu-id="45828-108">Attributes</span></span>

<span data-ttu-id="45828-109">なし。</span><span class="sxs-lookup"><span data-stu-id="45828-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="45828-110">子要素</span><span class="sxs-lookup"><span data-stu-id="45828-110">Child elements</span></span>

|<span data-ttu-id="45828-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="45828-111">**Element**</span></span>|<span data-ttu-id="45828-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="45828-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="45828-113">名 (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="45828-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="45828-114">メールボックス ユーザーの名前を定義します。</span><span class="sxs-lookup"><span data-stu-id="45828-114">Defines the name of the mailbox user.</span></span> <span data-ttu-id="45828-115">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="45828-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="45828-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="45828-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="45828-117">メールボックスのユーザーの簡易メール転送プロトコル (SMTP) アドレスを定義します。</span><span class="sxs-lookup"><span data-stu-id="45828-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="45828-118">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="45828-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="45828-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="45828-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="45828-120">メールボックスに使用されるルーティングを定義します。</span><span class="sxs-lookup"><span data-stu-id="45828-120">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="45828-121">既定値は、SMTP です。</span><span class="sxs-lookup"><span data-stu-id="45828-121">The default is SMTP.</span></span> <span data-ttu-id="45828-122">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="45828-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="45828-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="45828-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="45828-124">メールボックスのユーザーのメールボックスの種類を定義します。</span><span class="sxs-lookup"><span data-stu-id="45828-124">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="45828-125">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="45828-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="45828-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="45828-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="45828-127">ユーザーのアドレス帳フォルダーから受信者の連絡先または個人用配布リストの項目の識別子を定義します。</span><span class="sxs-lookup"><span data-stu-id="45828-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="45828-128">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="45828-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="45828-129">親要素</span><span class="sxs-lookup"><span data-stu-id="45828-129">Parent elements</span></span>

|<span data-ttu-id="45828-130">**要素**</span><span class="sxs-lookup"><span data-stu-id="45828-130">**Element**</span></span>|<span data-ttu-id="45828-131">**説明**</span><span class="sxs-lookup"><span data-stu-id="45828-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="45828-132">OriginalRecipients</span><span class="sxs-lookup"><span data-stu-id="45828-132">OriginalRecipients</span></span>](originalrecipients.md) <br/> |<span data-ttu-id="45828-133">追跡対象のメッセージの元の受信者を表すための電子メール アドレスのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="45828-133">Contains a collection of e-mail addresses that represent the original recipients of a tracked message.</span></span>  <br/> |
|[<span data-ttu-id="45828-134">RoomLists</span><span class="sxs-lookup"><span data-stu-id="45828-134">RoomLists</span></span>](roomlists.md) <br/> |<span data-ttu-id="45828-135">会議室、組織内の一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="45828-135">Contains a list of meeting rooms in an organization.</span></span>  <br/> |
|[<span data-ttu-id="45828-136">SentToAddresses</span><span class="sxs-lookup"><span data-stu-id="45828-136">SentToAddresses</span></span>](senttoaddresses.md) <br/> |<span data-ttu-id="45828-137">適用する条件または例外の順序でに送信されている受信メッセージを持つ電子メール アドレスの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="45828-137">Contains a list of e-mail addresses that incoming messages have to have been sent to in order for the condition or exception to apply.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="45828-138">テキスト値</span><span class="sxs-lookup"><span data-stu-id="45828-138">Text value</span></span>

<span data-ttu-id="45828-139">なし。</span><span class="sxs-lookup"><span data-stu-id="45828-139">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="45828-140">備考</span><span class="sxs-lookup"><span data-stu-id="45828-140">Remarks</span></span>

<span data-ttu-id="45828-141">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="45828-141">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="45828-142">要素情報</span><span class="sxs-lookup"><span data-stu-id="45828-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="45828-143">名前空間</span><span class="sxs-lookup"><span data-stu-id="45828-143">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="45828-144">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="45828-144">Schema Name</span></span>  <br/> |<span data-ttu-id="45828-145">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="45828-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="45828-146">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="45828-146">Validation File</span></span>  <br/> |<span data-ttu-id="45828-147">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="45828-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="45828-148">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="45828-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="45828-149">False</span><span class="sxs-lookup"><span data-stu-id="45828-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="45828-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="45828-150">See also</span></span>

- [<span data-ttu-id="45828-151">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="45828-151">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md) 
- [<span data-ttu-id="45828-152">GetRoomLists 操作</span><span class="sxs-lookup"><span data-stu-id="45828-152">GetRoomLists operation</span></span>](getroomlists-operation.md)
- [<span data-ttu-id="45828-153">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="45828-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

