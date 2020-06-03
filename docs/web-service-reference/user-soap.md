---
title: User (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: c6bc0031-bc1d-41bd-84e4-9074a5b77012
description: User 要素は、1人のユーザーの id を表します。
ms.openlocfilehash: f151ffa8050a10cdbb4562471d815f8692596cc3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456347"
---
# <a name="user-soap"></a><span data-ttu-id="68342-103">User (SOAP)</span><span class="sxs-lookup"><span data-stu-id="68342-103">User (SOAP)</span></span>

<span data-ttu-id="68342-104">**User**要素は、1人のユーザーの id を表します。</span><span class="sxs-lookup"><span data-stu-id="68342-104">The **User** element represents the identity of a single user.</span></span> 
  
```XML
<User>
    <LegacyDN/>
    <Mailbox/>
    <RequestedSettings/>
</User>
```

 <span data-ttu-id="68342-105">**ユーザー**</span><span class="sxs-lookup"><span data-stu-id="68342-105">**User**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="68342-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="68342-106">Attributes and elements</span></span>

<span data-ttu-id="68342-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="68342-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="68342-108">属性</span><span class="sxs-lookup"><span data-stu-id="68342-108">Attributes</span></span>

<span data-ttu-id="68342-109">なし。</span><span class="sxs-lookup"><span data-stu-id="68342-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="68342-110">子要素</span><span class="sxs-lookup"><span data-stu-id="68342-110">Child elements</span></span>

|<span data-ttu-id="68342-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="68342-111">**Element**</span></span>|<span data-ttu-id="68342-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="68342-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="68342-113">LegacyDN (SOAP)</span><span class="sxs-lookup"><span data-stu-id="68342-113">LegacyDN (SOAP)</span></span>](legacydn-soap.md) <br/> |<span data-ttu-id="68342-114">代替メールボックスの従来の識別名を表します。</span><span class="sxs-lookup"><span data-stu-id="68342-114">Represents the alternate mailbox legacy distinguished name.</span></span>  <br/> |
|[<span data-ttu-id="68342-115">メールボックス (SOAP)</span><span class="sxs-lookup"><span data-stu-id="68342-115">Mailbox (SOAP)</span></span>](mailbox-soap.md) <br/> |<span data-ttu-id="68342-116">検索するユーザーの電子メールアドレスが含まれます。</span><span class="sxs-lookup"><span data-stu-id="68342-116">Contains the e-mail address of the user to be discovered.</span></span>  <br/> |
|[<span data-ttu-id="68342-117">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="68342-117">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="68342-118">要求された構成設定の名前が含まれています。</span><span class="sxs-lookup"><span data-stu-id="68342-118">Contains the names of the requested configuration settings.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="68342-119">親要素</span><span class="sxs-lookup"><span data-stu-id="68342-119">Parent elements</span></span>

|<span data-ttu-id="68342-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="68342-120">**Element**</span></span>|<span data-ttu-id="68342-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="68342-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="68342-122">Users (SOAP)</span><span class="sxs-lookup"><span data-stu-id="68342-122">Users (SOAP)</span></span>](users-soap.md) <br/> |<span data-ttu-id="68342-123">**ユーザー**要素のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="68342-123">Represents a collection of **User** elements.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="68342-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="68342-124">Text value</span></span>

<span data-ttu-id="68342-125">なし。</span><span class="sxs-lookup"><span data-stu-id="68342-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="68342-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="68342-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="68342-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="68342-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="68342-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="68342-128">Schema Name</span></span>  <br/> |<span data-ttu-id="68342-129">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="68342-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="68342-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="68342-130">Validation File</span></span>  <br/> |<span data-ttu-id="68342-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="68342-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="68342-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="68342-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="68342-133">正しい</span><span class="sxs-lookup"><span data-stu-id="68342-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="68342-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="68342-134">See also</span></span>



[<span data-ttu-id="68342-135">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="68342-135">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="68342-136">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="68342-136">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="68342-137">GetFederationInformation 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="68342-137">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

