---
title: Name (EmailAddress)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Name
api_type:
- schema
ms.assetid: c719c55f-d625-4e64-846f-50ac91881443
description: Name 要素は、メールボックスユーザーの表示名を表します。
ms.openlocfilehash: 2c6b29f1b069f9cc72ac84e7aebfff99437e630a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/01/2020
ms.locfileid: "44466956"
---
# <a name="name-emailaddress"></a><span data-ttu-id="d0c61-103">Name (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="d0c61-103">Name (EmailAddress)</span></span>

<span data-ttu-id="d0c61-104">**Name**要素は、メールボックスユーザーの表示名を表します。</span><span class="sxs-lookup"><span data-stu-id="d0c61-104">The **Name** element represents the display name of the mailbox user.</span></span> 
  
```xml
<Name/>
```

<span data-ttu-id="d0c61-105">**String**</span><span class="sxs-lookup"><span data-stu-id="d0c61-105">**String**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d0c61-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d0c61-106">Attributes and elements</span></span>

<span data-ttu-id="d0c61-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d0c61-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d0c61-108">属性</span><span class="sxs-lookup"><span data-stu-id="d0c61-108">Attributes</span></span>

<span data-ttu-id="d0c61-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d0c61-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d0c61-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d0c61-110">Child elements</span></span>

<span data-ttu-id="d0c61-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d0c61-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d0c61-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d0c61-112">Parent elements</span></span>

|<span data-ttu-id="d0c61-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="d0c61-113">**Element**</span></span>|<span data-ttu-id="d0c61-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="d0c61-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d0c61-115">電子メール (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="d0c61-115">Email (EmailAddressType)</span></span>](email-emailaddresstype.md) <br/> |<span data-ttu-id="d0c61-116">GetUserAvailability クエリのメールボックスユーザーを表します。</span><span class="sxs-lookup"><span data-stu-id="d0c61-116">Represents the mailbox user for a GetUserAvailability query.</span></span>  <br/> <br/><span data-ttu-id="d0c61-117">この要素の XPath を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d0c61-117">The following is the XPath to this element:</span></span>  <br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[<span data-ttu-id="d0c61-118">メールボックス (可用性)</span><span class="sxs-lookup"><span data-stu-id="d0c61-118">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> | <span data-ttu-id="d0c61-119">SetUserOofSettings または GetUserOofSettings 要求のメールボックスユーザーを表します。</span><span class="sxs-lookup"><span data-stu-id="d0c61-119">Represents the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span>  <br/><br/>  <span data-ttu-id="d0c61-120">この要素の XPath 式は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="d0c61-120">The following are the XPath expressions to this element:</span></span>  <br/><br/>  `/GetUserOofSettingsRequest/Mailbox` <br/><br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d0c61-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d0c61-121">Text value</span></span>

<span data-ttu-id="d0c61-122">この要素を使用する場合は、テキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="d0c61-122">A text value is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d0c61-123">注釈</span><span class="sxs-lookup"><span data-stu-id="d0c61-123">Remarks</span></span>

<span data-ttu-id="d0c61-124">この要素は、 [email (EmailAddressType)](email-emailaddresstype.md)要素で最大で1回発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="d0c61-124">This element can occur at most one time in the [Email (EmailAddressType)](email-emailaddresstype.md) element.</span></span> <span data-ttu-id="d0c61-125">この要素は必須ではありません。</span><span class="sxs-lookup"><span data-stu-id="d0c61-125">This element is not required.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="d0c61-126">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="d0c61-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="d0c61-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d0c61-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d0c61-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="d0c61-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d0c61-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d0c61-129">Schema Name</span></span>  <br/> |<span data-ttu-id="d0c61-130">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d0c61-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="d0c61-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d0c61-131">Validation File</span></span>  <br/> |<span data-ttu-id="d0c61-132">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d0c61-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d0c61-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d0c61-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="d0c61-134">正しくない</span><span class="sxs-lookup"><span data-stu-id="d0c61-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d0c61-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="d0c61-135">See also</span></span>

- [<span data-ttu-id="d0c61-136">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="d0c61-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="d0c61-137">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="d0c61-137">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="d0c61-138">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="d0c61-138">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

