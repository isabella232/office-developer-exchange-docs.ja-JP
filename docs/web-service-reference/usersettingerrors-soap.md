---
title: UserSettingErrors (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a9b94bae-cab9-412d-a811-801e849ed6c5
description: UserSettingErrors 要素は、返されませんでしたの設定に関する情報のコレクションを表します。
ms.openlocfilehash: 4477c30145d2cb187a4309d018512537af974ee8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839960"
---
# <a name="usersettingerrors-soap"></a><span data-ttu-id="ed6ad-103">UserSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ed6ad-103">UserSettingErrors (SOAP)</span></span>

<span data-ttu-id="ed6ad-104">**UserSettingErrors**要素は、返されませんでしたの設定に関する情報のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="ed6ad-104">The **UserSettingErrors** element represents a collection of information about settings that could not be returned.</span></span> 
  
```XML
<UserSettingErrors>
    <UserSettingError/>
</UserSettingErrors>
```

 <span data-ttu-id="ed6ad-105">**UserSettingErrors**</span><span class="sxs-lookup"><span data-stu-id="ed6ad-105">**UserSettingErrors**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ed6ad-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ed6ad-106">Attributes and elements</span></span>

<span data-ttu-id="ed6ad-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ed6ad-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ed6ad-108">属性</span><span class="sxs-lookup"><span data-stu-id="ed6ad-108">Attributes</span></span>

<span data-ttu-id="ed6ad-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ed6ad-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ed6ad-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ed6ad-110">Child elements</span></span>

|<span data-ttu-id="ed6ad-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="ed6ad-111">**Element**</span></span>|<span data-ttu-id="ed6ad-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="ed6ad-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ed6ad-113">UserSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ed6ad-113">UserSettingError (SOAP)</span></span>](usersettingerror-soap.md) <br/> |<span data-ttu-id="ed6ad-114">ユーザー設定の取得中に返されるエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="ed6ad-114">Represents an error that is returned while retrieving a user setting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ed6ad-115">親要素</span><span class="sxs-lookup"><span data-stu-id="ed6ad-115">Parent elements</span></span>

|<span data-ttu-id="ed6ad-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="ed6ad-116">**Element**</span></span>|<span data-ttu-id="ed6ad-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="ed6ad-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ed6ad-118">UserResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ed6ad-118">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="ed6ad-119">個々 のユーザーの GetUserSettings の要求に対する応答を表します。</span><span class="sxs-lookup"><span data-stu-id="ed6ad-119">Represents a response to a GetUserSettings request for an individual user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ed6ad-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ed6ad-120">Text value</span></span>

<span data-ttu-id="ed6ad-121">なし。</span><span class="sxs-lookup"><span data-stu-id="ed6ad-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ed6ad-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="ed6ad-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ed6ad-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="ed6ad-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="ed6ad-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ed6ad-124">Schema Name</span></span>  <br/> |<span data-ttu-id="ed6ad-125">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="ed6ad-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="ed6ad-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ed6ad-126">Validation File</span></span>  <br/> |<span data-ttu-id="ed6ad-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ed6ad-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ed6ad-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ed6ad-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="ed6ad-129">True</span><span class="sxs-lookup"><span data-stu-id="ed6ad-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ed6ad-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="ed6ad-130">See also</span></span>



[<span data-ttu-id="ed6ad-131">Exchange 2013 の自動検出の XML 要素を SOAP</span><span class="sxs-lookup"><span data-stu-id="ed6ad-131">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

