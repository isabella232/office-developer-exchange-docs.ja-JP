---
title: RoutingType (EmailAddress)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RoutingType
api_type:
- schema
ms.assetid: 74d83198-0d9d-4c78-a2bc-9a671859ff37
description: RoutingType 要素は、受信者のルーティングプロトコルを表します。
ms.openlocfilehash: 2193e72c38c687669f6e052b4d2526029aa89d89
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459035"
---
# <a name="routingtype-emailaddress"></a><span data-ttu-id="6c6e4-103">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="6c6e4-103">RoutingType (EmailAddress)</span></span>

<span data-ttu-id="6c6e4-104">**Routingtype**要素は、受信者のルーティングプロトコルを表します。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-104">The **RoutingType** element represents the routing protocol for the recipient.</span></span> 
  
```XML
<RoutingType/>
```

 <span data-ttu-id="6c6e4-105">**string**</span><span class="sxs-lookup"><span data-stu-id="6c6e4-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6c6e4-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6c6e4-106">Attributes and elements</span></span>

<span data-ttu-id="6c6e4-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6c6e4-108">属性</span><span class="sxs-lookup"><span data-stu-id="6c6e4-108">Attributes</span></span>

<span data-ttu-id="6c6e4-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6c6e4-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6c6e4-110">Child elements</span></span>

<span data-ttu-id="6c6e4-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6c6e4-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6c6e4-112">Parent elements</span></span>

|<span data-ttu-id="6c6e4-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="6c6e4-113">**Element**</span></span>|<span data-ttu-id="6c6e4-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="6c6e4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6c6e4-115">電子メール (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="6c6e4-115">Email (EmailAddressType)</span></span>](email-emailaddresstype.md) <br/> |<span data-ttu-id="6c6e4-116">MailboxData オブジェクトの電子メールアドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-116">Specifies the e-mail address of the MailboxData object.</span></span> <span data-ttu-id="6c6e4-117">この要素は、 [Getuseravailability 操作](getuseravailability-operation.md)で使用されます。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-117">This element is used in the [GetUserAvailability operation](getuseravailability-operation.md).</span></span>  <br/><br/> <span data-ttu-id="6c6e4-118">この要素の XPath を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-118">The following is the XPath to this element:</span></span>  <br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[<span data-ttu-id="6c6e4-119">メールボックス (可用性)</span><span class="sxs-lookup"><span data-stu-id="6c6e4-119">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> | <span data-ttu-id="6c6e4-120">SetUserOofSettings または GetUserOofSettings 要求のメールボックスユーザーを表します。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-120">Represents the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span>  <br/><br/>  <span data-ttu-id="6c6e4-121">この要素の XPath 式は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-121">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/GetUserOofSettingsRequest/Mailbox` <br/><br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6c6e4-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6c6e4-122">Text value</span></span>

<span data-ttu-id="6c6e4-123">テキスト値はオプションです。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-123">A text value is optional.</span></span> <span data-ttu-id="6c6e4-124">指定可能な値は次のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-124">The following are the possible values:</span></span>

* <span data-ttu-id="6c6e4-125">SMTP</span><span class="sxs-lookup"><span data-stu-id="6c6e4-125">SMTP</span></span>
* <span data-ttu-id="6c6e4-126">渡し</span><span class="sxs-lookup"><span data-stu-id="6c6e4-126">EX</span></span>

<span data-ttu-id="6c6e4-127">値が指定されていない場合は、SMTP の既定値が使用されます。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-127">If no value is provided, the default value of SMTP is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6c6e4-128">注釈</span><span class="sxs-lookup"><span data-stu-id="6c6e4-128">Remarks</span></span>

<span data-ttu-id="6c6e4-129">この要素は、 [email (EmailAddressType)](email-emailaddresstype.md)要素で最大で1回発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-129">This element can occur at most one time in the [Email (EmailAddressType)](email-emailaddresstype.md) element.</span></span> <span data-ttu-id="6c6e4-130">この要素は必須ではありません。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-130">This element is not required.</span></span> <span data-ttu-id="6c6e4-131">この要素は、将来のプロトコルを含めるために存在します。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-131">This element exists for the inclusion of future protocols.</span></span> <span data-ttu-id="6c6e4-132">ユーザーのメールボックス内のアイテムにアクセスするには、別の**Routingtype**要素を使用します。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-132">Another **RoutingType** element is used for accessing items in a user's mailbox.</span></span> 
  
<span data-ttu-id="6c6e4-133">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-133">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6c6e4-134">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6c6e4-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6c6e4-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="6c6e4-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6c6e4-136">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6c6e4-136">Schema Name</span></span>  <br/> |<span data-ttu-id="6c6e4-137">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="6c6e4-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="6c6e4-138">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6c6e4-138">Validation File</span></span>  <br/> |<span data-ttu-id="6c6e4-139">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="6c6e4-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6c6e4-140">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6c6e4-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="6c6e4-141">正しくない</span><span class="sxs-lookup"><span data-stu-id="6c6e4-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6c6e4-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="6c6e4-142">See also</span></span>

- [<span data-ttu-id="6c6e4-143">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="6c6e4-143">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="6c6e4-144">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="6c6e4-144">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="6c6e4-145">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="6c6e4-145">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

