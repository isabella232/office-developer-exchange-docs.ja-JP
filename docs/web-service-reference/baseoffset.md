---
title: BaseOffset
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BaseOffset
api_type:
- schema
ms.assetid: 0ffad7a6-8e1b-452b-9d87-8e0f6c77f0a6
description: BaseOffset 要素は、現在のタイムゾーンの協定世界時 (UTC) からの時間単位のオフセットを表します。
ms.openlocfilehash: 1e29f123dfac2e29807e0a2077d47adb14844f4e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460261"
---
# <a name="baseoffset"></a><span data-ttu-id="7b7a7-103">BaseOffset</span><span class="sxs-lookup"><span data-stu-id="7b7a7-103">BaseOffset</span></span>

<span data-ttu-id="7b7a7-104">**Baseoffset**要素は、現在のタイムゾーンの協定世界時 (UTC) からの時間単位のオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="7b7a7-104">The **BaseOffset** element represents the hourly offset from Coordinated Universal Time (UTC) for the current time zone.</span></span> 
  
```xml
<BaseOffset/>
```

 <span data-ttu-id="7b7a7-105">**duration**</span><span class="sxs-lookup"><span data-stu-id="7b7a7-105">**duration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7b7a7-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7b7a7-106">Attributes and elements</span></span>

<span data-ttu-id="7b7a7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7b7a7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7b7a7-108">属性</span><span class="sxs-lookup"><span data-stu-id="7b7a7-108">Attributes</span></span>

<span data-ttu-id="7b7a7-109">なし</span><span class="sxs-lookup"><span data-stu-id="7b7a7-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7b7a7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7b7a7-110">Child elements</span></span>

<span data-ttu-id="7b7a7-111">なし。</span><span class="sxs-lookup"><span data-stu-id="7b7a7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7b7a7-112">親要素</span><span class="sxs-lookup"><span data-stu-id="7b7a7-112">Parent elements</span></span>

|<span data-ttu-id="7b7a7-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="7b7a7-113">**Element**</span></span>|<span data-ttu-id="7b7a7-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="7b7a7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7b7a7-115">MeetingTimeZone</span><span class="sxs-lookup"><span data-stu-id="7b7a7-115">MeetingTimeZone</span></span>](meetingtimezone.md) <br/> |<span data-ttu-id="7b7a7-116">会議がホストされている場所のタイムゾーンを表します。</span><span class="sxs-lookup"><span data-stu-id="7b7a7-116">Represents the time zone of the location where the meeting is hosted.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7b7a7-117">注釈</span><span class="sxs-lookup"><span data-stu-id="7b7a7-117">Remarks</span></span>

<span data-ttu-id="7b7a7-118">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="7b7a7-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7b7a7-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7b7a7-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7b7a7-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="7b7a7-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7b7a7-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7b7a7-121">Schema Name</span></span>  <br/> |<span data-ttu-id="7b7a7-122">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="7b7a7-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="7b7a7-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7b7a7-123">Validation File</span></span>  <br/> |<span data-ttu-id="7b7a7-124">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="7b7a7-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7b7a7-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7b7a7-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="7b7a7-126">正しくない</span><span class="sxs-lookup"><span data-stu-id="7b7a7-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7b7a7-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="7b7a7-127">See also</span></span>



- [<span data-ttu-id="7b7a7-128">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="7b7a7-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

