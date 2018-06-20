---
title: ユーザー (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 4e051617-4eea-47d0-871a-ea1f17a0f711
description: ユーザーの要素は、設定を取得する対象となるユーザーの電子メール アドレスのコレクションを表します。
ms.openlocfilehash: d7655f0020a315dcb32adbbc58610ca0e630c1fc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839952"
---
# <a name="users-soap"></a><span data-ttu-id="d324e-103">ユーザー (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d324e-103">Users (SOAP)</span></span>

<span data-ttu-id="d324e-104">**ユーザー**の要素は、設定を取得する対象となるユーザーの電子メール アドレスのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="d324e-104">The **Users** element represents a collection of e-mail addresses of the users for whom settings should be retrieved.</span></span> 
  
```XML
<Users>
   <User/>
</Users>
```

 <span data-ttu-id="d324e-105">**Users**</span><span class="sxs-lookup"><span data-stu-id="d324e-105">**Users**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d324e-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d324e-106">Attributes and elements</span></span>

<span data-ttu-id="d324e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d324e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d324e-108">属性</span><span class="sxs-lookup"><span data-stu-id="d324e-108">Attributes</span></span>

<span data-ttu-id="d324e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d324e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d324e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d324e-110">Child elements</span></span>

|<span data-ttu-id="d324e-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="d324e-111">**Element**</span></span>|<span data-ttu-id="d324e-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d324e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d324e-113">ユーザー (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d324e-113">User (SOAP)</span></span>](user-soap.md) <br/> |<span data-ttu-id="d324e-114">ユーザーの電子メール アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="d324e-114">Represents the e-mail address of a user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d324e-115">親要素</span><span class="sxs-lookup"><span data-stu-id="d324e-115">Parent elements</span></span>

|<span data-ttu-id="d324e-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="d324e-116">**Element**</span></span>|<span data-ttu-id="d324e-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="d324e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d324e-118">GetUserSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d324e-118">GetUserSettingsRequest (SOAP)</span></span>](getusersettingsrequest-soap.md) <br/> |<span data-ttu-id="d324e-119">1 つまたは複数のユーザーに対して指定した設定を取得する要求を表します。</span><span class="sxs-lookup"><span data-stu-id="d324e-119">Represents a request to retrieve specified settings for one or more users.</span></span>  <br/> |
|[<span data-ttu-id="d324e-120">要求 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d324e-120">Request (SOAP)</span></span>](request-soap.md) <br/> |<span data-ttu-id="d324e-121">要求された構成設定とユーザーを対象に含まれています。</span><span class="sxs-lookup"><span data-stu-id="d324e-121">Contains the requested configuration settings and the target users.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d324e-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d324e-122">Text value</span></span>

<span data-ttu-id="d324e-123">なし。</span><span class="sxs-lookup"><span data-stu-id="d324e-123">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d324e-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="d324e-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d324e-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="d324e-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="d324e-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d324e-126">Schema Name</span></span>  <br/> |<span data-ttu-id="d324e-127">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="d324e-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="d324e-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d324e-128">Validation File</span></span>  <br/> |<span data-ttu-id="d324e-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d324e-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d324e-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d324e-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="d324e-131">True</span><span class="sxs-lookup"><span data-stu-id="d324e-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d324e-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="d324e-132">See also</span></span>



[<span data-ttu-id="d324e-133">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d324e-133">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

