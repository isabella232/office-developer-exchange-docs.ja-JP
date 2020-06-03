---
title: ProposedEnd (会議 Registrationresponseobjecttype)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3e5d2567-a5a2-4791-b209-c29082894a9e
description: ProposedEnd (meeting Registrationresponseobjecttype) 要素は、会議の出席者が提案した新しい終了時刻を指定します。
ms.openlocfilehash: f6aafe157c653776dca511a104ceeb9518812d98
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466984"
---
# <a name="proposedend-meetingregistrationresponseobjecttype"></a><span data-ttu-id="a6466-103">ProposedEnd (会議 Registrationresponseobjecttype)</span><span class="sxs-lookup"><span data-stu-id="a6466-103">ProposedEnd (MeetingRegistrationResponseObjectType)</span></span>

<span data-ttu-id="a6466-104">**ProposedEnd (Meeting Registrationresponseobjecttype)** 要素は、会議の出席者が提案した新しい終了時刻を指定します。</span><span class="sxs-lookup"><span data-stu-id="a6466-104">The **ProposedEnd (MeetingRegistrationResponseObjectType)** element specifies an attendee's proposed new end time for a meeting.</span></span> 
  
```XML
<ProposedEnd />
```

 <span data-ttu-id="a6466-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="a6466-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a6466-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a6466-106">Attributes and elements</span></span>

<span data-ttu-id="a6466-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a6466-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a6466-108">属性</span><span class="sxs-lookup"><span data-stu-id="a6466-108">Attributes</span></span>

<span data-ttu-id="a6466-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a6466-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a6466-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a6466-110">Child elements</span></span>

<span data-ttu-id="a6466-111">なし。</span><span class="sxs-lookup"><span data-stu-id="a6466-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a6466-112">親要素</span><span class="sxs-lookup"><span data-stu-id="a6466-112">Parent elements</span></span>

<span data-ttu-id="a6466-113">[Acceptitem](acceptitem.md)  | [TentativelyAcceptItem](tentativelyacceptitem.md)  | [Declineitem](declineitem.md)</span><span class="sxs-lookup"><span data-stu-id="a6466-113">[AcceptItem](acceptitem.md) | [TentativelyAcceptItem](tentativelyacceptitem.md) | [DeclineItem](declineitem.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="a6466-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a6466-114">Text value</span></span>

<span data-ttu-id="a6466-115">**ProposedEnd (Meeting Registrationresponseobjecttype)** 要素のテキスト値は、提案された会議の終了日時です。</span><span class="sxs-lookup"><span data-stu-id="a6466-115">The text value of the **ProposedEnd (MeetingRegistrationResponseObjectType)** element is the proposed end date and time of the meeting.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a6466-116">注釈</span><span class="sxs-lookup"><span data-stu-id="a6466-116">Remarks</span></span>

<span data-ttu-id="a6466-117">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="a6466-117">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="a6466-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a6466-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a6466-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a6466-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a6466-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="a6466-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a6466-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a6466-121">Schema Name</span></span>  <br/> |<span data-ttu-id="a6466-122">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="a6466-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="a6466-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a6466-123">Validation File</span></span>  <br/> |<span data-ttu-id="a6466-124">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="a6466-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a6466-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a6466-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="a6466-126">正しい</span><span class="sxs-lookup"><span data-stu-id="a6466-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a6466-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="a6466-127">See also</span></span>



[<span data-ttu-id="a6466-128">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="a6466-128">AcceptItem</span></span>](acceptitem.md)
  
[<span data-ttu-id="a6466-129">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="a6466-129">DeclineItem</span></span>](declineitem.md)
  
[<span data-ttu-id="a6466-130">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="a6466-130">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md)


- [<span data-ttu-id="a6466-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="a6466-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

