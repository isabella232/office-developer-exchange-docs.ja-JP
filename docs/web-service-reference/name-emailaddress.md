---
title: 名 (EmailAddress)
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
description: Name 要素は、メールボックス ユーザーの表示名を表します。
ms.openlocfilehash: 6d30f06c3bfd77d2715798349ab084cdf81f21a6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832505"
---
# <a name="name-emailaddress"></a><span data-ttu-id="bec4c-103">名 (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="bec4c-103">Name (EmailAddress)</span></span>

<span data-ttu-id="bec4c-104">**Name**要素は、メールボックス ユーザーの表示名を表します。</span><span class="sxs-lookup"><span data-stu-id="bec4c-104">The **Name** element represents the display name of the mailbox user.</span></span> 
  
```xml
<Name/>
```

<span data-ttu-id="bec4c-105">**文字列型 (String)**</span><span class="sxs-lookup"><span data-stu-id="bec4c-105">**String**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="bec4c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="bec4c-106">Attributes and elements</span></span>

<span data-ttu-id="bec4c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="bec4c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bec4c-108">属性</span><span class="sxs-lookup"><span data-stu-id="bec4c-108">Attributes</span></span>

<span data-ttu-id="bec4c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="bec4c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bec4c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="bec4c-110">Child elements</span></span>

<span data-ttu-id="bec4c-111">なし。</span><span class="sxs-lookup"><span data-stu-id="bec4c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bec4c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="bec4c-112">Parent elements</span></span>

|<span data-ttu-id="bec4c-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="bec4c-113">**Element**</span></span>|<span data-ttu-id="bec4c-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="bec4c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bec4c-115">電子メール (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="bec4c-115">Email (EmailAddressType)</span></span>](email-emailaddresstype.md) <br/> |<span data-ttu-id="bec4c-116">GetUserAvailability クエリのメールボックスのユーザーを表します。</span><span class="sxs-lookup"><span data-stu-id="bec4c-116">Represents the mailbox user for a GetUserAvailability query.</span></span>  <br/> <br/><span data-ttu-id="bec4c-117">以下は、この要素の XPath です。</span><span class="sxs-lookup"><span data-stu-id="bec4c-117">The following is the XPath to this element:</span></span>  <br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[<span data-ttu-id="bec4c-118">メールボックス (可用性)</span><span class="sxs-lookup"><span data-stu-id="bec4c-118">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> | <span data-ttu-id="bec4c-119">SetUserOofSettings または GetUserOofSettings の要求をメールボックスのユーザーを表します。</span><span class="sxs-lookup"><span data-stu-id="bec4c-119">Represents the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span>  <br/><br/>  <span data-ttu-id="bec4c-120">この要素への XPath 式は、次のように。</span><span class="sxs-lookup"><span data-stu-id="bec4c-120">The following are the XPath expressions to this element:</span></span>  <br/><br/>  `/GetUserOofSettingsRequest/Mailbox` <br/><br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bec4c-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="bec4c-121">Text value</span></span>

<span data-ttu-id="bec4c-122">テキスト値は、この要素が使用される場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="bec4c-122">A text value is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bec4c-123">備考</span><span class="sxs-lookup"><span data-stu-id="bec4c-123">Remarks</span></span>

<span data-ttu-id="bec4c-124">この要素は、最大で 1 回、[電子メール (EmailAddressType)](email-emailaddresstype.md)の要素で発生します。</span><span class="sxs-lookup"><span data-stu-id="bec4c-124">This element can occur at most one time in the [Email (EmailAddressType)](email-emailaddresstype.md) element.</span></span> <span data-ttu-id="bec4c-125">この要素は必須ではありません。</span><span class="sxs-lookup"><span data-stu-id="bec4c-125">This element is not required.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="bec4c-126">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="bec4c-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="bec4c-127">要素情報</span><span class="sxs-lookup"><span data-stu-id="bec4c-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bec4c-128">名前空間</span><span class="sxs-lookup"><span data-stu-id="bec4c-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bec4c-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="bec4c-129">Schema Name</span></span>  <br/> |<span data-ttu-id="bec4c-130">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="bec4c-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="bec4c-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="bec4c-131">Validation File</span></span>  <br/> |<span data-ttu-id="bec4c-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bec4c-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bec4c-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="bec4c-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="bec4c-134">False</span><span class="sxs-lookup"><span data-stu-id="bec4c-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bec4c-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="bec4c-135">See also</span></span>

- [<span data-ttu-id="bec4c-136">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="bec4c-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="bec4c-137">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="bec4c-137">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="bec4c-138">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="bec4c-138">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

