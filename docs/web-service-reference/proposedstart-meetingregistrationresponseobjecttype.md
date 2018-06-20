---
title: ProposedStart (MeetingRegistrationResponseObjectType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8c58cef7-bc43-493a-a323-ba4dc6a33704
description: ProposedStart (MeetingRegistrationResponseObjectType) の要素では、出席者の提案された新しい開始会議の時間を指定します。
ms.openlocfilehash: db03d1b5e79ed53313cff9677687647f24e90756
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832905"
---
# <a name="proposedstart-meetingregistrationresponseobjecttype"></a><span data-ttu-id="19c01-103">ProposedStart (MeetingRegistrationResponseObjectType)</span><span class="sxs-lookup"><span data-stu-id="19c01-103">ProposedStart (MeetingRegistrationResponseObjectType)</span></span>

<span data-ttu-id="19c01-104">**ProposedStart (MeetingRegistrationResponseObjectType)** の要素では、出席者の提案された新しい開始会議の時間を指定します。</span><span class="sxs-lookup"><span data-stu-id="19c01-104">The **ProposedStart (MeetingRegistrationResponseObjectType)** element specifies an attendee's proposed new start time for a meeting.</span></span> 
  
```XML
<ProposedStart />
```

 <span data-ttu-id="19c01-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="19c01-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="19c01-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="19c01-106">Attributes and elements</span></span>

<span data-ttu-id="19c01-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="19c01-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="19c01-108">属性</span><span class="sxs-lookup"><span data-stu-id="19c01-108">Attributes</span></span>

<span data-ttu-id="19c01-109">なし。</span><span class="sxs-lookup"><span data-stu-id="19c01-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="19c01-110">子要素</span><span class="sxs-lookup"><span data-stu-id="19c01-110">Child elements</span></span>

<span data-ttu-id="19c01-111">なし。</span><span class="sxs-lookup"><span data-stu-id="19c01-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="19c01-112">親要素</span><span class="sxs-lookup"><span data-stu-id="19c01-112">Parent elements</span></span>

<span data-ttu-id="19c01-113">[AcceptItem](acceptitem.md) | [TentativelyAcceptItem](tentativelyacceptitem.md) | [DeclineItem](declineitem.md)</span><span class="sxs-lookup"><span data-stu-id="19c01-113">[AcceptItem](acceptitem.md) | [TentativelyAcceptItem](tentativelyacceptitem.md) | [DeclineItem](declineitem.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="19c01-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="19c01-114">Text value</span></span>

<span data-ttu-id="19c01-115">**ProposedStart (MeetingRegistrationResponseObjectType)** の要素のテキスト値とは、提案された開始日と会議の時刻です。</span><span class="sxs-lookup"><span data-stu-id="19c01-115">The text value of the **ProposedStart (MeetingRegistrationResponseObjectType)** element is the proposed start date and time of the meeting.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="19c01-116">備考</span><span class="sxs-lookup"><span data-stu-id="19c01-116">Remarks</span></span>

<span data-ttu-id="19c01-117">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="19c01-117">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="19c01-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="19c01-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="19c01-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="19c01-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="19c01-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="19c01-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="19c01-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="19c01-121">Schema Name</span></span>  <br/> |<span data-ttu-id="19c01-122">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="19c01-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="19c01-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="19c01-123">Validation File</span></span>  <br/> |<span data-ttu-id="19c01-124">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="19c01-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="19c01-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="19c01-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="19c01-126">True</span><span class="sxs-lookup"><span data-stu-id="19c01-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="19c01-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="19c01-127">See also</span></span>



[<span data-ttu-id="19c01-128">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="19c01-128">AcceptItem</span></span>](acceptitem.md)
  
[<span data-ttu-id="19c01-129">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="19c01-129">DeclineItem</span></span>](declineitem.md)
  
[<span data-ttu-id="19c01-130">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="19c01-130">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md)


- [<span data-ttu-id="19c01-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="19c01-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

