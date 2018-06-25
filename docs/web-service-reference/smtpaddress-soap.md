---
title: SmtpAddress (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: e833351c-4bd9-4937-8752-c743a7ce57ea
description: SmtpAddress 要素は、別のメールボックスの SMTP アドレスを表します。
ms.openlocfilehash: a5ece8906d337f356126f1bcb2c349699f41831d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833508"
---
# <a name="smtpaddress-soap"></a><span data-ttu-id="da02c-103">SmtpAddress (SOAP)</span><span class="sxs-lookup"><span data-stu-id="da02c-103">SmtpAddress (SOAP)</span></span>

<span data-ttu-id="da02c-104">**SmtpAddress**要素は、別のメールボックスの SMTP アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="da02c-104">The **SmtpAddress** element represents the alternate mailbox SMTP address.</span></span> 
  
```XML
<SmtpAddress/>
```

<span data-ttu-id="da02c-105">**string**</span><span class="sxs-lookup"><span data-stu-id="da02c-105">**string**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="da02c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="da02c-106">Attributes and elements</span></span>

<span data-ttu-id="da02c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="da02c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="da02c-108">属性</span><span class="sxs-lookup"><span data-stu-id="da02c-108">Attributes</span></span>

<span data-ttu-id="da02c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="da02c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="da02c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="da02c-110">Child elements</span></span>

<span data-ttu-id="da02c-111">なし。</span><span class="sxs-lookup"><span data-stu-id="da02c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="da02c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="da02c-112">Parent elements</span></span>

|<span data-ttu-id="da02c-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="da02c-113">**Element**</span></span>|<span data-ttu-id="da02c-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="da02c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="da02c-115">AlternateMailbox (SOAP)</span><span class="sxs-lookup"><span data-stu-id="da02c-115">AlternateMailbox (SOAP)</span></span>](alternatemailbox-soap.md) <br/> |<span data-ttu-id="da02c-116">別のメールボックスを表します。</span><span class="sxs-lookup"><span data-stu-id="da02c-116">Represents an alternate mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="da02c-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="da02c-117">Text value</span></span>

<span data-ttu-id="da02c-118">**SmtpAddress**要素のテキスト値は、別のメールボックスの SMTP 電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="da02c-118">The text value of the **SmtpAddress** element is the SMTP email address of the alternate mailbox.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="da02c-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="da02c-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="da02c-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="da02c-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="da02c-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="da02c-121">Schema Name</span></span>  <br/> |<span data-ttu-id="da02c-122">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="da02c-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="da02c-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="da02c-123">Validation File</span></span>  <br/> |<span data-ttu-id="da02c-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="da02c-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="da02c-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="da02c-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="da02c-126">True</span><span class="sxs-lookup"><span data-stu-id="da02c-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="da02c-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="da02c-127">See also</span></span>

- [<span data-ttu-id="da02c-128">Exchange の自動検出 web サービスの参照</span><span class="sxs-lookup"><span data-stu-id="da02c-128">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="da02c-129">Exchange 2013 の自動検出の XML 要素を SOAP</span><span class="sxs-lookup"><span data-stu-id="da02c-129">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

