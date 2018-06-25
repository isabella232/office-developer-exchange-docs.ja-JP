---
title: RedirectTarget (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: f8162724-cf9a-4543-a1ad-5846c8b10bfa
description: RedirectTarget (SOAP) の要素には、リダイレクト URL または電子メール アドレスのターゲットが含まれています。
ms.openlocfilehash: 3a8a0c39c6889730c9d17778c6a26f84fcbcd4a7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833019"
---
# <a name="redirecttarget-soap"></a><span data-ttu-id="c140e-103">RedirectTarget (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c140e-103">RedirectTarget (SOAP)</span></span>

<span data-ttu-id="c140e-104">[RedirectTarget (SOAP)](redirecttarget-soap.md)の要素には、リダイレクト URL または電子メール アドレスのターゲットが含まれています。</span><span class="sxs-lookup"><span data-stu-id="c140e-104">The [RedirectTarget (SOAP)](redirecttarget-soap.md) element contains the target of the redirection URL or e-mail address.</span></span> 
  
```XML
<RedirectTarget/>
```

 <span data-ttu-id="c140e-105">**string**</span><span class="sxs-lookup"><span data-stu-id="c140e-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c140e-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="c140e-106">Attributes and elements</span></span>

<span data-ttu-id="c140e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c140e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c140e-108">属性</span><span class="sxs-lookup"><span data-stu-id="c140e-108">Attributes</span></span>

<span data-ttu-id="c140e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c140e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c140e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c140e-110">Child elements</span></span>

<span data-ttu-id="c140e-111">なし。</span><span class="sxs-lookup"><span data-stu-id="c140e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c140e-112">親要素</span><span class="sxs-lookup"><span data-stu-id="c140e-112">Parent elements</span></span>

|<span data-ttu-id="c140e-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="c140e-113">**Element**</span></span>|<span data-ttu-id="c140e-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="c140e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c140e-115">UserResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c140e-115">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="c140e-116">個々 のユーザーの GetUserSettings の要求に対する応答を表します。</span><span class="sxs-lookup"><span data-stu-id="c140e-116">Represents a response to a GetUserSettings request for an individual user.</span></span>  <br/> |
|[<span data-ttu-id="c140e-117">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c140e-117">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="c140e-118">指定したドメインの指定された設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c140e-118">Contains the requested settings for the specified domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c140e-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c140e-119">Text value</span></span>

<span data-ttu-id="c140e-120">テキスト値には、それ以降の GetUserSettings に使用するリダイレクト URL または電子メール アドレスのターゲットが含まれているか、GetDomainSettings を要求します。</span><span class="sxs-lookup"><span data-stu-id="c140e-120">The text value contains the target of the redirection URL or e-mail address that should be used for a subsequent GetUserSettings or GetDomainSettings request.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c140e-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="c140e-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c140e-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="c140e-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="c140e-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c140e-123">Schema Name</span></span>  <br/> |<span data-ttu-id="c140e-124">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="c140e-124">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="c140e-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c140e-125">Validation File</span></span>  <br/> |<span data-ttu-id="c140e-126">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c140e-126">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c140e-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c140e-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="c140e-128">True</span><span class="sxs-lookup"><span data-stu-id="c140e-128">True</span></span>  <br/> |
   

