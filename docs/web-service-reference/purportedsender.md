---
title: PurportedSender
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PurportedSender
api_type:
- schema
ms.assetid: eb7a54ec-2e48-4030-bbcf-50a31609691b
description: PurportedSender 要素には、申し立ての送信者の電子メール メッセージの連絡先の情報が含まれています。
ms.openlocfilehash: 1e5b74d60d824c06834cf988557ef64fb84d70c4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832937"
---
# <a name="purportedsender"></a><span data-ttu-id="9b8d8-103">PurportedSender</span><span class="sxs-lookup"><span data-stu-id="9b8d8-103">PurportedSender</span></span>

<span data-ttu-id="9b8d8-104">**PurportedSender**要素には、申し立ての送信者の電子メール メッセージの連絡先の情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9b8d8-104">The **PurportedSender** element contains contact information for the alleged sender of an e-mail message.</span></span> 
  
```XML
<PurportedSender>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</PurportedSender>
```

 <span data-ttu-id="9b8d8-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="9b8d8-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9b8d8-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9b8d8-106">Attributes and elements</span></span>

<span data-ttu-id="9b8d8-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9b8d8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9b8d8-108">属性</span><span class="sxs-lookup"><span data-stu-id="9b8d8-108">Attributes</span></span>

<span data-ttu-id="9b8d8-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9b8d8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9b8d8-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9b8d8-110">Child elements</span></span>

|<span data-ttu-id="9b8d8-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="9b8d8-111">**Element**</span></span>|<span data-ttu-id="9b8d8-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="9b8d8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9b8d8-113">名 (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="9b8d8-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="9b8d8-114">メールボックス ユーザーの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="9b8d8-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="9b8d8-115">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="9b8d8-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="9b8d8-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="9b8d8-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="9b8d8-117">メールボックスのユーザーの簡易メール転送プロトコル (SMTP) アドレスを定義します。</span><span class="sxs-lookup"><span data-stu-id="9b8d8-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="9b8d8-118">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="9b8d8-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="9b8d8-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="9b8d8-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="9b8d8-120">受信者のルーティング プロトコルを表します。</span><span class="sxs-lookup"><span data-stu-id="9b8d8-120">Represents the routing protocol for the recipient.</span></span> <span data-ttu-id="9b8d8-121">既定値は、SMTP です。</span><span class="sxs-lookup"><span data-stu-id="9b8d8-121">The default value is SMTP.</span></span> <span data-ttu-id="9b8d8-122">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="9b8d8-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="9b8d8-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="9b8d8-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="9b8d8-124">電子メール アドレスで表されるメールボックスの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="9b8d8-124">Represents the type of mailbox that is represented by the e-mail address..</span></span> <span data-ttu-id="9b8d8-125">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="9b8d8-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="9b8d8-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="9b8d8-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="9b8d8-127">ユーザーのアドレス帳フォルダーから受信者の連絡先または個人用配布リストの項目の識別子を定義します。</span><span class="sxs-lookup"><span data-stu-id="9b8d8-127">Defines the item identifier of a contact or private distribution list for recipients from a user's contacts folder.</span></span> <span data-ttu-id="9b8d8-128">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="9b8d8-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9b8d8-129">親要素</span><span class="sxs-lookup"><span data-stu-id="9b8d8-129">Parent elements</span></span>

|<span data-ttu-id="9b8d8-130">**要素**</span><span class="sxs-lookup"><span data-stu-id="9b8d8-130">**Element**</span></span>|<span data-ttu-id="9b8d8-131">**説明**</span><span class="sxs-lookup"><span data-stu-id="9b8d8-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9b8d8-132">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="9b8d8-132">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="9b8d8-133">検索するメッセージの種類の条件を指定します。</span><span class="sxs-lookup"><span data-stu-id="9b8d8-133">Specifies criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="9b8d8-134">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="9b8d8-134">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="9b8d8-135">[GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)で返される 1 つのメッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="9b8d8-135">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="9b8d8-136">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="9b8d8-136">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="9b8d8-137">[FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md)要素の 1 つのメッセージの結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9b8d8-137">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9b8d8-138">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9b8d8-138">Text value</span></span>

<span data-ttu-id="9b8d8-139">なし。</span><span class="sxs-lookup"><span data-stu-id="9b8d8-139">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9b8d8-140">備考</span><span class="sxs-lookup"><span data-stu-id="9b8d8-140">Remarks</span></span>

<span data-ttu-id="9b8d8-141">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9b8d8-141">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9b8d8-142">要素情報</span><span class="sxs-lookup"><span data-stu-id="9b8d8-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9b8d8-143">名前空間</span><span class="sxs-lookup"><span data-stu-id="9b8d8-143">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9b8d8-144">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9b8d8-144">Schema Name</span></span>  <br/> |<span data-ttu-id="9b8d8-145">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="9b8d8-145">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9b8d8-146">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9b8d8-146">Validation File</span></span>  <br/> |<span data-ttu-id="9b8d8-147">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9b8d8-147">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9b8d8-148">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9b8d8-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="9b8d8-149">False</span><span class="sxs-lookup"><span data-stu-id="9b8d8-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9b8d8-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="9b8d8-150">See also</span></span>



[<span data-ttu-id="9b8d8-151">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="9b8d8-151">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="9b8d8-152">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="9b8d8-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

