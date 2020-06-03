---
title: RoomList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RoomList
api_type:
- schema
ms.assetid: cb02bdf0-df9f-4e31-b7dd-cd9f2f2cc2b2
description: RoomList 要素は、会議室の一覧を識別する電子メールアドレスを表します。
ms.openlocfilehash: 0444475cb9fffbb89ba2861096baee0c7e645995
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460520"
---
# <a name="roomlist"></a><span data-ttu-id="1e3db-103">RoomList</span><span class="sxs-lookup"><span data-stu-id="1e3db-103">RoomList</span></span>

<span data-ttu-id="1e3db-104">**RoomList**要素は、会議室の一覧を識別する電子メールアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="1e3db-104">The **RoomList** element represents an e-mail address that identifies a list of meeting rooms.</span></span> 
  
[<span data-ttu-id="1e3db-105">GetRooms</span><span class="sxs-lookup"><span data-stu-id="1e3db-105">GetRooms</span></span>](getrooms.md)
  
[<span data-ttu-id="1e3db-106">RoomList</span><span class="sxs-lookup"><span data-stu-id="1e3db-106">RoomList</span></span>](roomlist.md)
  
```XML
<RoomList>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</RoomList>
```

 <span data-ttu-id="1e3db-107">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="1e3db-107">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1e3db-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1e3db-108">Attributes and elements</span></span>

<span data-ttu-id="1e3db-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1e3db-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1e3db-110">属性</span><span class="sxs-lookup"><span data-stu-id="1e3db-110">Attributes</span></span>

<span data-ttu-id="1e3db-111">なし。</span><span class="sxs-lookup"><span data-stu-id="1e3db-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1e3db-112">子要素</span><span class="sxs-lookup"><span data-stu-id="1e3db-112">Child elements</span></span>

|<span data-ttu-id="1e3db-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="1e3db-113">**Element**</span></span>|<span data-ttu-id="1e3db-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="1e3db-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1e3db-115">Name (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="1e3db-115">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="1e3db-116">会議室一覧の表示名を定義します。</span><span class="sxs-lookup"><span data-stu-id="1e3db-116">Defines the display name of the room list.</span></span> <span data-ttu-id="1e3db-117">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="1e3db-117">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="1e3db-118">EmailAddress (非 Emptystringtype)</span><span class="sxs-lookup"><span data-stu-id="1e3db-118">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="1e3db-119">会議室一覧の簡易メール転送プロトコル (SMTP) アドレスを定義します。</span><span class="sxs-lookup"><span data-stu-id="1e3db-119">Defines the Simple Mail Transfer Protocol (SMTP) address of a room list.</span></span> <span data-ttu-id="1e3db-120">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="1e3db-120">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="1e3db-121">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="1e3db-121">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="1e3db-122">メールボックスに使用されるルーティングを定義します。</span><span class="sxs-lookup"><span data-stu-id="1e3db-122">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="1e3db-123">既定値は SMTP です。</span><span class="sxs-lookup"><span data-stu-id="1e3db-123">The default is SMTP.</span></span> <span data-ttu-id="1e3db-124">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="1e3db-124">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="1e3db-125">MailboxType</span><span class="sxs-lookup"><span data-stu-id="1e3db-125">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="1e3db-126">メールボックスユーザーのメールボックスの種類を定義します。</span><span class="sxs-lookup"><span data-stu-id="1e3db-126">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="1e3db-127">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="1e3db-127">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="1e3db-128">ItemId</span><span class="sxs-lookup"><span data-stu-id="1e3db-128">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="1e3db-129">ユーザーの連絡先フォルダーにある受信者の連絡先またはプライベート配布リストのアイテム識別子を定義します。</span><span class="sxs-lookup"><span data-stu-id="1e3db-129">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="1e3db-130">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="1e3db-130">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1e3db-131">親要素</span><span class="sxs-lookup"><span data-stu-id="1e3db-131">Parent elements</span></span>

|<span data-ttu-id="1e3db-132">**要素**</span><span class="sxs-lookup"><span data-stu-id="1e3db-132">**Element**</span></span>|<span data-ttu-id="1e3db-133">**説明**</span><span class="sxs-lookup"><span data-stu-id="1e3db-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1e3db-134">GetRooms</span><span class="sxs-lookup"><span data-stu-id="1e3db-134">GetRooms</span></span>](getrooms.md) <br/> |<span data-ttu-id="1e3db-135">特定の会議室リスト内のルームのリストを取得する要求のルート要素。</span><span class="sxs-lookup"><span data-stu-id="1e3db-135">The root element in a request to get a list of rooms within a particular room list.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1e3db-136">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1e3db-136">Text value</span></span>

<span data-ttu-id="1e3db-137">なし。</span><span class="sxs-lookup"><span data-stu-id="1e3db-137">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1e3db-138">注釈</span><span class="sxs-lookup"><span data-stu-id="1e3db-138">Remarks</span></span>

<span data-ttu-id="1e3db-139">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="1e3db-139">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1e3db-140">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1e3db-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1e3db-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="1e3db-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1e3db-142">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1e3db-142">Schema Name</span></span>  <br/> |<span data-ttu-id="1e3db-143">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="1e3db-143">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1e3db-144">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1e3db-144">Validation File</span></span>  <br/> |<span data-ttu-id="1e3db-145">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="1e3db-145">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1e3db-146">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1e3db-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="1e3db-147">正しくない</span><span class="sxs-lookup"><span data-stu-id="1e3db-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1e3db-148">関連項目</span><span class="sxs-lookup"><span data-stu-id="1e3db-148">See also</span></span>



[<span data-ttu-id="1e3db-149">GetRooms 操作</span><span class="sxs-lookup"><span data-stu-id="1e3db-149">GetRooms operation</span></span>](getrooms-operation.md)


- [<span data-ttu-id="1e3db-150">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="1e3db-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

