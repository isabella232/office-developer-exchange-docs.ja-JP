---
title: MicrosoftOnline (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 0b88f02a-9c50-44b3-841b-560b24e37af5
description: MicrosoftOnline 要素には、Office 365 の一部としてかどうかユーザーのメールボックスがホストされている Exchange オンラインまたは Exchange Online を示す値が含まれています。
ms.openlocfilehash: b952bfda17b30dcf29812697d225db32718d9781
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832458"
---
# <a name="microsoftonline-pox"></a><span data-ttu-id="f6c23-103">MicrosoftOnline (POX)</span><span class="sxs-lookup"><span data-stu-id="f6c23-103">MicrosoftOnline (POX)</span></span>

<span data-ttu-id="f6c23-104">**MicrosoftOnline**要素には、Office 365 の一部としてかどうかユーザーのメールボックスがホストされている Exchange オンラインまたは Exchange Online を示す値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f6c23-104">The **MicrosoftOnline** element contains a value that indicates whether the user's mailbox is hosted in Exchange Online or Exchange Online as part of Office 365.</span></span> 
  
[<span data-ttu-id="f6c23-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="f6c23-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="f6c23-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="f6c23-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="f6c23-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="f6c23-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="f6c23-108">MicrosoftOnline (POX)</span><span class="sxs-lookup"><span data-stu-id="f6c23-108">MicrosoftOnline (POX)</span></span>](microsoftonline-pox.md)
  
```XML
<MicrosoftOnline/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="f6c23-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f6c23-109">Attributes and elements</span></span>

<span data-ttu-id="f6c23-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f6c23-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f6c23-111">属性</span><span class="sxs-lookup"><span data-stu-id="f6c23-111">Attributes</span></span>

<span data-ttu-id="f6c23-112">なし。</span><span class="sxs-lookup"><span data-stu-id="f6c23-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f6c23-113">子要素</span><span class="sxs-lookup"><span data-stu-id="f6c23-113">Child elements</span></span>

<span data-ttu-id="f6c23-114">なし。</span><span class="sxs-lookup"><span data-stu-id="f6c23-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f6c23-115">親要素</span><span class="sxs-lookup"><span data-stu-id="f6c23-115">Parent elements</span></span>

|<span data-ttu-id="f6c23-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="f6c23-116">**Element**</span></span>|<span data-ttu-id="f6c23-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="f6c23-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f6c23-118">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="f6c23-118">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="f6c23-119">ユーザーのアカウントの設定を指定またはエラー応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f6c23-119">Specifies account settings for the user or contains error responses.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f6c23-120">備考</span><span class="sxs-lookup"><span data-stu-id="f6c23-120">Remarks</span></span>

<span data-ttu-id="f6c23-121">テキスト値は、Exchange Online でユーザーのメールボックスがホストされているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f6c23-121">The text value indicates whether the user's mailbox is hosted in Exchange Online.</span></span> <span data-ttu-id="f6c23-122">値は、 **true の**場合、ユーザーのメールボックスがホストされている Exchange オンラインです。それ以外の場合、 **false を指定**します。</span><span class="sxs-lookup"><span data-stu-id="f6c23-122">The value is **true** if the user's mailbox is hosted in Exchange Online; otherwise, **false**.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="f6c23-123">関連項目</span><span class="sxs-lookup"><span data-stu-id="f6c23-123">See also</span></span>



[<span data-ttu-id="f6c23-124">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="f6c23-124">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

