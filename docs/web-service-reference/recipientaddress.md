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
description: RecipientAddress 要素は、受信者のメールボックスを表します。
ms.openlocfilehash: 10928ac206227cfc21bd83ab5bfa9a55aad354e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832974"
---
# <a name="recipientaddress"></a><span data-ttu-id="3f7e0-103">RecipientAddress</span><span class="sxs-lookup"><span data-stu-id="3f7e0-103">RecipientAddress</span></span>

<span data-ttu-id="3f7e0-104">**RecipientAddress**要素は、受信者のメールボックスを表します。</span><span class="sxs-lookup"><span data-stu-id="3f7e0-104">The **RecipientAddress** element represents the mailbox of the recipient.</span></span> 
  
```xml
<RecipientAddress>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</RecipientAddress>
```

 <span data-ttu-id="3f7e0-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="3f7e0-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3f7e0-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="3f7e0-106">Attributes and elements</span></span>

<span data-ttu-id="3f7e0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3f7e0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3f7e0-108">属性</span><span class="sxs-lookup"><span data-stu-id="3f7e0-108">Attributes</span></span>

<span data-ttu-id="3f7e0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3f7e0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3f7e0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3f7e0-110">Child elements</span></span>

|<span data-ttu-id="3f7e0-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="3f7e0-111">**Element**</span></span>|<span data-ttu-id="3f7e0-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="3f7e0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3f7e0-113">名 (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="3f7e0-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="3f7e0-114">メールボックス ユーザーの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="3f7e0-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="3f7e0-115">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="3f7e0-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="3f7e0-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="3f7e0-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="3f7e0-117">メールボックスのユーザーの簡易メール転送プロトコル (SMTP) アドレスを定義します。</span><span class="sxs-lookup"><span data-stu-id="3f7e0-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="3f7e0-118">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="3f7e0-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="3f7e0-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="3f7e0-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="3f7e0-120">受信者のルーティング プロトコルを表します。</span><span class="sxs-lookup"><span data-stu-id="3f7e0-120">Represents the routing protocol for the recipient.</span></span> <span data-ttu-id="3f7e0-121">既定値は、SMTP です。</span><span class="sxs-lookup"><span data-stu-id="3f7e0-121">The default is SMTP.</span></span> <span data-ttu-id="3f7e0-122">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="3f7e0-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="3f7e0-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="3f7e0-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="3f7e0-124">電子メール アドレスで表されるメールボックスの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="3f7e0-124">Represents the type of mailbox that is represented by the e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="3f7e0-125">ItemId</span><span class="sxs-lookup"><span data-stu-id="3f7e0-125">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="3f7e0-126">ユーザーのアドレス帳フォルダーから受信者の連絡先または個人用配布リストの項目の識別子を定義します。</span><span class="sxs-lookup"><span data-stu-id="3f7e0-126">Defines the item identifier of a contact or private distribution list for recipients from a user's contacts folder.</span></span> <span data-ttu-id="3f7e0-127">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="3f7e0-127">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3f7e0-128">親要素</span><span class="sxs-lookup"><span data-stu-id="3f7e0-128">Parent elements</span></span>

|<span data-ttu-id="3f7e0-129">**要素**</span><span class="sxs-lookup"><span data-stu-id="3f7e0-129">**Element**</span></span>|<span data-ttu-id="3f7e0-130">**説明**</span><span class="sxs-lookup"><span data-stu-id="3f7e0-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3f7e0-131">メール ヒント</span><span class="sxs-lookup"><span data-stu-id="3f7e0-131">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="3f7e0-132">さまざまな種類のメール ヒントの値を表します。</span><span class="sxs-lookup"><span data-stu-id="3f7e0-132">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3f7e0-133">備考</span><span class="sxs-lookup"><span data-stu-id="3f7e0-133">Remarks</span></span>

<span data-ttu-id="3f7e0-134">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="3f7e0-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3f7e0-135">要素情報</span><span class="sxs-lookup"><span data-stu-id="3f7e0-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3f7e0-136">名前空間</span><span class="sxs-lookup"><span data-stu-id="3f7e0-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3f7e0-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3f7e0-137">Schema Name</span></span>  <br/> |<span data-ttu-id="3f7e0-138">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="3f7e0-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="3f7e0-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3f7e0-139">Validation File</span></span>  <br/> |<span data-ttu-id="3f7e0-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3f7e0-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3f7e0-141">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3f7e0-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="3f7e0-142">False</span><span class="sxs-lookup"><span data-stu-id="3f7e0-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3f7e0-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="3f7e0-143">See also</span></span>



- [<span data-ttu-id="3f7e0-144">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="3f7e0-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

