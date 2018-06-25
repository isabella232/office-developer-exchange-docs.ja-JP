---
title: ユーザー (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: c6bc0031-bc1d-41bd-84e4-9074a5b77012
description: ユーザー要素は、1 人のユーザーの id を表します。
ms.openlocfilehash: a8dcb22f5c74a9622f978f34e48146115351fe82
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839923"
---
# <a name="user-soap"></a><span data-ttu-id="fe6e7-103">ユーザー (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fe6e7-103">User (SOAP)</span></span>

<span data-ttu-id="fe6e7-104">**ユーザー**要素は、1 人のユーザーの id を表します。</span><span class="sxs-lookup"><span data-stu-id="fe6e7-104">The **User** element represents the identity of a single user.</span></span> 
  
```XML
<User>
    <LegacyDN/>
    <Mailbox/>
    <RequestedSettings/>
</User>
```

 <span data-ttu-id="fe6e7-105">**User**</span><span class="sxs-lookup"><span data-stu-id="fe6e7-105">**User**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fe6e7-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="fe6e7-106">Attributes and elements</span></span>

<span data-ttu-id="fe6e7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fe6e7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fe6e7-108">属性</span><span class="sxs-lookup"><span data-stu-id="fe6e7-108">Attributes</span></span>

<span data-ttu-id="fe6e7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="fe6e7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fe6e7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="fe6e7-110">Child elements</span></span>

|<span data-ttu-id="fe6e7-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="fe6e7-111">**Element**</span></span>|<span data-ttu-id="fe6e7-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="fe6e7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fe6e7-113">LegacyDN (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fe6e7-113">LegacyDN (SOAP)</span></span>](legacydn-soap.md) <br/> |<span data-ttu-id="fe6e7-114">代替メールボックスの従来の識別名を表します。</span><span class="sxs-lookup"><span data-stu-id="fe6e7-114">Represents the alternate mailbox legacy distinguished name.</span></span>  <br/> |
|[<span data-ttu-id="fe6e7-115">メールボックス (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fe6e7-115">Mailbox (SOAP)</span></span>](mailbox-soap.md) <br/> |<span data-ttu-id="fe6e7-116">検出するユーザーの電子メール アドレスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="fe6e7-116">Contains the e-mail address of the user to be discovered.</span></span>  <br/> |
|[<span data-ttu-id="fe6e7-117">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fe6e7-117">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="fe6e7-118">要求された構成設定の名前が含まれています。</span><span class="sxs-lookup"><span data-stu-id="fe6e7-118">Contains the names of the requested configuration settings.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fe6e7-119">親要素</span><span class="sxs-lookup"><span data-stu-id="fe6e7-119">Parent elements</span></span>

|<span data-ttu-id="fe6e7-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="fe6e7-120">**Element**</span></span>|<span data-ttu-id="fe6e7-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="fe6e7-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fe6e7-122">ユーザー (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fe6e7-122">Users (SOAP)</span></span>](users-soap.md) <br/> |<span data-ttu-id="fe6e7-123">**ユーザー**要素のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="fe6e7-123">Represents a collection of **User** elements.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fe6e7-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="fe6e7-124">Text value</span></span>

<span data-ttu-id="fe6e7-125">なし。</span><span class="sxs-lookup"><span data-stu-id="fe6e7-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fe6e7-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="fe6e7-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fe6e7-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="fe6e7-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="fe6e7-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fe6e7-128">Schema Name</span></span>  <br/> |<span data-ttu-id="fe6e7-129">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="fe6e7-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="fe6e7-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fe6e7-130">Validation File</span></span>  <br/> |<span data-ttu-id="fe6e7-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fe6e7-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fe6e7-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="fe6e7-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="fe6e7-133">True</span><span class="sxs-lookup"><span data-stu-id="fe6e7-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fe6e7-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="fe6e7-134">See also</span></span>



[<span data-ttu-id="fe6e7-135">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fe6e7-135">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="fe6e7-136">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fe6e7-136">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="fe6e7-137">GetFederationInformation 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fe6e7-137">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

