---
title: PublicFolderInformation (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: a221aa9e-b4ac-4ec5-aa42-7e2a69e8eaa6
description: PublicFolderInformation 要素には、クライアント ユーザーのパブリック フォルダー情報を検出する自動検出要求の送信に使用できる情報が含まれています。
ms.openlocfilehash: bb4432a664024c3d1ccb17826948cfe7a1b58cdf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832927"
---
# <a name="publicfolderinformation-pox"></a><span data-ttu-id="97eb8-103">PublicFolderInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="97eb8-103">PublicFolderInformation (POX)</span></span>

<span data-ttu-id="97eb8-104">**PublicFolderInformation**要素には、クライアント ユーザーのパブリック フォルダー情報を検出する自動検出要求の送信に使用できる情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="97eb8-104">The **PublicFolderInformation** element contains information that clients can use to send an Autodiscover request to discover public folder information for the user.</span></span> 
  
[<span data-ttu-id="97eb8-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="97eb8-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="97eb8-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="97eb8-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="97eb8-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="97eb8-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="97eb8-108">PublicFolderInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="97eb8-108">PublicFolderInformation (POX)</span></span>](publicfolderinformation-pox.md)
  
```XML
<PublicFolderInformation>
   <SmtpAddress/>
</PublicFolderInformation>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="97eb8-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="97eb8-109">Attributes and elements</span></span>

<span data-ttu-id="97eb8-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="97eb8-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="97eb8-111">属性</span><span class="sxs-lookup"><span data-stu-id="97eb8-111">Attributes</span></span>

<span data-ttu-id="97eb8-112">なし。</span><span class="sxs-lookup"><span data-stu-id="97eb8-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="97eb8-113">子要素</span><span class="sxs-lookup"><span data-stu-id="97eb8-113">Child elements</span></span>

|<span data-ttu-id="97eb8-114">**要素**</span><span class="sxs-lookup"><span data-stu-id="97eb8-114">**Element**</span></span>|<span data-ttu-id="97eb8-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="97eb8-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97eb8-116">SmtpAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="97eb8-116">SmtpAddress (POX)</span></span>](smtpaddress-pox.md) <br/> |<span data-ttu-id="97eb8-117">ユーザー用に構成するパブリック フォルダーのメッセージ ストアに割り当てられている SMTP アドレスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="97eb8-117">Contains the SMTP address assigned to the public folder message store configured for the user.</span></span> <span data-ttu-id="97eb8-118">この SMTP アドレスは、パブリック フォルダーの設定を検出する自動検出要求の[EMailAddress (POX)](emailaddress-pox.md)要素で使用できます。</span><span class="sxs-lookup"><span data-stu-id="97eb8-118">This SMTP address can be used in the [EMailAddress (POX)](emailaddress-pox.md) element of an Autodiscover request to discover public folder settings.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="97eb8-119">親要素</span><span class="sxs-lookup"><span data-stu-id="97eb8-119">Parent elements</span></span>

|<span data-ttu-id="97eb8-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="97eb8-120">**Element**</span></span>|<span data-ttu-id="97eb8-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="97eb8-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97eb8-122">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="97eb8-122">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="97eb8-123">ユーザーのアカウントの設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="97eb8-123">Specifies account settings for the user.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="97eb8-124">備考</span><span class="sxs-lookup"><span data-stu-id="97eb8-124">Remarks</span></span>

<span data-ttu-id="97eb8-125">**PublicFolderInformation**要素は、**アカウント**の要素の省略可能な子要素です。</span><span class="sxs-lookup"><span data-stu-id="97eb8-125">The **PublicFolderInformation** element is an optional child element of the **Account** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="97eb8-126">関連項目</span><span class="sxs-lookup"><span data-stu-id="97eb8-126">See also</span></span>



[<span data-ttu-id="97eb8-127">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="97eb8-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

