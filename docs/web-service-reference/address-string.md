---
title: アドレス (文字列)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Address
api_type:
- schema
ms.assetid: a3cdfcbd-d0c5-46d6-8daa-52405fc63ff0
description: アドレス要素では、メールボックス ユーザーの電子メール アドレスを表します。
ms.openlocfilehash: 07c634d6166d88a8912bc66081a13671e600c801
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759299"
---
# <a name="address-string"></a><span data-ttu-id="9eb82-103">アドレス (文字列)</span><span class="sxs-lookup"><span data-stu-id="9eb82-103">Address (string)</span></span>

<span data-ttu-id="9eb82-104">**アドレス**要素では、メールボックス ユーザーの電子メール アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="9eb82-104">The **Address** element represents the e-mail address of the mailbox user.</span></span> 
  
```xml
<Address>...</Address>
```

 <span data-ttu-id="9eb82-105">**string**</span><span class="sxs-lookup"><span data-stu-id="9eb82-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9eb82-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9eb82-106">Attributes and elements</span></span>

<span data-ttu-id="9eb82-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9eb82-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9eb82-108">属性</span><span class="sxs-lookup"><span data-stu-id="9eb82-108">Attributes</span></span>

<span data-ttu-id="9eb82-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9eb82-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9eb82-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9eb82-110">Child elements</span></span>

<span data-ttu-id="9eb82-111">なし。</span><span class="sxs-lookup"><span data-stu-id="9eb82-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9eb82-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9eb82-112">Parent elements</span></span>

|<span data-ttu-id="9eb82-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="9eb82-113">**Element**</span></span>|<span data-ttu-id="9eb82-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="9eb82-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9eb82-115">電子メール (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="9eb82-115">Email (EmailAddressType)</span></span>](email-emailaddresstype.md) <br/> |<span data-ttu-id="9eb82-116">MailboxData オブジェクトの電子メール アドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="9eb82-116">Specifies the e-mail address of the MailboxData object.</span></span> <span data-ttu-id="9eb82-117">この要素は、 [GetUserAvailability の操作](getuseravailability-operation.md)で使用されます。</span><span class="sxs-lookup"><span data-stu-id="9eb82-117">This element is used in the [GetUserAvailability operation](getuseravailability-operation.md).</span></span><br/><br/> <span data-ttu-id="9eb82-118">以下は、この要素の XPath です。</span><span class="sxs-lookup"><span data-stu-id="9eb82-118">The following is the XPath to this element:</span></span><br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[<span data-ttu-id="9eb82-119">メールボックス (可用性)</span><span class="sxs-lookup"><span data-stu-id="9eb82-119">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> | <span data-ttu-id="9eb82-120">SetUserOofSettings または GetUserOofSettings の要求をメールボックスのユーザーを表します。</span><span class="sxs-lookup"><span data-stu-id="9eb82-120">Represents the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span><br/><br/>  <span data-ttu-id="9eb82-121">この要素への XPath 式は、次のように。</span><span class="sxs-lookup"><span data-stu-id="9eb82-121">The following are the XPath expressions to this element:</span></span><br/><br/>  `/GetUserOofSettingsRequest/Mailbox` <br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9eb82-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9eb82-122">Text value</span></span>

<span data-ttu-id="9eb82-123">テキスト値は、この要素が使用される場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="9eb82-123">A text value is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9eb82-124">備考</span><span class="sxs-lookup"><span data-stu-id="9eb82-124">Remarks</span></span>

<span data-ttu-id="9eb82-125">この要素には、最大で 1 回の[電子メール (EmailAddressType)](email-emailaddresstype.md)の要素と、[メールボックス (可用性)](mailbox-availability.md)が発生する可能性がします。</span><span class="sxs-lookup"><span data-stu-id="9eb82-125">This element can occur at most one time in the [Email (EmailAddressType)](email-emailaddresstype.md) element and the [Mailbox (Availability)](mailbox-availability.md) element.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="9eb82-126">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="9eb82-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="9eb82-127">要素情報</span><span class="sxs-lookup"><span data-stu-id="9eb82-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9eb82-128">名前空間</span><span class="sxs-lookup"><span data-stu-id="9eb82-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9eb82-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9eb82-129">Schema Name</span></span>  <br/> |<span data-ttu-id="9eb82-130">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="9eb82-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="9eb82-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9eb82-131">Validation File</span></span>  <br/> |<span data-ttu-id="9eb82-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9eb82-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9eb82-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9eb82-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="9eb82-134">False</span><span class="sxs-lookup"><span data-stu-id="9eb82-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9eb82-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="9eb82-135">See also</span></span>

- [<span data-ttu-id="9eb82-136">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="9eb82-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="9eb82-137">GetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="9eb82-137">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
- [<span data-ttu-id="9eb82-138">SetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="9eb82-138">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)
- [<span data-ttu-id="9eb82-139">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="9eb82-139">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="9eb82-140">GetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="9eb82-140">GetUserOofSettingsRequest</span></span>](getuseroofsettingsrequest.md)
- [<span data-ttu-id="9eb82-141">SetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="9eb82-141">SetUserOofSettingsRequest</span></span>](setuseroofsettingsrequest.md)
- [<span data-ttu-id="9eb82-142">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="9eb82-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

