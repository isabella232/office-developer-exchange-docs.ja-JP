---
title: NormalizedBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bfb813e4-642d-4f1b-9e91-1fee89dbd083
description: NormalizedBody 要素は、別の HTML 本文に挿入できるフラグメントとしてアイテムの Body プロパティの HTML 表記を指定します。
ms.openlocfilehash: 07c2176d2c8a7473c06b7e42f8bcbbe6670581ef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832548"
---
# <a name="normalizedbody"></a><span data-ttu-id="c5559-103">NormalizedBody</span><span class="sxs-lookup"><span data-stu-id="c5559-103">NormalizedBody</span></span>

<span data-ttu-id="c5559-104">**NormalizedBody**要素は、別の HTML 本文に挿入できるフラグメントとしてアイテムの**Body**プロパティの HTML 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c5559-104">The **NormalizedBody** element specifies an HTML representation of the **Body** property of an item as a fragment that can be inserted into another HTML body.</span></span> 
  
```XML
<NormalizedBody BodyType="Text | HTML" IsTruncated="true | false"></NormalizedBody>
```

 <span data-ttu-id="c5559-105">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="c5559-105">**BodyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c5559-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="c5559-106">Attributes and elements</span></span>

<span data-ttu-id="c5559-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c5559-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c5559-108">属性</span><span class="sxs-lookup"><span data-stu-id="c5559-108">Attributes</span></span>

|<span data-ttu-id="c5559-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="c5559-109">**Attribute**</span></span>|<span data-ttu-id="c5559-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="c5559-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c5559-111">BodyType</span><span class="sxs-lookup"><span data-stu-id="c5559-111">BodyType</span></span>  <br/> |<span data-ttu-id="c5559-112">本文の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="c5559-112">Indicates the body type.</span></span> <span data-ttu-id="c5559-113">**BodyType**属性の**テキスト**の値は、プレーン テキスト形式の本文であることを示します。</span><span class="sxs-lookup"><span data-stu-id="c5559-113">The value of **Text** for the **BodyType** attribute indicates that the body is in plain text form.</span></span> <span data-ttu-id="c5559-114">**BodyType**属性の**HTML**の値は、本文が HTML 形式でことを示します。</span><span class="sxs-lookup"><span data-stu-id="c5559-114">The value of **HTML** for the **BodyType** attribute indicates that the body is in HTML form.</span></span> <span data-ttu-id="c5559-115">**BodyType**属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="c5559-115">The **BodyType** attribute is required.</span></span>  <br/> |
|<span data-ttu-id="c5559-116">IsTruncated</span><span class="sxs-lookup"><span data-stu-id="c5559-116">IsTruncated</span></span>  <br/> |<span data-ttu-id="c5559-117">本文の内容が切り詰められたことを示します。</span><span class="sxs-lookup"><span data-stu-id="c5559-117">Indicates that the body contents have been truncated.</span></span> <span data-ttu-id="c5559-118">テキスト値が**false**の**IsTruncated**属性のでは、本文の内容は切り捨てられましたしないことを示します。</span><span class="sxs-lookup"><span data-stu-id="c5559-118">A text value of **false** for the **IsTruncated** attribute indicates that the body contents have not been truncated.</span></span> <span data-ttu-id="c5559-119">正規化された本文は[MaximumBodySize](maximumbodysize.md)要素で設定した値よりも長い場合は、正規化された本文の長さに切り詰められます。</span><span class="sxs-lookup"><span data-stu-id="c5559-119">The normalized body will be truncated if the normalized body length is longer than the value set in the [MaximumBodySize](maximumbodysize.md) element.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c5559-120">子要素</span><span class="sxs-lookup"><span data-stu-id="c5559-120">Child elements</span></span>

<span data-ttu-id="c5559-121">なし。</span><span class="sxs-lookup"><span data-stu-id="c5559-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c5559-122">親要素</span><span class="sxs-lookup"><span data-stu-id="c5559-122">Parent elements</span></span>

<span data-ttu-id="c5559-123">[項目](item.md) | [メッセージ](message-ex15websvcsotherref.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [MeetingCancellation](meetingcancellation.md) | [作業](task.md) | [PostItem](postitem.md)  | [カレンダー項目](calendaritem.md) | [連絡先](contact.md) | [DistributionList](distributionlist.md)</span><span class="sxs-lookup"><span data-stu-id="c5559-123">[Item](item.md) | [Message](message-ex15websvcsotherref.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [MeetingCancellation](meetingcancellation.md) | [Task](task.md) | [PostItem](postitem.md) | [CalendarItem](calendaritem.md) | [Contact](contact.md) | [DistributionList](distributionlist.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="c5559-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c5559-124">Text value</span></span>

<span data-ttu-id="c5559-125">**NormalizedBody**要素のテキスト値は、項目の正規化の本体です。</span><span class="sxs-lookup"><span data-stu-id="c5559-125">The text value of the **NormalizedBody** element is the normalized body of the item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c5559-126">備考</span><span class="sxs-lookup"><span data-stu-id="c5559-126">Remarks</span></span>

<span data-ttu-id="c5559-127">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="c5559-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c5559-128">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="c5559-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c5559-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="c5559-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c5559-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="c5559-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c5559-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c5559-131">Schema name</span></span>  <br/> |<span data-ttu-id="c5559-132">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="c5559-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="c5559-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c5559-133">Validation file</span></span>  <br/> |<span data-ttu-id="c5559-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c5559-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c5559-135">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c5559-135">Can be empty</span></span>  <br/> ||
   

