---
title: Id
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
description: Id 要素には、タイム ゾーン定義の識別子の配列が含まれています。
ms.openlocfilehash: e4f8afb1292b3cb9f3990d4613b7461050976a59
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831856"
---
# <a name="ids"></a><span data-ttu-id="74221-103">Id</span><span class="sxs-lookup"><span data-stu-id="74221-103">Ids</span></span>

<span data-ttu-id="74221-104">**Id**要素には、タイム ゾーン定義の識別子の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="74221-104">The **Ids** element contains an array of time zone definition identifiers.</span></span> 
  
```XML
<Ids>
   <Id/>
</Ids>
```

 <span data-ttu-id="74221-105">**NonEmptyArrayOfTimeZoneIdType**</span><span class="sxs-lookup"><span data-stu-id="74221-105">**NonEmptyArrayOfTimeZoneIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="74221-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="74221-106">Attributes and elements</span></span>

<span data-ttu-id="74221-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="74221-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="74221-108">属性</span><span class="sxs-lookup"><span data-stu-id="74221-108">Attributes</span></span>

<span data-ttu-id="74221-109">なし。</span><span class="sxs-lookup"><span data-stu-id="74221-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="74221-110">子要素</span><span class="sxs-lookup"><span data-stu-id="74221-110">Child elements</span></span>

|<span data-ttu-id="74221-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="74221-111">**Element**</span></span>|<span data-ttu-id="74221-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="74221-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="74221-113">Id (タイムゾーン)</span><span class="sxs-lookup"><span data-stu-id="74221-113">Id (TimeZone)</span></span>](id-timezone.md) <br/> |<span data-ttu-id="74221-114">単一のタイム ゾーン定義を識別する要素です。</span><span class="sxs-lookup"><span data-stu-id="74221-114">The element that identifies a single time zone definition.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="74221-115">親要素</span><span class="sxs-lookup"><span data-stu-id="74221-115">Parent elements</span></span>

|<span data-ttu-id="74221-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="74221-116">**Element**</span></span>|<span data-ttu-id="74221-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="74221-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="74221-118">GetServerTimeZones</span><span class="sxs-lookup"><span data-stu-id="74221-118">GetServerTimeZones</span></span>](getservertimezones.md) <br/> |<span data-ttu-id="74221-119">Exchange サーバーからのタイム ゾーン定義を取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="74221-119">Defines a request to retrieve time zone definitions from the Exchange server.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="74221-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="74221-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="74221-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="74221-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="74221-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="74221-122">Schema Name</span></span>  <br/> |<span data-ttu-id="74221-123">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="74221-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="74221-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="74221-124">Validation File</span></span>  <br/> |<span data-ttu-id="74221-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="74221-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="74221-126">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="74221-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="74221-127">False</span><span class="sxs-lookup"><span data-stu-id="74221-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="74221-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="74221-128">See also</span></span>



- [<span data-ttu-id="74221-129">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="74221-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

