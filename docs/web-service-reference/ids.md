---
title: Rid
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Ids
api_type:
- schema
ms.assetid: c54cdeaf-6761-4d1a-a329-fb279f0e2a64
description: Ids 要素には、タイムゾーン定義識別子の配列が含まれています。
ms.openlocfilehash: 1c5a6974c8d3abc318ff122f3db09d8c3472dc65
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457621"
---
# <a name="ids"></a><span data-ttu-id="f23b6-103">Rid</span><span class="sxs-lookup"><span data-stu-id="f23b6-103">Ids</span></span>

<span data-ttu-id="f23b6-104">**Ids**要素には、タイムゾーン定義識別子の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f23b6-104">The **Ids** element contains an array of time zone definition identifiers.</span></span> 
  
```XML
<Ids>
   <Id/>
</Ids>
```

 <span data-ttu-id="f23b6-105">**NonEmptyArrayOfTimeZoneIdType**</span><span class="sxs-lookup"><span data-stu-id="f23b6-105">**NonEmptyArrayOfTimeZoneIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f23b6-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f23b6-106">Attributes and elements</span></span>

<span data-ttu-id="f23b6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f23b6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f23b6-108">属性</span><span class="sxs-lookup"><span data-stu-id="f23b6-108">Attributes</span></span>

<span data-ttu-id="f23b6-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f23b6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f23b6-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f23b6-110">Child elements</span></span>

|<span data-ttu-id="f23b6-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="f23b6-111">**Element**</span></span>|<span data-ttu-id="f23b6-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="f23b6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f23b6-113">Id (TimeZone)</span><span class="sxs-lookup"><span data-stu-id="f23b6-113">Id (TimeZone)</span></span>](id-timezone.md) <br/> |<span data-ttu-id="f23b6-114">1つのタイムゾーン定義を識別する要素。</span><span class="sxs-lookup"><span data-stu-id="f23b6-114">The element that identifies a single time zone definition.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f23b6-115">親要素</span><span class="sxs-lookup"><span data-stu-id="f23b6-115">Parent elements</span></span>

|<span data-ttu-id="f23b6-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="f23b6-116">**Element**</span></span>|<span data-ttu-id="f23b6-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="f23b6-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f23b6-118">GetServerTimeZones</span><span class="sxs-lookup"><span data-stu-id="f23b6-118">GetServerTimeZones</span></span>](getservertimezones.md) <br/> |<span data-ttu-id="f23b6-119">Exchange サーバーからタイムゾーン定義を取得するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="f23b6-119">Defines a request to retrieve time zone definitions from the Exchange server.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="f23b6-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f23b6-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f23b6-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="f23b6-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f23b6-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f23b6-122">Schema Name</span></span>  <br/> |<span data-ttu-id="f23b6-123">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="f23b6-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f23b6-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f23b6-124">Validation File</span></span>  <br/> |<span data-ttu-id="f23b6-125">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="f23b6-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f23b6-126">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f23b6-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="f23b6-127">正しくない</span><span class="sxs-lookup"><span data-stu-id="f23b6-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f23b6-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="f23b6-128">See also</span></span>



- [<span data-ttu-id="f23b6-129">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="f23b6-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

