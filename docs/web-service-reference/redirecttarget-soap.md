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
description: RedirectTarget (SOAP) 要素には、リダイレクト URL または電子メールアドレスのターゲットが含まれています。
ms.openlocfilehash: 092d575560379d43b12dd98a3efa155b59c31450
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462200"
---
# <a name="redirecttarget-soap"></a><span data-ttu-id="81346-103">RedirectTarget (SOAP)</span><span class="sxs-lookup"><span data-stu-id="81346-103">RedirectTarget (SOAP)</span></span>

<span data-ttu-id="81346-104">[Redirecttarget (SOAP)](redirecttarget-soap.md)要素には、リダイレクト URL または電子メールアドレスのターゲットが含まれています。</span><span class="sxs-lookup"><span data-stu-id="81346-104">The [RedirectTarget (SOAP)](redirecttarget-soap.md) element contains the target of the redirection URL or e-mail address.</span></span> 
  
```XML
<RedirectTarget/>
```

 <span data-ttu-id="81346-105">**string**</span><span class="sxs-lookup"><span data-stu-id="81346-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="81346-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="81346-106">Attributes and elements</span></span>

<span data-ttu-id="81346-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="81346-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="81346-108">属性</span><span class="sxs-lookup"><span data-stu-id="81346-108">Attributes</span></span>

<span data-ttu-id="81346-109">なし。</span><span class="sxs-lookup"><span data-stu-id="81346-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="81346-110">子要素</span><span class="sxs-lookup"><span data-stu-id="81346-110">Child elements</span></span>

<span data-ttu-id="81346-111">なし。</span><span class="sxs-lookup"><span data-stu-id="81346-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="81346-112">親要素</span><span class="sxs-lookup"><span data-stu-id="81346-112">Parent elements</span></span>

|<span data-ttu-id="81346-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="81346-113">**Element**</span></span>|<span data-ttu-id="81346-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="81346-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="81346-115">UserResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="81346-115">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="81346-116">個々のユーザーに対する GetUserSettings 要求への応答を表します。</span><span class="sxs-lookup"><span data-stu-id="81346-116">Represents a response to a GetUserSettings request for an individual user.</span></span>  <br/> |
|[<span data-ttu-id="81346-117">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="81346-117">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="81346-118">指定したドメインに対して要求された設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="81346-118">Contains the requested settings for the specified domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="81346-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="81346-119">Text value</span></span>

<span data-ttu-id="81346-120">テキスト値には、以降の GetUserSettings または GetDomainSettings 要求に対して使用する必要があるリダイレクト URL または電子メールアドレスのターゲットが含まれています。</span><span class="sxs-lookup"><span data-stu-id="81346-120">The text value contains the target of the redirection URL or e-mail address that should be used for a subsequent GetUserSettings or GetDomainSettings request.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="81346-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="81346-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="81346-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="81346-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="81346-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="81346-123">Schema Name</span></span>  <br/> |<span data-ttu-id="81346-124">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="81346-124">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="81346-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="81346-125">Validation File</span></span>  <br/> |<span data-ttu-id="81346-126">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="81346-126">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="81346-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="81346-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="81346-128">はい</span><span class="sxs-lookup"><span data-stu-id="81346-128">True</span></span>  <br/> |
   

