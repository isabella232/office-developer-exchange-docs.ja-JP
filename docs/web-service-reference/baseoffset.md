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
description: BaseOffset 要素は、時間単位の現在のタイム ゾーンの世界協定時刻 (UTC) からのオフセットを表します。
ms.openlocfilehash: 56fc136537b7d5370074a0e6d492f214da3fd960
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759493"
---
# <a name="baseoffset"></a><span data-ttu-id="5a3a4-103">BaseOffset</span><span class="sxs-lookup"><span data-stu-id="5a3a4-103">BaseOffset</span></span>

<span data-ttu-id="5a3a4-104">**BaseOffset**要素は、時間単位の現在のタイム ゾーンの世界協定時刻 (UTC) からのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="5a3a4-104">The **BaseOffset** element represents the hourly offset from Coordinated Universal Time (UTC) for the current time zone.</span></span> 
  
```xml
<BaseOffset/>
```

 <span data-ttu-id="5a3a4-105">**duration**</span><span class="sxs-lookup"><span data-stu-id="5a3a4-105">**duration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5a3a4-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5a3a4-106">Attributes and elements</span></span>

<span data-ttu-id="5a3a4-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5a3a4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5a3a4-108">属性</span><span class="sxs-lookup"><span data-stu-id="5a3a4-108">Attributes</span></span>

<span data-ttu-id="5a3a4-109">なし</span><span class="sxs-lookup"><span data-stu-id="5a3a4-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5a3a4-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5a3a4-110">Child elements</span></span>

<span data-ttu-id="5a3a4-111">なし。</span><span class="sxs-lookup"><span data-stu-id="5a3a4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5a3a4-112">親要素</span><span class="sxs-lookup"><span data-stu-id="5a3a4-112">Parent elements</span></span>

|<span data-ttu-id="5a3a4-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="5a3a4-113">**Element**</span></span>|<span data-ttu-id="5a3a4-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="5a3a4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5a3a4-115">MeetingTimeZone</span><span class="sxs-lookup"><span data-stu-id="5a3a4-115">MeetingTimeZone</span></span>](meetingtimezone.md) <br/> |<span data-ttu-id="5a3a4-116">会議がホストされている場所のタイム ゾーンを表します。</span><span class="sxs-lookup"><span data-stu-id="5a3a4-116">Represents the time zone of the location where the meeting is hosted.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5a3a4-117">備考</span><span class="sxs-lookup"><span data-stu-id="5a3a4-117">Remarks</span></span>

<span data-ttu-id="5a3a4-118">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="5a3a4-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5a3a4-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="5a3a4-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5a3a4-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="5a3a4-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5a3a4-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5a3a4-121">Schema Name</span></span>  <br/> |<span data-ttu-id="5a3a4-122">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="5a3a4-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="5a3a4-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5a3a4-123">Validation File</span></span>  <br/> |<span data-ttu-id="5a3a4-124">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5a3a4-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5a3a4-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5a3a4-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="5a3a4-126">False</span><span class="sxs-lookup"><span data-stu-id="5a3a4-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5a3a4-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="5a3a4-127">See also</span></span>



- [<span data-ttu-id="5a3a4-128">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="5a3a4-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

