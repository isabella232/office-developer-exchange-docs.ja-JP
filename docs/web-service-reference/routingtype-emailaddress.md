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
description: RoutingType 要素は、受信者のルーティング プロトコルを表します。
ms.openlocfilehash: a0a6cf312bcb1d4b4818a82bc8d8d3e3f33ad6f6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833255"
---
# <a name="routingtype-emailaddress"></a><span data-ttu-id="ea73a-103">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="ea73a-103">RoutingType (EmailAddress)</span></span>

<span data-ttu-id="ea73a-104">**RoutingType**要素は、受信者のルーティング プロトコルを表します。</span><span class="sxs-lookup"><span data-stu-id="ea73a-104">The **RoutingType** element represents the routing protocol for the recipient.</span></span> 
  
```XML
<RoutingType/>
```

 <span data-ttu-id="ea73a-105">**string**</span><span class="sxs-lookup"><span data-stu-id="ea73a-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ea73a-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ea73a-106">Attributes and elements</span></span>

<span data-ttu-id="ea73a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ea73a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ea73a-108">属性</span><span class="sxs-lookup"><span data-stu-id="ea73a-108">Attributes</span></span>

<span data-ttu-id="ea73a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ea73a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ea73a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ea73a-110">Child elements</span></span>

<span data-ttu-id="ea73a-111">なし。</span><span class="sxs-lookup"><span data-stu-id="ea73a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ea73a-112">親要素</span><span class="sxs-lookup"><span data-stu-id="ea73a-112">Parent elements</span></span>

|<span data-ttu-id="ea73a-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="ea73a-113">**Element**</span></span>|<span data-ttu-id="ea73a-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="ea73a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ea73a-115">電子メール (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="ea73a-115">Email (EmailAddressType)</span></span>](email-emailaddresstype.md) <br/> |<span data-ttu-id="ea73a-116">MailboxData オブジェクトの電子メール アドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="ea73a-116">Specifies the e-mail address of the MailboxData object.</span></span> <span data-ttu-id="ea73a-117">この要素は、 [GetUserAvailability の操作](getuseravailability-operation.md)で使用されます。</span><span class="sxs-lookup"><span data-stu-id="ea73a-117">This element is used in the [GetUserAvailability operation](getuseravailability-operation.md).</span></span>  <br/><br/> <span data-ttu-id="ea73a-118">以下は、この要素の XPath です。</span><span class="sxs-lookup"><span data-stu-id="ea73a-118">The following is the XPath to this element:</span></span>  <br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[<span data-ttu-id="ea73a-119">メールボックス (可用性)</span><span class="sxs-lookup"><span data-stu-id="ea73a-119">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> | <span data-ttu-id="ea73a-120">SetUserOofSettings または GetUserOofSettings の要求をメールボックスのユーザーを表します。</span><span class="sxs-lookup"><span data-stu-id="ea73a-120">Represents the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span>  <br/><br/>  <span data-ttu-id="ea73a-121">この要素への XPath 式は、次のように。</span><span class="sxs-lookup"><span data-stu-id="ea73a-121">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/GetUserOofSettingsRequest/Mailbox` <br/><br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ea73a-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ea73a-122">Text value</span></span>

<span data-ttu-id="ea73a-123">テキスト値は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="ea73a-123">A text value is optional.</span></span> <span data-ttu-id="ea73a-124">唯一の有効値は、SMTP です。</span><span class="sxs-lookup"><span data-stu-id="ea73a-124">The only valid value is SMTP.</span></span> <span data-ttu-id="ea73a-125">値が指定されていない場合は、SMTP のデフォルト値が使用されます。</span><span class="sxs-lookup"><span data-stu-id="ea73a-125">If no value is provided, the default value of SMTP is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ea73a-126">備考</span><span class="sxs-lookup"><span data-stu-id="ea73a-126">Remarks</span></span>

<span data-ttu-id="ea73a-127">この要素は、最大で 1 回、[電子メール (EmailAddressType)](email-emailaddresstype.md)の要素で発生します。</span><span class="sxs-lookup"><span data-stu-id="ea73a-127">This element can occur at most one time in the [Email (EmailAddressType)](email-emailaddresstype.md) element.</span></span> <span data-ttu-id="ea73a-128">この要素は必須ではありません。</span><span class="sxs-lookup"><span data-stu-id="ea73a-128">This element is not required.</span></span> <span data-ttu-id="ea73a-129">将来のプロトコルのため、この要素が存在しています。</span><span class="sxs-lookup"><span data-stu-id="ea73a-129">This element exists for the inclusion of future protocols.</span></span> <span data-ttu-id="ea73a-130">もう 1 つの**RoutingType**要素は、ユーザーのメールボックス内のアイテムへのアクセスに使用されます。</span><span class="sxs-lookup"><span data-stu-id="ea73a-130">Another **RoutingType** element is used for accessing items in a user's mailbox.</span></span> 
  
<span data-ttu-id="ea73a-131">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ea73a-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ea73a-132">要素情報</span><span class="sxs-lookup"><span data-stu-id="ea73a-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ea73a-133">名前空間</span><span class="sxs-lookup"><span data-stu-id="ea73a-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ea73a-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ea73a-134">Schema Name</span></span>  <br/> |<span data-ttu-id="ea73a-135">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="ea73a-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="ea73a-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ea73a-136">Validation File</span></span>  <br/> |<span data-ttu-id="ea73a-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ea73a-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ea73a-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ea73a-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="ea73a-139">False</span><span class="sxs-lookup"><span data-stu-id="ea73a-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ea73a-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="ea73a-140">See also</span></span>

- [<span data-ttu-id="ea73a-141">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="ea73a-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="ea73a-142">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="ea73a-142">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="ea73a-143">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="ea73a-143">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

