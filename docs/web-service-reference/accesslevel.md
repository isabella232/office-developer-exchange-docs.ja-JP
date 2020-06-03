---
title: AccessLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 09475586-00fa-4e82-a915-5ca263ab4d1c
description: AccessLevel 要素は、オンライン会議のアクセスレベルを指定します。
ms.openlocfilehash: 3c1375ef37ea666c6c4fafce7daa46ae0d0a2696
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462340"
---
# <a name="accesslevel"></a><span data-ttu-id="25650-103">AccessLevel</span><span class="sxs-lookup"><span data-stu-id="25650-103">AccessLevel</span></span>

<span data-ttu-id="25650-104">**Accesslevel**要素は、オンライン会議のアクセスレベルを指定します。</span><span class="sxs-lookup"><span data-stu-id="25650-104">The **AccessLevel** element specifies the access level for an online meeting.</span></span> 
  
```XML
<AccessLevel/>
```

 <span data-ttu-id="25650-105">**OnlineMeetingSettingsType**</span><span class="sxs-lookup"><span data-stu-id="25650-105">**OnlineMeetingSettingsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="25650-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="25650-106">Attributes and elements</span></span>

<span data-ttu-id="25650-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="25650-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="25650-108">属性</span><span class="sxs-lookup"><span data-stu-id="25650-108">Attributes</span></span>

<span data-ttu-id="25650-109">なし。</span><span class="sxs-lookup"><span data-stu-id="25650-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="25650-110">子要素</span><span class="sxs-lookup"><span data-stu-id="25650-110">Child elements</span></span>

<span data-ttu-id="25650-111">なし。</span><span class="sxs-lookup"><span data-stu-id="25650-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="25650-112">親要素</span><span class="sxs-lookup"><span data-stu-id="25650-112">Parent elements</span></span>

|<span data-ttu-id="25650-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="25650-113">**Element**</span></span>|<span data-ttu-id="25650-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="25650-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="25650-115">OnlineMeetingSettings</span><span class="sxs-lookup"><span data-stu-id="25650-115">OnlineMeetingSettings</span></span>](onlinemeetingsettings.md) <br/> |<span data-ttu-id="25650-116">オンライン会議の設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="25650-116">Specifies the settings for online meetings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="25650-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="25650-117">Text value</span></span>

<span data-ttu-id="25650-118">次の表に、 **Accesslevel**要素のテキスト値を示します。</span><span class="sxs-lookup"><span data-stu-id="25650-118">The following table lists the text values for the **AccessLevel** element.</span></span> 
  
<span data-ttu-id="25650-119">**AccessLevel 要素のテキスト値**</span><span class="sxs-lookup"><span data-stu-id="25650-119">**AccessLevel element text values**</span></span>

|<span data-ttu-id="25650-120">**値**</span><span class="sxs-lookup"><span data-stu-id="25650-120">**Value**</span></span>|<span data-ttu-id="25650-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="25650-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="25650-122">すべてのユーザー</span><span class="sxs-lookup"><span data-stu-id="25650-122">Everyone</span></span>  <br/> |<span data-ttu-id="25650-123">アクセスレベルが [すべて] になっています。</span><span class="sxs-lookup"><span data-stu-id="25650-123">The access level is open to all.</span></span>  <br/> |
|<span data-ttu-id="25650-124">内部</span><span class="sxs-lookup"><span data-stu-id="25650-124">Internal</span></span>  <br/> |<span data-ttu-id="25650-125">アクセスレベルは内部のみです。</span><span class="sxs-lookup"><span data-stu-id="25650-125">The access level is internal only.</span></span>  <br/> |
|<span data-ttu-id="25650-126">あなた</span><span class="sxs-lookup"><span data-stu-id="25650-126">Invited</span></span>  <br/> |<span data-ttu-id="25650-127">アクセスレベルは、招待された参加者のみになります。</span><span class="sxs-lookup"><span data-stu-id="25650-127">The access level is invited participants only.</span></span>  <br/> |
|<span data-ttu-id="25650-128">ロックされています</span><span class="sxs-lookup"><span data-stu-id="25650-128">Locked</span></span>  <br/> |<span data-ttu-id="25650-129">アクセスレベルがロックされています。</span><span class="sxs-lookup"><span data-stu-id="25650-129">The access level is locked.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="25650-130">注釈</span><span class="sxs-lookup"><span data-stu-id="25650-130">Remarks</span></span>

<span data-ttu-id="25650-131">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="25650-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="25650-132">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="25650-132">This element was introduced in Exchange Server 2013.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="25650-133">要素の情報</span><span class="sxs-lookup"><span data-stu-id="25650-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="25650-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="25650-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="25650-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="25650-135">Schema name</span></span>  <br/> |<span data-ttu-id="25650-136">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="25650-136">Type schema</span></span>  <br/> |
|<span data-ttu-id="25650-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="25650-137">Validation file</span></span>  <br/> |<span data-ttu-id="25650-138">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="25650-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="25650-139">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="25650-139">Can be empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="25650-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="25650-140">See also</span></span>

- [<span data-ttu-id="25650-141">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="25650-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

