---
title: Address (string)
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
description: Address 要素は、メールボックスユーザーの電子メールアドレスを表します。
ms.openlocfilehash: 839107050f22df5c00cb4dea9c531563df52933d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463644"
---
# <a name="address-string"></a><span data-ttu-id="afa12-103">Address (string)</span><span class="sxs-lookup"><span data-stu-id="afa12-103">Address (string)</span></span>

<span data-ttu-id="afa12-104">**Address**要素は、メールボックスユーザーの電子メールアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="afa12-104">The **Address** element represents the e-mail address of the mailbox user.</span></span> 
  
```xml
<Address>...</Address>
```

 <span data-ttu-id="afa12-105">**string**</span><span class="sxs-lookup"><span data-stu-id="afa12-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="afa12-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="afa12-106">Attributes and elements</span></span>

<span data-ttu-id="afa12-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="afa12-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="afa12-108">属性</span><span class="sxs-lookup"><span data-stu-id="afa12-108">Attributes</span></span>

<span data-ttu-id="afa12-109">なし。</span><span class="sxs-lookup"><span data-stu-id="afa12-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="afa12-110">子要素</span><span class="sxs-lookup"><span data-stu-id="afa12-110">Child elements</span></span>

<span data-ttu-id="afa12-111">なし。</span><span class="sxs-lookup"><span data-stu-id="afa12-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="afa12-112">親要素</span><span class="sxs-lookup"><span data-stu-id="afa12-112">Parent elements</span></span>

|<span data-ttu-id="afa12-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="afa12-113">**Element**</span></span>|<span data-ttu-id="afa12-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="afa12-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="afa12-115">電子メール (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="afa12-115">Email (EmailAddressType)</span></span>](email-emailaddresstype.md) <br/> |<span data-ttu-id="afa12-116">MailboxData オブジェクトの電子メールアドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="afa12-116">Specifies the e-mail address of the MailboxData object.</span></span> <span data-ttu-id="afa12-117">この要素は、 [Getuseravailability 操作](getuseravailability-operation.md)で使用されます。</span><span class="sxs-lookup"><span data-stu-id="afa12-117">This element is used in the [GetUserAvailability operation](getuseravailability-operation.md).</span></span><br/><br/> <span data-ttu-id="afa12-118">この要素の XPath を次に示します。</span><span class="sxs-lookup"><span data-stu-id="afa12-118">The following is the XPath to this element:</span></span><br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[<span data-ttu-id="afa12-119">メールボックス (可用性)</span><span class="sxs-lookup"><span data-stu-id="afa12-119">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> | <span data-ttu-id="afa12-120">SetUserOofSettings または GetUserOofSettings 要求のメールボックスユーザーを表します。</span><span class="sxs-lookup"><span data-stu-id="afa12-120">Represents the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span><br/><br/>  <span data-ttu-id="afa12-121">この要素の XPath 式は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="afa12-121">The following are the XPath expressions to this element:</span></span><br/><br/>  `/GetUserOofSettingsRequest/Mailbox` <br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="afa12-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="afa12-122">Text value</span></span>

<span data-ttu-id="afa12-123">この要素を使用する場合は、テキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="afa12-123">A text value is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="afa12-124">注釈</span><span class="sxs-lookup"><span data-stu-id="afa12-124">Remarks</span></span>

<span data-ttu-id="afa12-125">この要素は、 [email (EmailAddressType)](email-emailaddresstype.md)要素と[Mailbox (Availability)](mailbox-availability.md)要素で、最大で1回だけ発生します。</span><span class="sxs-lookup"><span data-stu-id="afa12-125">This element can occur at most one time in the [Email (EmailAddressType)](email-emailaddresstype.md) element and the [Mailbox (Availability)](mailbox-availability.md) element.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="afa12-126">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="afa12-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="afa12-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="afa12-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="afa12-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="afa12-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="afa12-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="afa12-129">Schema Name</span></span>  <br/> |<span data-ttu-id="afa12-130">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="afa12-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="afa12-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="afa12-131">Validation File</span></span>  <br/> |<span data-ttu-id="afa12-132">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="afa12-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="afa12-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="afa12-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="afa12-134">正しくない</span><span class="sxs-lookup"><span data-stu-id="afa12-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="afa12-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="afa12-135">See also</span></span>

- [<span data-ttu-id="afa12-136">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="afa12-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="afa12-137">GetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="afa12-137">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
- [<span data-ttu-id="afa12-138">SetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="afa12-138">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)
- [<span data-ttu-id="afa12-139">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="afa12-139">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="afa12-140">GetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="afa12-140">GetUserOofSettingsRequest</span></span>](getuseroofsettingsrequest.md)
- [<span data-ttu-id="afa12-141">SetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="afa12-141">SetUserOofSettingsRequest</span></span>](setuseroofsettingsrequest.md)
- [<span data-ttu-id="afa12-142">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="afa12-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

