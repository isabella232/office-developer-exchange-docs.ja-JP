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
description: PurportedSender 要素には、電子メールメッセージの申し立て sender の連絡先情報が含まれています。
ms.openlocfilehash: 5ecf352484a423e3955736620bf5a65c4e98099a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468335"
---
# <a name="purportedsender"></a><span data-ttu-id="4e0ad-103">PurportedSender</span><span class="sxs-lookup"><span data-stu-id="4e0ad-103">PurportedSender</span></span>

<span data-ttu-id="4e0ad-104">**PurportedSender**要素には、電子メールメッセージの申し立て sender の連絡先情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="4e0ad-104">The **PurportedSender** element contains contact information for the alleged sender of an e-mail message.</span></span> 
  
```XML
<PurportedSender>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</PurportedSender>
```

 <span data-ttu-id="4e0ad-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="4e0ad-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4e0ad-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="4e0ad-106">Attributes and elements</span></span>

<span data-ttu-id="4e0ad-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4e0ad-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4e0ad-108">属性</span><span class="sxs-lookup"><span data-stu-id="4e0ad-108">Attributes</span></span>

<span data-ttu-id="4e0ad-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4e0ad-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4e0ad-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4e0ad-110">Child elements</span></span>

|<span data-ttu-id="4e0ad-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="4e0ad-111">**Element**</span></span>|<span data-ttu-id="4e0ad-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="4e0ad-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4e0ad-113">Name (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="4e0ad-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="4e0ad-114">メールボックスユーザーの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="4e0ad-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="4e0ad-115">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="4e0ad-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="4e0ad-116">EmailAddress (非 Emptystringtype)</span><span class="sxs-lookup"><span data-stu-id="4e0ad-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="4e0ad-117">メールボックスユーザーの簡易メール転送プロトコル (SMTP) アドレスを定義します。</span><span class="sxs-lookup"><span data-stu-id="4e0ad-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="4e0ad-118">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="4e0ad-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="4e0ad-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="4e0ad-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="4e0ad-120">受信者のルーティングプロトコルを表します。</span><span class="sxs-lookup"><span data-stu-id="4e0ad-120">Represents the routing protocol for the recipient.</span></span> <span data-ttu-id="4e0ad-121">既定値は SMTP です。</span><span class="sxs-lookup"><span data-stu-id="4e0ad-121">The default value is SMTP.</span></span> <span data-ttu-id="4e0ad-122">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="4e0ad-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="4e0ad-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="4e0ad-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="4e0ad-124">電子メールアドレスによって表されるメールボックスの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="4e0ad-124">Represents the type of mailbox that is represented by the e-mail address..</span></span> <span data-ttu-id="4e0ad-125">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="4e0ad-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="4e0ad-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="4e0ad-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="4e0ad-127">ユーザーの連絡先フォルダーにある受信者の連絡先またはプライベート配布リストのアイテム識別子を定義します。</span><span class="sxs-lookup"><span data-stu-id="4e0ad-127">Defines the item identifier of a contact or private distribution list for recipients from a user's contacts folder.</span></span> <span data-ttu-id="4e0ad-128">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="4e0ad-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4e0ad-129">親要素</span><span class="sxs-lookup"><span data-stu-id="4e0ad-129">Parent elements</span></span>

|<span data-ttu-id="4e0ad-130">**要素**</span><span class="sxs-lookup"><span data-stu-id="4e0ad-130">**Element**</span></span>|<span data-ttu-id="4e0ad-131">**説明**</span><span class="sxs-lookup"><span data-stu-id="4e0ad-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4e0ad-132">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="4e0ad-132">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="4e0ad-133">検索するメッセージの種類の条件を指定します。</span><span class="sxs-lookup"><span data-stu-id="4e0ad-133">Specifies criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="4e0ad-134">および search-messagetrackingreport</span><span class="sxs-lookup"><span data-stu-id="4e0ad-134">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="4e0ad-135">[Getmessagetrackingreport 操作](getmessagetrackingreport-operation.md)で返される1つのメッセージを格納します。</span><span class="sxs-lookup"><span data-stu-id="4e0ad-135">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="4e0ad-136">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="4e0ad-136">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="4e0ad-137">[Findmessagetrackingreportresponse](findmessagetrackingreportresponse.md)要素の単一メッセージ結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="4e0ad-137">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4e0ad-138">テキスト値</span><span class="sxs-lookup"><span data-stu-id="4e0ad-138">Text value</span></span>

<span data-ttu-id="4e0ad-139">なし。</span><span class="sxs-lookup"><span data-stu-id="4e0ad-139">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4e0ad-140">注釈</span><span class="sxs-lookup"><span data-stu-id="4e0ad-140">Remarks</span></span>

<span data-ttu-id="4e0ad-141">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="4e0ad-141">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4e0ad-142">要素の情報</span><span class="sxs-lookup"><span data-stu-id="4e0ad-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4e0ad-143">Namespace</span><span class="sxs-lookup"><span data-stu-id="4e0ad-143">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4e0ad-144">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4e0ad-144">Schema Name</span></span>  <br/> |<span data-ttu-id="4e0ad-145">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="4e0ad-145">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4e0ad-146">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4e0ad-146">Validation File</span></span>  <br/> |<span data-ttu-id="4e0ad-147">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="4e0ad-147">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4e0ad-148">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4e0ad-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="4e0ad-149">正しくない</span><span class="sxs-lookup"><span data-stu-id="4e0ad-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4e0ad-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="4e0ad-150">See also</span></span>



[<span data-ttu-id="4e0ad-151">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="4e0ad-151">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="4e0ad-152">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="4e0ad-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

