---
title: Microsoft Online (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 0b88f02a-9c50-44b3-841b-560b24e37af5
description: Microsoft Office Online 要素には、ユーザーのメールボックスが Office 365 の一部として Exchange Online または Exchange Online でホストされているかどうかを示す値が含まれています。
ms.openlocfilehash: f3144a673a4c98aad821e21c562141b0ae00f426
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467985"
---
# <a name="microsoftonline-pox"></a><span data-ttu-id="5850e-103">Microsoft Online (POX)</span><span class="sxs-lookup"><span data-stu-id="5850e-103">MicrosoftOnline (POX)</span></span>

<span data-ttu-id="5850e-104">**Microsoft Office online**要素には、ユーザーのメールボックスが Office 365 の一部として exchange online または exchange online でホストされているかどうかを示す値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5850e-104">The **MicrosoftOnline** element contains a value that indicates whether the user's mailbox is hosted in Exchange Online or Exchange Online as part of Office 365.</span></span> 
  
[<span data-ttu-id="5850e-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="5850e-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="5850e-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="5850e-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="5850e-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="5850e-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="5850e-108">Microsoft Online (POX)</span><span class="sxs-lookup"><span data-stu-id="5850e-108">MicrosoftOnline (POX)</span></span>](microsoftonline-pox.md)
  
```XML
<MicrosoftOnline/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="5850e-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="5850e-109">Attributes and elements</span></span>

<span data-ttu-id="5850e-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5850e-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5850e-111">属性</span><span class="sxs-lookup"><span data-stu-id="5850e-111">Attributes</span></span>

<span data-ttu-id="5850e-112">なし。</span><span class="sxs-lookup"><span data-stu-id="5850e-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5850e-113">子要素</span><span class="sxs-lookup"><span data-stu-id="5850e-113">Child elements</span></span>

<span data-ttu-id="5850e-114">なし。</span><span class="sxs-lookup"><span data-stu-id="5850e-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5850e-115">親要素</span><span class="sxs-lookup"><span data-stu-id="5850e-115">Parent elements</span></span>

|<span data-ttu-id="5850e-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="5850e-116">**Element**</span></span>|<span data-ttu-id="5850e-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="5850e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5850e-118">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="5850e-118">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="5850e-119">ユーザーのアカウント設定を指定します。または、エラー応答を含みます。</span><span class="sxs-lookup"><span data-stu-id="5850e-119">Specifies account settings for the user or contains error responses.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5850e-120">注釈</span><span class="sxs-lookup"><span data-stu-id="5850e-120">Remarks</span></span>

<span data-ttu-id="5850e-121">テキスト値は、ユーザーのメールボックスが Exchange Online でホストされているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5850e-121">The text value indicates whether the user's mailbox is hosted in Exchange Online.</span></span> <span data-ttu-id="5850e-122">この値は、ユーザーのメールボックスが Exchange Online でホストされている場合は**true**です。それ以外の場合は**false**。</span><span class="sxs-lookup"><span data-stu-id="5850e-122">The value is **true** if the user's mailbox is hosted in Exchange Online; otherwise, **false**.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="5850e-123">関連項目</span><span class="sxs-lookup"><span data-stu-id="5850e-123">See also</span></span>



[<span data-ttu-id="5850e-124">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="5850e-124">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

