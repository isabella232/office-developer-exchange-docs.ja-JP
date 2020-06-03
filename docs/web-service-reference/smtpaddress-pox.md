---
title: SmtpAddress (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 984ccd97-c337-47b6-ba42-3405a8b55a71
description: SmtpAddress 要素には、ユーザー用に構成されたパブリックフォルダーメッセージストアに割り当てられた SMTP アドレスが含まれています。
ms.openlocfilehash: 48703a11fb056967c6c76073c2e928d5f6efa264
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468643"
---
# <a name="smtpaddress-pox"></a><span data-ttu-id="cb174-103">SmtpAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="cb174-103">SmtpAddress (POX)</span></span>

<span data-ttu-id="cb174-104">**Smtpaddress**要素には、ユーザー用に構成されたパブリックフォルダーメッセージストアに割り当てられた SMTP アドレスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="cb174-104">The **SmtpAddress** element contains the SMTP address assigned to the public folder message store configured for the user.</span></span> 
  
- [<span data-ttu-id="cb174-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="cb174-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
- [<span data-ttu-id="cb174-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="cb174-106">Response (POX)</span></span>](response-pox.md)
  
- [<span data-ttu-id="cb174-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="cb174-107">Account (POX)</span></span>](account-pox.md)
  
- [<span data-ttu-id="cb174-108">PublicFolderInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="cb174-108">PublicFolderInformation (POX)</span></span>](publicfolderinformation-pox.md)
  
- [<span data-ttu-id="cb174-109">SmtpAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="cb174-109">SmtpAddress (POX)</span></span>](smtpaddress-pox.md)
  
```XML
<SmtpAddress/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="cb174-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="cb174-110">Attributes and elements</span></span>

<span data-ttu-id="cb174-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cb174-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cb174-112">属性</span><span class="sxs-lookup"><span data-stu-id="cb174-112">Attributes</span></span>

<span data-ttu-id="cb174-113">なし。</span><span class="sxs-lookup"><span data-stu-id="cb174-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cb174-114">子要素</span><span class="sxs-lookup"><span data-stu-id="cb174-114">Child elements</span></span>

<span data-ttu-id="cb174-115">なし。</span><span class="sxs-lookup"><span data-stu-id="cb174-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cb174-116">親要素</span><span class="sxs-lookup"><span data-stu-id="cb174-116">Parent elements</span></span>

|<span data-ttu-id="cb174-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="cb174-117">**Element**</span></span>|<span data-ttu-id="cb174-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="cb174-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cb174-119">PublicFolderInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="cb174-119">PublicFolderInformation (POX)</span></span>](publicfolderinformation-pox.md) <br/> |<span data-ttu-id="cb174-120">クライアントが、ユーザーのパブリックフォルダー情報を検出するために自動検出要求を送信するために使用できる情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cb174-120">Contains information that clients can use to send an Autodiscover request to discover public folder information for the user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cb174-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="cb174-121">Text value</span></span>

<span data-ttu-id="cb174-122">Text 値は、ユーザーに対して構成されているパブリックフォルダーストアに割り当てられた SMTP アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="cb174-122">The text value represents the SMTP address assigned to the public folder store configured for the user.</span></span> <span data-ttu-id="cb174-123">この SMTP アドレスは、自動検出要求の[EMailAddress (POX)](emailaddress-pox.md)要素で、パブリックフォルダーの設定を検出するために使用できます。</span><span class="sxs-lookup"><span data-stu-id="cb174-123">This SMTP address can be used in the [EMailAddress (POX)](emailaddress-pox.md) element of an Autodiscover request to discover public folder settings.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="cb174-124">注釈</span><span class="sxs-lookup"><span data-stu-id="cb174-124">Remarks</span></span>

<span data-ttu-id="cb174-125">**Smtpaddress**要素は、 **publicfolderinformation**要素の必須の子要素です。</span><span class="sxs-lookup"><span data-stu-id="cb174-125">The **SmtpAddress** element is a required child element of the **PublicFolderInformation** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="cb174-126">関連項目</span><span class="sxs-lookup"><span data-stu-id="cb174-126">See also</span></span>

- [<span data-ttu-id="cb174-127">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="cb174-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

