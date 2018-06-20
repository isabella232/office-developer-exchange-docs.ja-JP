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
description: RecipientFilter 要素は、指定したメッセージ追跡レポートを使用する受信者のアドレスを表します。
ms.openlocfilehash: c31ed469132b110a690416b112d5e4e96e44c501
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832972"
---
# <a name="recipientfilter"></a><span data-ttu-id="11bcf-103">RecipientFilter</span><span class="sxs-lookup"><span data-stu-id="11bcf-103">RecipientFilter</span></span>

<span data-ttu-id="11bcf-104">**RecipientFilter**要素は、指定したメッセージ追跡レポートを使用する受信者のアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="11bcf-104">The **RecipientFilter** element represents a recipient address to use with the specified message tracking report.</span></span> 
  
```XML
 <RecipientFilter>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</RecipientFilter>
```

 <span data-ttu-id="11bcf-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="11bcf-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="11bcf-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="11bcf-106">Attributes and elements</span></span>

<span data-ttu-id="11bcf-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="11bcf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="11bcf-108">属性</span><span class="sxs-lookup"><span data-stu-id="11bcf-108">Attributes</span></span>

<span data-ttu-id="11bcf-109">なし。</span><span class="sxs-lookup"><span data-stu-id="11bcf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="11bcf-110">子要素</span><span class="sxs-lookup"><span data-stu-id="11bcf-110">Child elements</span></span>

|<span data-ttu-id="11bcf-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="11bcf-111">**Element**</span></span>|<span data-ttu-id="11bcf-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="11bcf-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="11bcf-113">名 (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="11bcf-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="11bcf-114">メールボックス ユーザーの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="11bcf-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="11bcf-115">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="11bcf-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="11bcf-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="11bcf-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="11bcf-117">メールボックスのユーザーのプライマリ簡易メール転送プロトコル (SMTP) アドレスを定義します。</span><span class="sxs-lookup"><span data-stu-id="11bcf-117">Defines the primary Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="11bcf-118">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="11bcf-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="11bcf-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="11bcf-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="11bcf-120">この受信者へのルーティング プロトコルを表します。</span><span class="sxs-lookup"><span data-stu-id="11bcf-120">Represents the routing protocol for this recipient.</span></span> <span data-ttu-id="11bcf-121">既定値は、SMTP です。</span><span class="sxs-lookup"><span data-stu-id="11bcf-121">The default value is SMTP.</span></span> <span data-ttu-id="11bcf-122">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="11bcf-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="11bcf-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="11bcf-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="11bcf-124">電子メール アドレスで表されるメールボックスの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="11bcf-124">Represents the type of mailbox that is represented by the e-mail address.</span></span> <span data-ttu-id="11bcf-125">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="11bcf-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="11bcf-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="11bcf-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="11bcf-127">ユーザーのアドレス帳フォルダーから受信者の連絡先または個人用配布リストの項目の識別子を定義します。</span><span class="sxs-lookup"><span data-stu-id="11bcf-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="11bcf-128">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="11bcf-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="11bcf-129">親要素</span><span class="sxs-lookup"><span data-stu-id="11bcf-129">Parent elements</span></span>

|<span data-ttu-id="11bcf-130">**要素**</span><span class="sxs-lookup"><span data-stu-id="11bcf-130">**Element**</span></span>|<span data-ttu-id="11bcf-131">**説明**</span><span class="sxs-lookup"><span data-stu-id="11bcf-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="11bcf-132">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="11bcf-132">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="11bcf-133">レポートを指定した ID の追跡を取得するために[GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)の要求が含まれています</span><span class="sxs-lookup"><span data-stu-id="11bcf-133">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="11bcf-134">テキスト値</span><span class="sxs-lookup"><span data-stu-id="11bcf-134">Text value</span></span>

<span data-ttu-id="11bcf-135">なし。</span><span class="sxs-lookup"><span data-stu-id="11bcf-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="11bcf-136">備考</span><span class="sxs-lookup"><span data-stu-id="11bcf-136">Remarks</span></span>

<span data-ttu-id="11bcf-137">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="11bcf-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="11bcf-138">要素情報</span><span class="sxs-lookup"><span data-stu-id="11bcf-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="11bcf-139">名前空間</span><span class="sxs-lookup"><span data-stu-id="11bcf-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="11bcf-140">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="11bcf-140">Schema Name</span></span>  <br/> |<span data-ttu-id="11bcf-141">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="11bcf-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="11bcf-142">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="11bcf-142">Validation File</span></span>  <br/> |<span data-ttu-id="11bcf-143">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="11bcf-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="11bcf-144">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="11bcf-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="11bcf-145">False</span><span class="sxs-lookup"><span data-stu-id="11bcf-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="11bcf-146">関連項目</span><span class="sxs-lookup"><span data-stu-id="11bcf-146">See also</span></span>



[<span data-ttu-id="11bcf-147">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="11bcf-147">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="11bcf-148">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="11bcf-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

