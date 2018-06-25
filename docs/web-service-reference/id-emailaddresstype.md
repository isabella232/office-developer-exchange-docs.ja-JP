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
ms.openlocfilehash: 5cd62f6f4e5912d2ecccda352be15c6a3b24e06c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831847"
---
# <a name="id-emailaddresstype"></a><span data-ttu-id="9c95f-103">Id (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="9c95f-103">Id (EmailAddressType)</span></span>

<span data-ttu-id="9c95f-104">**Id**要素は、Exchange server 組織内の会議室を識別します。</span><span class="sxs-lookup"><span data-stu-id="9c95f-104">The **Id** element identifies a meeting room within the Exchange server organization.</span></span> 
  
[<span data-ttu-id="9c95f-105">ルーム</span><span class="sxs-lookup"><span data-stu-id="9c95f-105">Room</span></span>](room.md)
  
[<span data-ttu-id="9c95f-106">Id (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="9c95f-106">Id (EmailAddressType)</span></span>](id-emailaddresstype.md)
  
```xml
<Id>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Id>
```

 <span data-ttu-id="9c95f-107">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="9c95f-107">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9c95f-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9c95f-108">Attributes and elements</span></span>

<span data-ttu-id="9c95f-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9c95f-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9c95f-110">属性</span><span class="sxs-lookup"><span data-stu-id="9c95f-110">Attributes</span></span>

<span data-ttu-id="9c95f-111">なし。</span><span class="sxs-lookup"><span data-stu-id="9c95f-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9c95f-112">子要素</span><span class="sxs-lookup"><span data-stu-id="9c95f-112">Child elements</span></span>

|<span data-ttu-id="9c95f-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="9c95f-113">**Element**</span></span>|<span data-ttu-id="9c95f-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="9c95f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9c95f-115">名 (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="9c95f-115">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="9c95f-116">会議室の名前を定義します。</span><span class="sxs-lookup"><span data-stu-id="9c95f-116">Defines the name of the meeting room.</span></span> <span data-ttu-id="9c95f-117">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="9c95f-117">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="9c95f-118">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="9c95f-118">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="9c95f-119">会議室の簡易メール転送プロトコル (SMTP) アドレスを定義します。</span><span class="sxs-lookup"><span data-stu-id="9c95f-119">Defines the Simple Mail Transfer Protocol (SMTP) address of a meeting room.</span></span> <span data-ttu-id="9c95f-120">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="9c95f-120">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="9c95f-121">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="9c95f-121">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="9c95f-122">メールボックスに使用されるルーティングを定義します。</span><span class="sxs-lookup"><span data-stu-id="9c95f-122">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="9c95f-123">既定値は、SMTP です。</span><span class="sxs-lookup"><span data-stu-id="9c95f-123">The default is SMTP.</span></span> <span data-ttu-id="9c95f-124">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="9c95f-124">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="9c95f-125">MailboxType</span><span class="sxs-lookup"><span data-stu-id="9c95f-125">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="9c95f-126">メールボックスのユーザーのメールボックスの種類を定義します。</span><span class="sxs-lookup"><span data-stu-id="9c95f-126">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="9c95f-127">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="9c95f-127">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="9c95f-128">ItemId</span><span class="sxs-lookup"><span data-stu-id="9c95f-128">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="9c95f-129">ユーザーのアドレス帳フォルダーから受信者の連絡先または個人用配布リストの項目の識別子を定義します。</span><span class="sxs-lookup"><span data-stu-id="9c95f-129">Defines the item identifier of a contact or private distribution list for recipients from a user's contacts folder.</span></span> <span data-ttu-id="9c95f-130">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="9c95f-130">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9c95f-131">親要素</span><span class="sxs-lookup"><span data-stu-id="9c95f-131">Parent elements</span></span>

|<span data-ttu-id="9c95f-132">**要素**</span><span class="sxs-lookup"><span data-stu-id="9c95f-132">**Element**</span></span>|<span data-ttu-id="9c95f-133">**説明**</span><span class="sxs-lookup"><span data-stu-id="9c95f-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9c95f-134">ルーム</span><span class="sxs-lookup"><span data-stu-id="9c95f-134">Room</span></span>](room.md) <br/> |<span data-ttu-id="9c95f-135">Exchange server 組織内の会議室を定義します。</span><span class="sxs-lookup"><span data-stu-id="9c95f-135">Defines a meeting room in the Exchange server organization.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9c95f-136">備考</span><span class="sxs-lookup"><span data-stu-id="9c95f-136">Remarks</span></span>

<span data-ttu-id="9c95f-137">この要素を記述するスキーマは、EWS のディレクトリにあるクライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターです。</span><span class="sxs-lookup"><span data-stu-id="9c95f-137">The schema that describes this element is located in the EWS directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9c95f-138">要素情報</span><span class="sxs-lookup"><span data-stu-id="9c95f-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9c95f-139">名前空間</span><span class="sxs-lookup"><span data-stu-id="9c95f-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9c95f-140">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9c95f-140">Schema Name</span></span>  <br/> |<span data-ttu-id="9c95f-141">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="9c95f-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="9c95f-142">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9c95f-142">Validation File</span></span>  <br/> |<span data-ttu-id="9c95f-143">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9c95f-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9c95f-144">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9c95f-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="9c95f-145">False</span><span class="sxs-lookup"><span data-stu-id="9c95f-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9c95f-146">関連項目</span><span class="sxs-lookup"><span data-stu-id="9c95f-146">See also</span></span>



[<span data-ttu-id="9c95f-147">GetRooms 操作</span><span class="sxs-lookup"><span data-stu-id="9c95f-147">GetRooms operation</span></span>](getrooms-operation.md)


- [<span data-ttu-id="9c95f-148">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="9c95f-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

