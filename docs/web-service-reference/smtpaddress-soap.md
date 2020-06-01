---
title: SmtpAddress (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: e833351c-4bd9-4937-8752-c743a7ce57ea
description: SmtpAddress 要素は、代替メールボックス SMTP アドレスを表します。
ms.openlocfilehash: 53238caef1287536de838f4167e8937c182b41b0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459014"
---
# <a name="smtpaddress-soap"></a><span data-ttu-id="d7fc7-103">SmtpAddress (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d7fc7-103">SmtpAddress (SOAP)</span></span>

<span data-ttu-id="d7fc7-104">**Smtpaddress**要素は、代替メールボックス SMTP アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="d7fc7-104">The **SmtpAddress** element represents the alternate mailbox SMTP address.</span></span> 
  
```XML
<SmtpAddress/>
```

<span data-ttu-id="d7fc7-105">**string**</span><span class="sxs-lookup"><span data-stu-id="d7fc7-105">**string**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d7fc7-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d7fc7-106">Attributes and elements</span></span>

<span data-ttu-id="d7fc7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d7fc7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d7fc7-108">属性</span><span class="sxs-lookup"><span data-stu-id="d7fc7-108">Attributes</span></span>

<span data-ttu-id="d7fc7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d7fc7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d7fc7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d7fc7-110">Child elements</span></span>

<span data-ttu-id="d7fc7-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d7fc7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d7fc7-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d7fc7-112">Parent elements</span></span>

|<span data-ttu-id="d7fc7-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="d7fc7-113">**Element**</span></span>|<span data-ttu-id="d7fc7-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="d7fc7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d7fc7-115">AlternateMailbox (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d7fc7-115">AlternateMailbox (SOAP)</span></span>](alternatemailbox-soap.md) <br/> |<span data-ttu-id="d7fc7-116">代替メールボックスを表します。</span><span class="sxs-lookup"><span data-stu-id="d7fc7-116">Represents an alternate mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d7fc7-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d7fc7-117">Text value</span></span>

<span data-ttu-id="d7fc7-118">**Smtpaddress**要素のテキスト値は、代替メールボックスの SMTP 電子メールアドレスです。</span><span class="sxs-lookup"><span data-stu-id="d7fc7-118">The text value of the **SmtpAddress** element is the SMTP email address of the alternate mailbox.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="d7fc7-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d7fc7-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d7fc7-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="d7fc7-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="d7fc7-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d7fc7-121">Schema Name</span></span>  <br/> |<span data-ttu-id="d7fc7-122">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="d7fc7-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="d7fc7-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d7fc7-123">Validation File</span></span>  <br/> |<span data-ttu-id="d7fc7-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="d7fc7-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d7fc7-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d7fc7-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="d7fc7-126">正しい</span><span class="sxs-lookup"><span data-stu-id="d7fc7-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d7fc7-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="d7fc7-127">See also</span></span>

- [<span data-ttu-id="d7fc7-128">Exchange 用自動検出 Web サービス リファレンス</span><span class="sxs-lookup"><span data-stu-id="d7fc7-128">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="d7fc7-129">Exchange 2013 の SOAP 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="d7fc7-129">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

