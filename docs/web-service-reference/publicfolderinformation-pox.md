---
title: PublicFolderInformation (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: a221aa9e-b4ac-4ec5-aa42-7e2a69e8eaa6
description: PublicFolderInformation 要素には、クライアントが自動検出要求を送信してユーザーのパブリックフォルダー情報を検出するために使用できる情報が含まれています。
ms.openlocfilehash: e044a1feddfaeb4eb93c289c617dde9adc66f332
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457719"
---
# <a name="publicfolderinformation-pox"></a><span data-ttu-id="4c8e4-103">PublicFolderInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="4c8e4-103">PublicFolderInformation (POX)</span></span>

<span data-ttu-id="4c8e4-104">**Publicfolderinformation**要素には、クライアントが自動検出要求を送信してユーザーのパブリックフォルダー情報を検出するために使用できる情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="4c8e4-104">The **PublicFolderInformation** element contains information that clients can use to send an Autodiscover request to discover public folder information for the user.</span></span> 
  
[<span data-ttu-id="4c8e4-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="4c8e4-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="4c8e4-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="4c8e4-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="4c8e4-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="4c8e4-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="4c8e4-108">PublicFolderInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="4c8e4-108">PublicFolderInformation (POX)</span></span>](publicfolderinformation-pox.md)
  
```XML
<PublicFolderInformation>
   <SmtpAddress/>
</PublicFolderInformation>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="4c8e4-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="4c8e4-109">Attributes and elements</span></span>

<span data-ttu-id="4c8e4-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4c8e4-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4c8e4-111">属性</span><span class="sxs-lookup"><span data-stu-id="4c8e4-111">Attributes</span></span>

<span data-ttu-id="4c8e4-112">なし。</span><span class="sxs-lookup"><span data-stu-id="4c8e4-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4c8e4-113">子要素</span><span class="sxs-lookup"><span data-stu-id="4c8e4-113">Child elements</span></span>

|<span data-ttu-id="4c8e4-114">**Element**</span><span class="sxs-lookup"><span data-stu-id="4c8e4-114">**Element**</span></span>|<span data-ttu-id="4c8e4-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="4c8e4-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4c8e4-116">SmtpAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="4c8e4-116">SmtpAddress (POX)</span></span>](smtpaddress-pox.md) <br/> |<span data-ttu-id="4c8e4-117">ユーザー用に構成されたパブリックフォルダーメッセージストアに割り当てられている SMTP アドレスが含まれます。</span><span class="sxs-lookup"><span data-stu-id="4c8e4-117">Contains the SMTP address assigned to the public folder message store configured for the user.</span></span> <span data-ttu-id="4c8e4-118">この SMTP アドレスは、自動検出要求の[EMailAddress (POX)](emailaddress-pox.md)要素で、パブリックフォルダーの設定を検出するために使用できます。</span><span class="sxs-lookup"><span data-stu-id="4c8e4-118">This SMTP address can be used in the [EMailAddress (POX)](emailaddress-pox.md) element of an Autodiscover request to discover public folder settings.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4c8e4-119">親要素</span><span class="sxs-lookup"><span data-stu-id="4c8e4-119">Parent elements</span></span>

|<span data-ttu-id="4c8e4-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="4c8e4-120">**Element**</span></span>|<span data-ttu-id="4c8e4-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="4c8e4-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4c8e4-122">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="4c8e4-122">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="4c8e4-123">ユーザーのアカウント設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="4c8e4-123">Specifies account settings for the user.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4c8e4-124">注釈</span><span class="sxs-lookup"><span data-stu-id="4c8e4-124">Remarks</span></span>

<span data-ttu-id="4c8e4-125">**Publicfolderinformation**要素は、 **Account**要素のオプションの子要素です。</span><span class="sxs-lookup"><span data-stu-id="4c8e4-125">The **PublicFolderInformation** element is an optional child element of the **Account** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="4c8e4-126">関連項目</span><span class="sxs-lookup"><span data-stu-id="4c8e4-126">See also</span></span>



[<span data-ttu-id="4c8e4-127">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="4c8e4-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

