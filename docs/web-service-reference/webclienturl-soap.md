---
title: WebClientUrl (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 7f8cb6d6-4aac-4a1f-8bec-2dcb90fc1df6
description: WebClientUrl 要素は、Exchange web クライアントの URL を表します。
ms.openlocfilehash: 649845018acee1706a96f9e37475a6d5c5fa0aa7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840014"
---
# <a name="webclienturl-soap"></a><span data-ttu-id="4cf16-103">WebClientUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4cf16-103">WebClientUrl (SOAP)</span></span>

<span data-ttu-id="4cf16-104">**WebClientUrl**要素は、Exchange web クライアントの URL を表します。</span><span class="sxs-lookup"><span data-stu-id="4cf16-104">The **WebClientUrl** element represents the URL of an Exchange web client.</span></span> 
  
[<span data-ttu-id="4cf16-105">UserSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4cf16-105">UserSetting (SOAP)</span></span>](usersetting-soap.md)
  
[<span data-ttu-id="4cf16-106">WebClientUrls (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4cf16-106">WebClientUrls (SOAP)</span></span>](webclienturls-soap.md)
  
[<span data-ttu-id="4cf16-107">WebClientUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4cf16-107">WebClientUrl (SOAP)</span></span>](webclienturl-soap.md)
  
```XML
<WebClientUrl>
    <AuthenticationMethods/>
    <Url/>
</WebClientUrl>
```

 <span data-ttu-id="4cf16-108">**WebClientUrl**</span><span class="sxs-lookup"><span data-stu-id="4cf16-108">**WebClientUrl**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4cf16-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4cf16-109">Attributes and elements</span></span>

<span data-ttu-id="4cf16-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4cf16-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4cf16-111">属性</span><span class="sxs-lookup"><span data-stu-id="4cf16-111">Attributes</span></span>

<span data-ttu-id="4cf16-112">なし。</span><span class="sxs-lookup"><span data-stu-id="4cf16-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4cf16-113">子要素</span><span class="sxs-lookup"><span data-stu-id="4cf16-113">Child elements</span></span>

|<span data-ttu-id="4cf16-114">**要素**</span><span class="sxs-lookup"><span data-stu-id="4cf16-114">**Element**</span></span>|<span data-ttu-id="4cf16-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="4cf16-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4cf16-116">AuthenticationMethods (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4cf16-116">AuthenticationMethods (SOAP)</span></span>](authenticationmethods-soap.md) <br/> |<span data-ttu-id="4cf16-117">指定した URL にアクセスするときに使用する認証メソッドを表します。</span><span class="sxs-lookup"><span data-stu-id="4cf16-117">Represents the authentication method to use when accessing the specified URL.</span></span>  <br/> |
|[<span data-ttu-id="4cf16-118">Url (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4cf16-118">Url (SOAP)</span></span>](url-soap.md) <br/> |<span data-ttu-id="4cf16-119">URL の web アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="4cf16-119">Represents the web address for the URL.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4cf16-120">親要素</span><span class="sxs-lookup"><span data-stu-id="4cf16-120">Parent elements</span></span>

|<span data-ttu-id="4cf16-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="4cf16-121">**Element**</span></span>|<span data-ttu-id="4cf16-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="4cf16-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4cf16-123">WebClientUrls (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4cf16-123">WebClientUrls (SOAP)</span></span>](webclienturls-soap.md) <br/> |<span data-ttu-id="4cf16-124">**WebClientUrl**要素のコレクションを含むユーザー設定を表します。</span><span class="sxs-lookup"><span data-stu-id="4cf16-124">Represents a user setting that contains a collection of **WebClientUrl** elements.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="4cf16-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="4cf16-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4cf16-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="4cf16-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="4cf16-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4cf16-127">Schema Name</span></span>  <br/> |<span data-ttu-id="4cf16-128">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="4cf16-128">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="4cf16-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4cf16-129">Validation File</span></span>  <br/> |<span data-ttu-id="4cf16-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4cf16-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4cf16-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4cf16-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="4cf16-132">True</span><span class="sxs-lookup"><span data-stu-id="4cf16-132">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4cf16-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="4cf16-133">See also</span></span>



[<span data-ttu-id="4cf16-134">Url (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4cf16-134">Url (SOAP)</span></span>](url-soap.md)
  
[<span data-ttu-id="4cf16-135">WebClientUrls (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4cf16-135">WebClientUrls (SOAP)</span></span>](webclienturls-soap.md)

