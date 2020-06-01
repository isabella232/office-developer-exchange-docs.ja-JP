---
title: NetShowUrl
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NetShowUrl
api_type:
- schema
ms.assetid: a5d48fc1-b141-422c-bcb0-05d0f9ba90dd
description: NetShowUrl 要素は、Microsoft NetShow online 会議の URL を指定します。
ms.openlocfilehash: 66e288a5e66eecf404698135cc3257085b852034
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466333"
---
# <a name="netshowurl"></a><span data-ttu-id="d7f67-103">NetShowUrl</span><span class="sxs-lookup"><span data-stu-id="d7f67-103">NetShowUrl</span></span>

<span data-ttu-id="d7f67-104">**Netshowurl**要素は、Microsoft NetShow online 会議の URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="d7f67-104">The **NetShowUrl** element specifies the URL for a Microsoft NetShow online meeting.</span></span> 
  
```xml
<NetShowUrl/>
```

 <span data-ttu-id="d7f67-105">**string**</span><span class="sxs-lookup"><span data-stu-id="d7f67-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d7f67-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d7f67-106">Attributes and elements</span></span>

<span data-ttu-id="d7f67-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d7f67-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d7f67-108">属性</span><span class="sxs-lookup"><span data-stu-id="d7f67-108">Attributes</span></span>

<span data-ttu-id="d7f67-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d7f67-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d7f67-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d7f67-110">Child elements</span></span>

<span data-ttu-id="d7f67-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d7f67-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d7f67-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d7f67-112">Parent elements</span></span>

|<span data-ttu-id="d7f67-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="d7f67-113">**Element**</span></span>|<span data-ttu-id="d7f67-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="d7f67-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d7f67-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="d7f67-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="d7f67-116">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="d7f67-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d7f67-117">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="d7f67-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="d7f67-118">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="d7f67-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d7f67-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d7f67-119">Text value</span></span>

<span data-ttu-id="d7f67-120">この要素を使用する場合は、URL を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="d7f67-120">A text value that represents a URL is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d7f67-121">注釈</span><span class="sxs-lookup"><span data-stu-id="d7f67-121">Remarks</span></span>

<span data-ttu-id="d7f67-122">この NetShowUrl プロパティは、開催者の予定表アイテムに対して読み取り/書き込み可能です。</span><span class="sxs-lookup"><span data-stu-id="d7f67-122">This NetShowUrl property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="d7f67-123">会議出席依頼と出席者には読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d7f67-123">It is read-only for meeting requests and for attendees.</span></span>
  
<span data-ttu-id="d7f67-124">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="d7f67-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d7f67-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d7f67-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d7f67-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="d7f67-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d7f67-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d7f67-127">Schema name</span></span>  <br/> |<span data-ttu-id="d7f67-128">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d7f67-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="d7f67-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d7f67-129">Validation file</span></span>  <br/> |<span data-ttu-id="d7f67-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d7f67-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d7f67-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d7f67-131">Can be empty</span></span>  <br/> |<span data-ttu-id="d7f67-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="d7f67-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d7f67-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="d7f67-133">See also</span></span>



- [<span data-ttu-id="d7f67-134">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d7f67-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

