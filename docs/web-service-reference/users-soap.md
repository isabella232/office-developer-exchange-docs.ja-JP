---
title: Users (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 4e051617-4eea-47d0-871a-ea1f17a0f711
description: Users 要素は、設定を取得する必要があるユーザーの電子メールアドレスのコレクションを表します。
ms.openlocfilehash: 851447a2918e365b7c5d8812a61c9d425d26ffa2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461899"
---
# <a name="users-soap"></a><span data-ttu-id="efd59-103">Users (SOAP)</span><span class="sxs-lookup"><span data-stu-id="efd59-103">Users (SOAP)</span></span>

<span data-ttu-id="efd59-104">**Users**要素は、設定を取得する必要があるユーザーの電子メールアドレスのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="efd59-104">The **Users** element represents a collection of e-mail addresses of the users for whom settings should be retrieved.</span></span> 
  
```XML
<Users>
   <User/>
</Users>
```

 <span data-ttu-id="efd59-105">**Users**</span><span class="sxs-lookup"><span data-stu-id="efd59-105">**Users**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="efd59-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="efd59-106">Attributes and elements</span></span>

<span data-ttu-id="efd59-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="efd59-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="efd59-108">属性</span><span class="sxs-lookup"><span data-stu-id="efd59-108">Attributes</span></span>

<span data-ttu-id="efd59-109">なし。</span><span class="sxs-lookup"><span data-stu-id="efd59-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="efd59-110">子要素</span><span class="sxs-lookup"><span data-stu-id="efd59-110">Child elements</span></span>

|<span data-ttu-id="efd59-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="efd59-111">**Element**</span></span>|<span data-ttu-id="efd59-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="efd59-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="efd59-113">User (SOAP)</span><span class="sxs-lookup"><span data-stu-id="efd59-113">User (SOAP)</span></span>](user-soap.md) <br/> |<span data-ttu-id="efd59-114">ユーザーの電子メールアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="efd59-114">Represents the e-mail address of a user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="efd59-115">親要素</span><span class="sxs-lookup"><span data-stu-id="efd59-115">Parent elements</span></span>

|<span data-ttu-id="efd59-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="efd59-116">**Element**</span></span>|<span data-ttu-id="efd59-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="efd59-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="efd59-118">GetUserSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="efd59-118">GetUserSettingsRequest (SOAP)</span></span>](getusersettingsrequest-soap.md) <br/> |<span data-ttu-id="efd59-119">1人または複数のユーザーに対して指定された設定を取得する要求を表します。</span><span class="sxs-lookup"><span data-stu-id="efd59-119">Represents a request to retrieve specified settings for one or more users.</span></span>  <br/> |
|[<span data-ttu-id="efd59-120">要求 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="efd59-120">Request (SOAP)</span></span>](request-soap.md) <br/> |<span data-ttu-id="efd59-121">要求された構成設定と対象ユーザーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="efd59-121">Contains the requested configuration settings and the target users.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="efd59-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="efd59-122">Text value</span></span>

<span data-ttu-id="efd59-123">なし。</span><span class="sxs-lookup"><span data-stu-id="efd59-123">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="efd59-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="efd59-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="efd59-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="efd59-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="efd59-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="efd59-126">Schema Name</span></span>  <br/> |<span data-ttu-id="efd59-127">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="efd59-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="efd59-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="efd59-128">Validation File</span></span>  <br/> |<span data-ttu-id="efd59-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="efd59-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="efd59-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="efd59-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="efd59-131">正しい</span><span class="sxs-lookup"><span data-stu-id="efd59-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="efd59-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="efd59-132">See also</span></span>



[<span data-ttu-id="efd59-133">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="efd59-133">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

