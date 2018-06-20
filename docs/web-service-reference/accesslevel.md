---
title: AccessLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 09475586-00fa-4e82-a915-5ca263ab4d1c
description: AccessLevel 要素は、オンライン会議のアクセス レベルを指定します。
ms.openlocfilehash: 1bf0a191fad529b555117e4ff992c352615bc79b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760420"
---
# <a name="accesslevel"></a><span data-ttu-id="bea0c-103">AccessLevel</span><span class="sxs-lookup"><span data-stu-id="bea0c-103">AccessLevel</span></span>

<span data-ttu-id="bea0c-104">**AccessLevel**要素は、オンライン会議のアクセス レベルを指定します。</span><span class="sxs-lookup"><span data-stu-id="bea0c-104">The **AccessLevel** element specifies the access level for an online meeting.</span></span> 
  
```XML
<AccessLevel/>
```

 <span data-ttu-id="bea0c-105">**OnlineMeetingSettingsType**</span><span class="sxs-lookup"><span data-stu-id="bea0c-105">**OnlineMeetingSettingsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bea0c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="bea0c-106">Attributes and elements</span></span>

<span data-ttu-id="bea0c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="bea0c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bea0c-108">属性</span><span class="sxs-lookup"><span data-stu-id="bea0c-108">Attributes</span></span>

<span data-ttu-id="bea0c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="bea0c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bea0c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="bea0c-110">Child elements</span></span>

<span data-ttu-id="bea0c-111">なし。</span><span class="sxs-lookup"><span data-stu-id="bea0c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bea0c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="bea0c-112">Parent elements</span></span>

|<span data-ttu-id="bea0c-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="bea0c-113">**Element**</span></span>|<span data-ttu-id="bea0c-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="bea0c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bea0c-115">OnlineMeetingSettings</span><span class="sxs-lookup"><span data-stu-id="bea0c-115">OnlineMeetingSettings</span></span>](onlinemeetingsettings.md) <br/> |<span data-ttu-id="bea0c-116">オンライン会議の設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="bea0c-116">Specifies the settings for online meetings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bea0c-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="bea0c-117">Text value</span></span>

<span data-ttu-id="bea0c-118">**AccessLevel**要素のテキスト値を次の表に一覧します。</span><span class="sxs-lookup"><span data-stu-id="bea0c-118">The following table lists the text values for the **AccessLevel** element.</span></span> 
  
<span data-ttu-id="bea0c-119">**AccessLevel 要素のテキスト値**</span><span class="sxs-lookup"><span data-stu-id="bea0c-119">**AccessLevel element text values**</span></span>

|<span data-ttu-id="bea0c-120">**値**</span><span class="sxs-lookup"><span data-stu-id="bea0c-120">**Value**</span></span>|<span data-ttu-id="bea0c-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="bea0c-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bea0c-122">全員</span><span class="sxs-lookup"><span data-stu-id="bea0c-122">Everyone</span></span>  <br/> |<span data-ttu-id="bea0c-123">アクセス レベルは、すべてに開かれています。</span><span class="sxs-lookup"><span data-stu-id="bea0c-123">The access level is open to all.</span></span>  <br/> |
|<span data-ttu-id="bea0c-124">内部</span><span class="sxs-lookup"><span data-stu-id="bea0c-124">Internal</span></span>  <br/> |<span data-ttu-id="bea0c-125">アクセス レベルは、内部のみです。</span><span class="sxs-lookup"><span data-stu-id="bea0c-125">The access level is internal only.</span></span>  <br/> |
|<span data-ttu-id="bea0c-126">招待</span><span class="sxs-lookup"><span data-stu-id="bea0c-126">Invited</span></span>  <br/> |<span data-ttu-id="bea0c-127">アクセス レベルとは、招待された参加者のみです。</span><span class="sxs-lookup"><span data-stu-id="bea0c-127">The access level is invited participants only.</span></span>  <br/> |
|<span data-ttu-id="bea0c-128">ロック</span><span class="sxs-lookup"><span data-stu-id="bea0c-128">Locked</span></span>  <br/> |<span data-ttu-id="bea0c-129">アクセス レベルはロックされています。</span><span class="sxs-lookup"><span data-stu-id="bea0c-129">The access level is locked.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bea0c-130">備考</span><span class="sxs-lookup"><span data-stu-id="bea0c-130">Remarks</span></span>

<span data-ttu-id="bea0c-131">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="bea0c-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="bea0c-132">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="bea0c-132">This element was introduced in Exchange Server 2013.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bea0c-133">要素情報</span><span class="sxs-lookup"><span data-stu-id="bea0c-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bea0c-134">名前空間</span><span class="sxs-lookup"><span data-stu-id="bea0c-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bea0c-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="bea0c-135">Schema name</span></span>  <br/> |<span data-ttu-id="bea0c-136">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="bea0c-136">Type schema</span></span>  <br/> |
|<span data-ttu-id="bea0c-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="bea0c-137">Validation file</span></span>  <br/> |<span data-ttu-id="bea0c-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bea0c-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bea0c-139">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="bea0c-139">Can be empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="bea0c-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="bea0c-140">See also</span></span>

- [<span data-ttu-id="bea0c-141">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="bea0c-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

