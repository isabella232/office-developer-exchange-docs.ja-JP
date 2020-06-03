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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466956"
---
# <a name="name-emailaddress"></a><span data-ttu-id="1fba5-103">Name (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="1fba5-103">Name (EmailAddress)</span></span>

<span data-ttu-id="1fba5-104">**Name**要素は、メールボックスユーザーの表示名を表します。</span><span class="sxs-lookup"><span data-stu-id="1fba5-104">The **Name** element represents the display name of the mailbox user.</span></span> 
  
```xml
<Name/>
```

<span data-ttu-id="1fba5-105">**String**</span><span class="sxs-lookup"><span data-stu-id="1fba5-105">**String**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="1fba5-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1fba5-106">Attributes and elements</span></span>

<span data-ttu-id="1fba5-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1fba5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1fba5-108">属性</span><span class="sxs-lookup"><span data-stu-id="1fba5-108">Attributes</span></span>

<span data-ttu-id="1fba5-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1fba5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1fba5-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1fba5-110">Child elements</span></span>

<span data-ttu-id="1fba5-111">なし。</span><span class="sxs-lookup"><span data-stu-id="1fba5-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1fba5-112">親要素</span><span class="sxs-lookup"><span data-stu-id="1fba5-112">Parent elements</span></span>

|<span data-ttu-id="1fba5-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="1fba5-113">**Element**</span></span>|<span data-ttu-id="1fba5-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="1fba5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1fba5-115">電子メール (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="1fba5-115">Email (EmailAddressType)</span></span>](email-emailaddresstype.md) <br/> |<span data-ttu-id="1fba5-116">GetUserAvailability クエリのメールボックスユーザーを表します。</span><span class="sxs-lookup"><span data-stu-id="1fba5-116">Represents the mailbox user for a GetUserAvailability query.</span></span>  <br/> <br/><span data-ttu-id="1fba5-117">この要素の XPath を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1fba5-117">The following is the XPath to this element:</span></span>  <br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[<span data-ttu-id="1fba5-118">メールボックス (可用性)</span><span class="sxs-lookup"><span data-stu-id="1fba5-118">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> | <span data-ttu-id="1fba5-119">SetUserOofSettings または GetUserOofSettings 要求のメールボックスユーザーを表します。</span><span class="sxs-lookup"><span data-stu-id="1fba5-119">Represents the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span>  <br/><br/>  <span data-ttu-id="1fba5-120">この要素の XPath 式は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="1fba5-120">The following are the XPath expressions to this element:</span></span>  <br/><br/>  `/GetUserOofSettingsRequest/Mailbox` <br/><br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1fba5-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1fba5-121">Text value</span></span>

<span data-ttu-id="1fba5-122">この要素を使用する場合は、テキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="1fba5-122">A text value is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1fba5-123">注釈</span><span class="sxs-lookup"><span data-stu-id="1fba5-123">Remarks</span></span>

<span data-ttu-id="1fba5-124">この要素は、 [email (EmailAddressType)](email-emailaddresstype.md)要素で最大で1回発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="1fba5-124">This element can occur at most one time in the [Email (EmailAddressType)](email-emailaddresstype.md) element.</span></span> <span data-ttu-id="1fba5-125">この要素は必須ではありません。</span><span class="sxs-lookup"><span data-stu-id="1fba5-125">This element is not required.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="1fba5-126">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="1fba5-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="1fba5-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1fba5-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1fba5-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="1fba5-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1fba5-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1fba5-129">Schema Name</span></span>  <br/> |<span data-ttu-id="1fba5-130">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="1fba5-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="1fba5-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1fba5-131">Validation File</span></span>  <br/> |<span data-ttu-id="1fba5-132">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="1fba5-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1fba5-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1fba5-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="1fba5-134">正しくない</span><span class="sxs-lookup"><span data-stu-id="1fba5-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1fba5-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="1fba5-135">See also</span></span>

- [<span data-ttu-id="1fba5-136">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="1fba5-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="1fba5-137">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="1fba5-137">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="1fba5-138">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="1fba5-138">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

