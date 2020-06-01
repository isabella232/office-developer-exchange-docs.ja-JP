---
title: Id (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Id
api_type:
- schema
ms.assetid: 3e1e37b5-5469-4447-ad1f-c2c6d4e0482f
description: Id 要素は、Exchange server 組織内の会議室を識別します。
ms.openlocfilehash: aa09e7764746ac6bc283de2d13248d769aba75b7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460779"
---
# <a name="id-emailaddresstype"></a><span data-ttu-id="52457-103">Id (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="52457-103">Id (EmailAddressType)</span></span>

<span data-ttu-id="52457-104">**Id**要素は、Exchange server 組織内の会議室を識別します。</span><span class="sxs-lookup"><span data-stu-id="52457-104">The **Id** element identifies a meeting room within the Exchange server organization.</span></span> 
  
[<span data-ttu-id="52457-105">作る</span><span class="sxs-lookup"><span data-stu-id="52457-105">Room</span></span>](room.md)
  
[<span data-ttu-id="52457-106">Id (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="52457-106">Id (EmailAddressType)</span></span>](id-emailaddresstype.md)
  
```xml
<Id>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Id>
```

 <span data-ttu-id="52457-107">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="52457-107">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="52457-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="52457-108">Attributes and elements</span></span>

<span data-ttu-id="52457-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="52457-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="52457-110">属性</span><span class="sxs-lookup"><span data-stu-id="52457-110">Attributes</span></span>

<span data-ttu-id="52457-111">なし。</span><span class="sxs-lookup"><span data-stu-id="52457-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="52457-112">子要素</span><span class="sxs-lookup"><span data-stu-id="52457-112">Child elements</span></span>

|<span data-ttu-id="52457-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="52457-113">**Element**</span></span>|<span data-ttu-id="52457-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="52457-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="52457-115">Name (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="52457-115">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="52457-116">会議室の名前を定義します。</span><span class="sxs-lookup"><span data-stu-id="52457-116">Defines the name of the meeting room.</span></span> <span data-ttu-id="52457-117">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="52457-117">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="52457-118">EmailAddress (非 Emptystringtype)</span><span class="sxs-lookup"><span data-stu-id="52457-118">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="52457-119">会議室の簡易メール転送プロトコル (SMTP) アドレスを定義します。</span><span class="sxs-lookup"><span data-stu-id="52457-119">Defines the Simple Mail Transfer Protocol (SMTP) address of a meeting room.</span></span> <span data-ttu-id="52457-120">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="52457-120">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="52457-121">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="52457-121">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="52457-122">メールボックスに使用されるルーティングを定義します。</span><span class="sxs-lookup"><span data-stu-id="52457-122">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="52457-123">既定値は SMTP です。</span><span class="sxs-lookup"><span data-stu-id="52457-123">The default is SMTP.</span></span> <span data-ttu-id="52457-124">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="52457-124">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="52457-125">MailboxType</span><span class="sxs-lookup"><span data-stu-id="52457-125">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="52457-126">メールボックスユーザーのメールボックスの種類を定義します。</span><span class="sxs-lookup"><span data-stu-id="52457-126">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="52457-127">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="52457-127">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="52457-128">ItemId</span><span class="sxs-lookup"><span data-stu-id="52457-128">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="52457-129">ユーザーの連絡先フォルダーにある受信者の連絡先またはプライベート配布リストのアイテム識別子を定義します。</span><span class="sxs-lookup"><span data-stu-id="52457-129">Defines the item identifier of a contact or private distribution list for recipients from a user's contacts folder.</span></span> <span data-ttu-id="52457-130">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="52457-130">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="52457-131">親要素</span><span class="sxs-lookup"><span data-stu-id="52457-131">Parent elements</span></span>

|<span data-ttu-id="52457-132">**要素**</span><span class="sxs-lookup"><span data-stu-id="52457-132">**Element**</span></span>|<span data-ttu-id="52457-133">**説明**</span><span class="sxs-lookup"><span data-stu-id="52457-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="52457-134">作る</span><span class="sxs-lookup"><span data-stu-id="52457-134">Room</span></span>](room.md) <br/> |<span data-ttu-id="52457-135">Exchange server 組織の会議室を定義します。</span><span class="sxs-lookup"><span data-stu-id="52457-135">Defines a meeting room in the Exchange server organization.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="52457-136">注釈</span><span class="sxs-lookup"><span data-stu-id="52457-136">Remarks</span></span>

<span data-ttu-id="52457-137">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="52457-137">The schema that describes this element is located in the EWS directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="52457-138">要素の情報</span><span class="sxs-lookup"><span data-stu-id="52457-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="52457-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="52457-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="52457-140">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="52457-140">Schema Name</span></span>  <br/> |<span data-ttu-id="52457-141">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="52457-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="52457-142">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="52457-142">Validation File</span></span>  <br/> |<span data-ttu-id="52457-143">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="52457-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="52457-144">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="52457-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="52457-145">正しくない</span><span class="sxs-lookup"><span data-stu-id="52457-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="52457-146">関連項目</span><span class="sxs-lookup"><span data-stu-id="52457-146">See also</span></span>



[<span data-ttu-id="52457-147">GetRooms 操作</span><span class="sxs-lookup"><span data-stu-id="52457-147">GetRooms operation</span></span>](getrooms-operation.md)


- [<span data-ttu-id="52457-148">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="52457-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

