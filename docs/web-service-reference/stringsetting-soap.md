---
title: StringSetting (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: bf7096d8-42d4-4bf5-bbdd-851af2754000
description: StringSetting 要素は、文字列型の値は、ユーザー設定を表します。
ms.openlocfilehash: af2c8ed243182e3491723be172ae162554250951
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833606"
---
# <a name="stringsetting-soap"></a><span data-ttu-id="05cd3-103">StringSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="05cd3-103">StringSetting (SOAP)</span></span>

<span data-ttu-id="05cd3-104">**StringSetting**要素は、文字列型の値は、ユーザー設定を表します。</span><span class="sxs-lookup"><span data-stu-id="05cd3-104">The **StringSetting** element represents a user setting the value of which is of type string.</span></span> 
  
```XML
<StringSetting>
   <Name/>
   <Value/>
</StringSetting>
```

 <span data-ttu-id="05cd3-105">**StringSetting**</span><span class="sxs-lookup"><span data-stu-id="05cd3-105">**StringSetting**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="05cd3-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="05cd3-106">Attributes and elements</span></span>

<span data-ttu-id="05cd3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="05cd3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="05cd3-108">属性</span><span class="sxs-lookup"><span data-stu-id="05cd3-108">Attributes</span></span>

<span data-ttu-id="05cd3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="05cd3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="05cd3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="05cd3-110">Child elements</span></span>

|<span data-ttu-id="05cd3-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="05cd3-111">**Element**</span></span>|<span data-ttu-id="05cd3-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="05cd3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="05cd3-113">名 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="05cd3-113">Name (SOAP)</span></span>](name-soap.md) <br/> |<span data-ttu-id="05cd3-114">ユーザー設定の名前を表します。</span><span class="sxs-lookup"><span data-stu-id="05cd3-114">Represents a user setting name.</span></span>  <br/> |
|[<span data-ttu-id="05cd3-115">値 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="05cd3-115">Value (SOAP)</span></span>](value-soap.md) <br/> |<span data-ttu-id="05cd3-116">ユーザー設定値を表します。</span><span class="sxs-lookup"><span data-stu-id="05cd3-116">Represents a user setting value.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="05cd3-117">親要素</span><span class="sxs-lookup"><span data-stu-id="05cd3-117">Parent elements</span></span>

<span data-ttu-id="05cd3-118">なし。</span><span class="sxs-lookup"><span data-stu-id="05cd3-118">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="05cd3-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="05cd3-119">Text value</span></span>

<span data-ttu-id="05cd3-120">なし。</span><span class="sxs-lookup"><span data-stu-id="05cd3-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="05cd3-121">備考</span><span class="sxs-lookup"><span data-stu-id="05cd3-121">Remarks</span></span>

<span data-ttu-id="05cd3-122">**StringSetting**型は、 **UserSetting**型を拡張します。</span><span class="sxs-lookup"><span data-stu-id="05cd3-122">The **StringSetting** type extends the **UserSetting** type.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="05cd3-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="05cd3-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="05cd3-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="05cd3-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="05cd3-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="05cd3-125">Schema Name</span></span>  <br/> |<span data-ttu-id="05cd3-126">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="05cd3-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="05cd3-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="05cd3-127">Validation File</span></span>  <br/> |<span data-ttu-id="05cd3-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="05cd3-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="05cd3-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="05cd3-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="05cd3-130">True</span><span class="sxs-lookup"><span data-stu-id="05cd3-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="05cd3-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="05cd3-131">See also</span></span>



[<span data-ttu-id="05cd3-132">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="05cd3-132">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="05cd3-133">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="05cd3-133">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="05cd3-134">GetFederationInformation 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="05cd3-134">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

