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
description: StringSetting 要素は、string 型の値を設定するユーザーを表します。
ms.openlocfilehash: 215d1187c0968577e894c9f9cddea050789697b9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463077"
---
# <a name="stringsetting-soap"></a><span data-ttu-id="58c86-103">StringSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="58c86-103">StringSetting (SOAP)</span></span>

<span data-ttu-id="58c86-104">**Stringsetting**要素は、string 型の値を設定するユーザーを表します。</span><span class="sxs-lookup"><span data-stu-id="58c86-104">The **StringSetting** element represents a user setting the value of which is of type string.</span></span> 
  
```XML
<StringSetting>
   <Name/>
   <Value/>
</StringSetting>
```

 <span data-ttu-id="58c86-105">**StringSetting**</span><span class="sxs-lookup"><span data-stu-id="58c86-105">**StringSetting**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="58c86-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="58c86-106">Attributes and elements</span></span>

<span data-ttu-id="58c86-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="58c86-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="58c86-108">属性</span><span class="sxs-lookup"><span data-stu-id="58c86-108">Attributes</span></span>

<span data-ttu-id="58c86-109">なし。</span><span class="sxs-lookup"><span data-stu-id="58c86-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="58c86-110">子要素</span><span class="sxs-lookup"><span data-stu-id="58c86-110">Child elements</span></span>

|<span data-ttu-id="58c86-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="58c86-111">**Element**</span></span>|<span data-ttu-id="58c86-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="58c86-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="58c86-113">Name (SOAP)</span><span class="sxs-lookup"><span data-stu-id="58c86-113">Name (SOAP)</span></span>](name-soap.md) <br/> |<span data-ttu-id="58c86-114">ユーザー設定の名前を表します。</span><span class="sxs-lookup"><span data-stu-id="58c86-114">Represents a user setting name.</span></span>  <br/> |
|[<span data-ttu-id="58c86-115">Value (SOAP)</span><span class="sxs-lookup"><span data-stu-id="58c86-115">Value (SOAP)</span></span>](value-soap.md) <br/> |<span data-ttu-id="58c86-116">ユーザー設定の値を表します。</span><span class="sxs-lookup"><span data-stu-id="58c86-116">Represents a user setting value.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="58c86-117">親要素</span><span class="sxs-lookup"><span data-stu-id="58c86-117">Parent elements</span></span>

<span data-ttu-id="58c86-118">なし。</span><span class="sxs-lookup"><span data-stu-id="58c86-118">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="58c86-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="58c86-119">Text value</span></span>

<span data-ttu-id="58c86-120">なし。</span><span class="sxs-lookup"><span data-stu-id="58c86-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="58c86-121">注釈</span><span class="sxs-lookup"><span data-stu-id="58c86-121">Remarks</span></span>

<span data-ttu-id="58c86-122">**Stringsetting**型は、 **usersetting**型を拡張します。</span><span class="sxs-lookup"><span data-stu-id="58c86-122">The **StringSetting** type extends the **UserSetting** type.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="58c86-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="58c86-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="58c86-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="58c86-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="58c86-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="58c86-125">Schema Name</span></span>  <br/> |<span data-ttu-id="58c86-126">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="58c86-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="58c86-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="58c86-127">Validation File</span></span>  <br/> |<span data-ttu-id="58c86-128">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="58c86-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="58c86-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="58c86-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="58c86-130">正しい</span><span class="sxs-lookup"><span data-stu-id="58c86-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="58c86-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="58c86-131">See also</span></span>



[<span data-ttu-id="58c86-132">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="58c86-132">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="58c86-133">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="58c86-133">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="58c86-134">GetFederationInformation 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="58c86-134">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

