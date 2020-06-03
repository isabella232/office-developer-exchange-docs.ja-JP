---
title: Sender (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Sender
api_type:
- schema
ms.assetid: 717eb6d0-d167-4b20-92e2-5d08b96186c4
description: Sender 要素は、メッセージの送信者の電子メールアドレスを表します。
ms.openlocfilehash: 23a487f216a110796d40f3d3e86224c691acc004
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455325"
---
# <a name="sender-emailaddresstype"></a><span data-ttu-id="7f1fb-103">Sender (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="7f1fb-103">Sender (EmailAddressType)</span></span>

<span data-ttu-id="7f1fb-104">**Sender**要素は、メッセージの送信者の電子メールアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="7f1fb-104">The **Sender** element represents the e-mail address for the sender of the message.</span></span> 
  
```XML
<Sender>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Sender>
```

 <span data-ttu-id="7f1fb-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="7f1fb-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7f1fb-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7f1fb-106">Attributes and elements</span></span>

<span data-ttu-id="7f1fb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7f1fb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7f1fb-108">属性</span><span class="sxs-lookup"><span data-stu-id="7f1fb-108">Attributes</span></span>

<span data-ttu-id="7f1fb-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7f1fb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7f1fb-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7f1fb-110">Child elements</span></span>

|<span data-ttu-id="7f1fb-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="7f1fb-111">**Element**</span></span>|<span data-ttu-id="7f1fb-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="7f1fb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7f1fb-113">Name (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="7f1fb-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="7f1fb-114">メールボックスユーザーの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="7f1fb-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="7f1fb-115">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="7f1fb-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="7f1fb-116">EmailAddress (非 Emptystringtype)</span><span class="sxs-lookup"><span data-stu-id="7f1fb-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="7f1fb-117">メールボックスユーザーのプライマリ簡易メール転送プロトコル (SMTP) アドレスを定義します。</span><span class="sxs-lookup"><span data-stu-id="7f1fb-117">Defines the primary Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="7f1fb-118">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="7f1fb-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="7f1fb-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="7f1fb-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="7f1fb-120">受信者のルーティングプロトコルを表します。</span><span class="sxs-lookup"><span data-stu-id="7f1fb-120">Represents the routing protocol for the recipient.</span></span> <span data-ttu-id="7f1fb-121">既定値は SMTP です。</span><span class="sxs-lookup"><span data-stu-id="7f1fb-121">The default value is SMTP.</span></span> <span data-ttu-id="7f1fb-122">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="7f1fb-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="7f1fb-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="7f1fb-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="7f1fb-124">電子メールアドレスによって表されるメールボックスの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="7f1fb-124">Represents the type of mailbox that is represented by the e-mail address.</span></span> <span data-ttu-id="7f1fb-125">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="7f1fb-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="7f1fb-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="7f1fb-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="7f1fb-127">ユーザーの連絡先フォルダーにある受信者の連絡先またはプライベート配布リストのアイテム識別子を定義します。</span><span class="sxs-lookup"><span data-stu-id="7f1fb-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="7f1fb-128">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="7f1fb-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7f1fb-129">親要素</span><span class="sxs-lookup"><span data-stu-id="7f1fb-129">Parent elements</span></span>

|<span data-ttu-id="7f1fb-130">**要素**</span><span class="sxs-lookup"><span data-stu-id="7f1fb-130">**Element**</span></span>|<span data-ttu-id="7f1fb-131">**説明**</span><span class="sxs-lookup"><span data-stu-id="7f1fb-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7f1fb-132">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="7f1fb-132">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="7f1fb-133">検索するメッセージの種類の条件を指定します。</span><span class="sxs-lookup"><span data-stu-id="7f1fb-133">Specifies criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="7f1fb-134">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="7f1fb-134">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="7f1fb-135">[Findmessagetrackingreportresponse](findmessagetrackingreportresponse.md)要素の単一メッセージ結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="7f1fb-135">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
|[<span data-ttu-id="7f1fb-136">および search-messagetrackingreport</span><span class="sxs-lookup"><span data-stu-id="7f1fb-136">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="7f1fb-137">[Getmessagetrackingreport 操作](getmessagetrackingreport-operation.md)で返される1つのメッセージを格納します。</span><span class="sxs-lookup"><span data-stu-id="7f1fb-137">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7f1fb-138">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7f1fb-138">Text value</span></span>

<span data-ttu-id="7f1fb-139">なし。</span><span class="sxs-lookup"><span data-stu-id="7f1fb-139">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7f1fb-140">注釈</span><span class="sxs-lookup"><span data-stu-id="7f1fb-140">Remarks</span></span>

<span data-ttu-id="7f1fb-141">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7f1fb-141">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7f1fb-142">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7f1fb-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7f1fb-143">Namespace</span><span class="sxs-lookup"><span data-stu-id="7f1fb-143">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7f1fb-144">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7f1fb-144">Schema Name</span></span>  <br/> |<span data-ttu-id="7f1fb-145">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="7f1fb-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="7f1fb-146">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7f1fb-146">Validation File</span></span>  <br/> |<span data-ttu-id="7f1fb-147">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="7f1fb-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7f1fb-148">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7f1fb-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="7f1fb-149">正しくない</span><span class="sxs-lookup"><span data-stu-id="7f1fb-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7f1fb-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="7f1fb-150">See also</span></span>



[<span data-ttu-id="7f1fb-151">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="7f1fb-151">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="7f1fb-152">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="7f1fb-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

