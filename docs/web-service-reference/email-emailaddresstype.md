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
description: Email 要素は、GetUserAvailability クエリのメールボックスユーザーを表します。
ms.openlocfilehash: 2ed8de9c011a385ec6c4ebd2f8d1d47304343a0e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459231"
---
# <a name="email-emailaddresstype"></a><span data-ttu-id="506b7-103">電子メール (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="506b7-103">Email (EmailAddressType)</span></span>

<span data-ttu-id="506b7-104">**Email**要素は、getuseravailability クエリのメールボックスユーザーを表します。</span><span class="sxs-lookup"><span data-stu-id="506b7-104">The **Email** element represents the mailbox user for a GetUserAvailability query.</span></span> 
  
- [<span data-ttu-id="506b7-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="506b7-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)  
- [<span data-ttu-id="506b7-106">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="506b7-106">MailboxDataArray</span></span>](mailboxdataarray.md) 
- [<span data-ttu-id="506b7-107">MailboxData</span><span class="sxs-lookup"><span data-stu-id="506b7-107">MailboxData</span></span>](mailboxdata.md) 
- [<span data-ttu-id="506b7-108">電子メール (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="506b7-108">Email (EmailAddressType)</span></span>](email-emailaddresstype.md)
  
```xml
<Email>
   <Name>...</Name>
   <Address>...</Address>
   <RoutingType>...</RoutingType>
</Email>
```

 <span data-ttu-id="506b7-109">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="506b7-109">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="506b7-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="506b7-110">Attributes and elements</span></span>

<span data-ttu-id="506b7-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="506b7-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="506b7-112">属性</span><span class="sxs-lookup"><span data-stu-id="506b7-112">Attributes</span></span>

<span data-ttu-id="506b7-113">なし。</span><span class="sxs-lookup"><span data-stu-id="506b7-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="506b7-114">子要素</span><span class="sxs-lookup"><span data-stu-id="506b7-114">Child elements</span></span>

|<span data-ttu-id="506b7-115">**Element**</span><span class="sxs-lookup"><span data-stu-id="506b7-115">**Element**</span></span>|<span data-ttu-id="506b7-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="506b7-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="506b7-117">Name (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="506b7-117">Name (EmailAddress)</span></span>](name-emailaddress.md) <br/> |<span data-ttu-id="506b7-118">メールボックスユーザーの表示名を表します。</span><span class="sxs-lookup"><span data-stu-id="506b7-118">Represents the display name of the mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="506b7-119">Address (string)</span><span class="sxs-lookup"><span data-stu-id="506b7-119">Address (string)</span></span>](address-string.md) <br/> |<span data-ttu-id="506b7-120">メールボックスユーザーの電子メールアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="506b7-120">Represents the e-mail address of the mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="506b7-121">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="506b7-121">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="506b7-122">メッセージのルーティングプロトコルを表します。</span><span class="sxs-lookup"><span data-stu-id="506b7-122">Represents the routing protocol for the message.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="506b7-123">親要素</span><span class="sxs-lookup"><span data-stu-id="506b7-123">Parent elements</span></span>

|<span data-ttu-id="506b7-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="506b7-124">**Element**</span></span>|<span data-ttu-id="506b7-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="506b7-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="506b7-126">MailboxData</span><span class="sxs-lookup"><span data-stu-id="506b7-126">MailboxData</span></span>](mailboxdata.md) <br/> |<span data-ttu-id="506b7-127">個々のメールボックスユーザー、およびメールボックスユーザーに関して返されるデータの種類のオプションを表します。</span><span class="sxs-lookup"><span data-stu-id="506b7-127">Represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span>  <br/> <span data-ttu-id="506b7-128">この要素の XPath を次に示します。</span><span class="sxs-lookup"><span data-stu-id="506b7-128">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]/MailboxData` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="506b7-129">注釈</span><span class="sxs-lookup"><span data-stu-id="506b7-129">Remarks</span></span>

<span data-ttu-id="506b7-130">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの/EWS/ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="506b7-130">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="506b7-131">要素の情報</span><span class="sxs-lookup"><span data-stu-id="506b7-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="506b7-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="506b7-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="506b7-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="506b7-133">Schema Name</span></span>  <br/> |<span data-ttu-id="506b7-134">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="506b7-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="506b7-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="506b7-135">Validation File</span></span>  <br/> |<span data-ttu-id="506b7-136">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="506b7-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="506b7-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="506b7-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="506b7-138">正しくない</span><span class="sxs-lookup"><span data-stu-id="506b7-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="506b7-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="506b7-139">See also</span></span>

- [<span data-ttu-id="506b7-140">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="506b7-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)  
- [<span data-ttu-id="506b7-141">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="506b7-141">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="506b7-142">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="506b7-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

