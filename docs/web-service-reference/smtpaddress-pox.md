---
title: SmtpAddress (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 984ccd97-c337-47b6-ba42-3405a8b55a71
description: SmtpAddress 要素には、ユーザー用に構成するパブリック フォルダーのメッセージ ストアに割り当てられている SMTP アドレスが含まれています。
ms.openlocfilehash: 43ebb328e31cdec11412e80b743d4d4393b7960a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833507"
---
# <a name="smtpaddress-pox"></a><span data-ttu-id="cba5d-103">SmtpAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="cba5d-103">SmtpAddress (POX)</span></span>

<span data-ttu-id="cba5d-104">**SmtpAddress**要素には、ユーザー用に構成するパブリック フォルダーのメッセージ ストアに割り当てられている SMTP アドレスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="cba5d-104">The **SmtpAddress** element contains the SMTP address assigned to the public folder message store configured for the user.</span></span> 
  
- [<span data-ttu-id="cba5d-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="cba5d-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
- [<span data-ttu-id="cba5d-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="cba5d-106">Response (POX)</span></span>](response-pox.md)
  
- [<span data-ttu-id="cba5d-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="cba5d-107">Account (POX)</span></span>](account-pox.md)
  
- [<span data-ttu-id="cba5d-108">PublicFolderInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="cba5d-108">PublicFolderInformation (POX)</span></span>](publicfolderinformation-pox.md)
  
- [<span data-ttu-id="cba5d-109">SmtpAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="cba5d-109">SmtpAddress (POX)</span></span>](smtpaddress-pox.md)
  
```XML
<SmtpAddress/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="cba5d-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="cba5d-110">Attributes and elements</span></span>

<span data-ttu-id="cba5d-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cba5d-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cba5d-112">属性</span><span class="sxs-lookup"><span data-stu-id="cba5d-112">Attributes</span></span>

<span data-ttu-id="cba5d-113">なし。</span><span class="sxs-lookup"><span data-stu-id="cba5d-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cba5d-114">子要素</span><span class="sxs-lookup"><span data-stu-id="cba5d-114">Child elements</span></span>

<span data-ttu-id="cba5d-115">なし。</span><span class="sxs-lookup"><span data-stu-id="cba5d-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cba5d-116">親要素</span><span class="sxs-lookup"><span data-stu-id="cba5d-116">Parent elements</span></span>

|<span data-ttu-id="cba5d-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="cba5d-117">**Element**</span></span>|<span data-ttu-id="cba5d-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="cba5d-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cba5d-119">PublicFolderInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="cba5d-119">PublicFolderInformation (POX)</span></span>](publicfolderinformation-pox.md) <br/> |<span data-ttu-id="cba5d-120">クライアント ユーザーのパブリック フォルダー情報を検出する自動検出要求の送信に使用できる情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cba5d-120">Contains information that clients can use to send an Autodiscover request to discover public folder information for the user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cba5d-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="cba5d-121">Text value</span></span>

<span data-ttu-id="cba5d-122">テキスト値は、ユーザー用に構成するパブリック フォルダー ストアに割り当てられている SMTP アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="cba5d-122">The text value represents the SMTP address assigned to the public folder store configured for the user.</span></span> <span data-ttu-id="cba5d-123">この SMTP アドレスは、パブリック フォルダーの設定を検出する自動検出要求の[EMailAddress (POX)](emailaddress-pox.md)要素で使用できます。</span><span class="sxs-lookup"><span data-stu-id="cba5d-123">This SMTP address can be used in the [EMailAddress (POX)](emailaddress-pox.md) element of an Autodiscover request to discover public folder settings.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="cba5d-124">備考</span><span class="sxs-lookup"><span data-stu-id="cba5d-124">Remarks</span></span>

<span data-ttu-id="cba5d-125">**SmtpAddress**要素は、 **PublicFolderInformation**要素の必須の子要素です。</span><span class="sxs-lookup"><span data-stu-id="cba5d-125">The **SmtpAddress** element is a required child element of the **PublicFolderInformation** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="cba5d-126">関連項目</span><span class="sxs-lookup"><span data-stu-id="cba5d-126">See also</span></span>

- [<span data-ttu-id="cba5d-127">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="cba5d-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

