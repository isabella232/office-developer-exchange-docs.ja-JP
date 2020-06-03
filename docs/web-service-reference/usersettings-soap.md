---
title: UserSettings (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: ac3b827c-2e46-49ef-8c5a-f88084c0a12c
description: UserSettings 要素は、ユーザー設定のコレクションを表します。
ms.openlocfilehash: 0e1627d4ef42db4e3bd2f4d841bea29fcf947a82
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530283"
---
# <a name="usersettings-soap"></a><span data-ttu-id="4ccf4-103">UserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4ccf4-103">UserSettings (SOAP)</span></span>

<span data-ttu-id="4ccf4-104">**UserSettings**要素は、ユーザー設定のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="4ccf4-104">The **UserSettings** element represents a collection of user settings.</span></span> 
  
```XML
<UserSettings>
    <UserSetting/>
</UserSettings>
```

 <span data-ttu-id="4ccf4-105">**UserSettings**</span><span class="sxs-lookup"><span data-stu-id="4ccf4-105">**UserSettings**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4ccf4-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="4ccf4-106">Attributes and elements</span></span>

<span data-ttu-id="4ccf4-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4ccf4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4ccf4-108">属性</span><span class="sxs-lookup"><span data-stu-id="4ccf4-108">Attributes</span></span>

<span data-ttu-id="4ccf4-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4ccf4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4ccf4-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4ccf4-110">Child elements</span></span>

|<span data-ttu-id="4ccf4-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="4ccf4-111">**Element**</span></span>|<span data-ttu-id="4ccf4-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="4ccf4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4ccf4-113">UserSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4ccf4-113">UserSetting (SOAP)</span></span>](usersetting-soap.md) <br/> |<span data-ttu-id="4ccf4-114">1つのユーザー設定を表します。</span><span class="sxs-lookup"><span data-stu-id="4ccf4-114">Represents a single user setting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4ccf4-115">親要素</span><span class="sxs-lookup"><span data-stu-id="4ccf4-115">Parent elements</span></span>

|<span data-ttu-id="4ccf4-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="4ccf4-116">**Element**</span></span>|<span data-ttu-id="4ccf4-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="4ccf4-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4ccf4-118">UserResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4ccf4-118">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="4ccf4-119">個々のユーザーに対する GetUserSettings 要求への応答を表します。</span><span class="sxs-lookup"><span data-stu-id="4ccf4-119">Represents a response to a GetUserSettings request for an individual user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4ccf4-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="4ccf4-120">Text value</span></span>

<span data-ttu-id="4ccf4-121">なし。</span><span class="sxs-lookup"><span data-stu-id="4ccf4-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4ccf4-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="4ccf4-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4ccf4-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="4ccf4-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="4ccf4-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4ccf4-124">Schema Name</span></span>  <br/> |<span data-ttu-id="4ccf4-125">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="4ccf4-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="4ccf4-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4ccf4-126">Validation File</span></span>  <br/> |<span data-ttu-id="4ccf4-127">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="4ccf4-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4ccf4-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4ccf4-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="4ccf4-129">正しい</span><span class="sxs-lookup"><span data-stu-id="4ccf4-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4ccf4-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="4ccf4-130">See also</span></span>



[<span data-ttu-id="4ccf4-131">Exchange 2013 の SOAP 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="4ccf4-131">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

