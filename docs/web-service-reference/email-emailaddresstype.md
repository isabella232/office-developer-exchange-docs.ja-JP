---
title: 電子メール (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Email
api_type:
- schema
ms.assetid: dfffa1d5-2c3c-4f56-af63-5853df462e58
description: Email 要素は、GetUserAvailability クエリのメールボックスのユーザーを表します。
ms.openlocfilehash: 0e7848d7c4f5001ed86b06d11af1d7623b4bf1f0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760211"
---
# <a name="email-emailaddresstype"></a><span data-ttu-id="5cfbc-103">電子メール (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="5cfbc-103">Email (EmailAddressType)</span></span>

<span data-ttu-id="5cfbc-104">**Email**要素は、GetUserAvailability クエリのメールボックスのユーザーを表します。</span><span class="sxs-lookup"><span data-stu-id="5cfbc-104">The **Email** element represents the mailbox user for a GetUserAvailability query.</span></span> 
  
- [<span data-ttu-id="5cfbc-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="5cfbc-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)  
- [<span data-ttu-id="5cfbc-106">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="5cfbc-106">MailboxDataArray</span></span>](mailboxdataarray.md) 
- [<span data-ttu-id="5cfbc-107">MailboxData</span><span class="sxs-lookup"><span data-stu-id="5cfbc-107">MailboxData</span></span>](mailboxdata.md) 
- [<span data-ttu-id="5cfbc-108">電子メール (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="5cfbc-108">Email (EmailAddressType)</span></span>](email-emailaddresstype.md)
  
```xml
<Email>
   <Name>...</Name>
   <Address>...</Address>
   <RoutingType>...</RoutingType>
</Email>
```

 <span data-ttu-id="5cfbc-109">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="5cfbc-109">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5cfbc-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5cfbc-110">Attributes and elements</span></span>

<span data-ttu-id="5cfbc-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5cfbc-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5cfbc-112">属性</span><span class="sxs-lookup"><span data-stu-id="5cfbc-112">Attributes</span></span>

<span data-ttu-id="5cfbc-113">なし。</span><span class="sxs-lookup"><span data-stu-id="5cfbc-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5cfbc-114">子要素</span><span class="sxs-lookup"><span data-stu-id="5cfbc-114">Child elements</span></span>

|<span data-ttu-id="5cfbc-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="5cfbc-115">**Element**</span></span>|<span data-ttu-id="5cfbc-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="5cfbc-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5cfbc-117">名 (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="5cfbc-117">Name (EmailAddress)</span></span>](name-emailaddress.md) <br/> |<span data-ttu-id="5cfbc-118">メールボックス ユーザーの表示名を表します。</span><span class="sxs-lookup"><span data-stu-id="5cfbc-118">Represents the display name of the mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="5cfbc-119">アドレス (文字列)</span><span class="sxs-lookup"><span data-stu-id="5cfbc-119">Address (string)</span></span>](address-string.md) <br/> |<span data-ttu-id="5cfbc-120">メールボックス ユーザーの電子メール アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="5cfbc-120">Represents the e-mail address of the mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="5cfbc-121">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="5cfbc-121">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="5cfbc-122">メッセージのルーティング プロトコルを表します。</span><span class="sxs-lookup"><span data-stu-id="5cfbc-122">Represents the routing protocol for the message.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5cfbc-123">親要素</span><span class="sxs-lookup"><span data-stu-id="5cfbc-123">Parent elements</span></span>

|<span data-ttu-id="5cfbc-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="5cfbc-124">**Element**</span></span>|<span data-ttu-id="5cfbc-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="5cfbc-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5cfbc-126">MailboxData</span><span class="sxs-lookup"><span data-stu-id="5cfbc-126">MailboxData</span></span>](mailboxdata.md) <br/> |<span data-ttu-id="5cfbc-127">個々 のメールボックス ユーザーのメールボックスのユーザーに返されるデータの種類のオプションを表します。</span><span class="sxs-lookup"><span data-stu-id="5cfbc-127">Represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span>  <br/> <span data-ttu-id="5cfbc-128">以下は、この要素の XPath です。</span><span class="sxs-lookup"><span data-stu-id="5cfbc-128">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]/MailboxData` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5cfbc-129">備考</span><span class="sxs-lookup"><span data-stu-id="5cfbc-129">Remarks</span></span>

<span data-ttu-id="5cfbc-130">この要素を記述するスキーマは、インストールされているクライアント アクセス サーバーの役割を持つ MicrosoftExchange Server 2007 を実行しているコンピューターの/EWS/ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="5cfbc-130">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5cfbc-131">要素情報</span><span class="sxs-lookup"><span data-stu-id="5cfbc-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5cfbc-132">名前空間</span><span class="sxs-lookup"><span data-stu-id="5cfbc-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5cfbc-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5cfbc-133">Schema Name</span></span>  <br/> |<span data-ttu-id="5cfbc-134">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="5cfbc-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="5cfbc-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5cfbc-135">Validation File</span></span>  <br/> |<span data-ttu-id="5cfbc-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5cfbc-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5cfbc-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5cfbc-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="5cfbc-138">False</span><span class="sxs-lookup"><span data-stu-id="5cfbc-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5cfbc-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="5cfbc-139">See also</span></span>

- [<span data-ttu-id="5cfbc-140">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="5cfbc-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)  
- [<span data-ttu-id="5cfbc-141">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="5cfbc-141">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="5cfbc-142">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="5cfbc-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

