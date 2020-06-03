---
title: NormalizedBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bfb813e4-642d-4f1b-9e91-1fee89dbd083
description: NormalizedBody 要素は、別の HTML 本文に挿入できるフラグメントとして、アイテムの Body プロパティの HTML 表記を指定します。
ms.openlocfilehash: fb249794bccfeed198e7a3230ab53c66893dcf96
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462669"
---
# <a name="normalizedbody"></a><span data-ttu-id="01e2f-103">NormalizedBody</span><span class="sxs-lookup"><span data-stu-id="01e2f-103">NormalizedBody</span></span>

<span data-ttu-id="01e2f-104">**Normalizedbody**要素は、別の html 本文に挿入できるフラグメントとして、アイテムの**BODY**プロパティの HTML 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="01e2f-104">The **NormalizedBody** element specifies an HTML representation of the **Body** property of an item as a fragment that can be inserted into another HTML body.</span></span> 
  
```XML
<NormalizedBody BodyType="Text | HTML" IsTruncated="true | false"></NormalizedBody>
```

 <span data-ttu-id="01e2f-105">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="01e2f-105">**BodyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="01e2f-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="01e2f-106">Attributes and elements</span></span>

<span data-ttu-id="01e2f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="01e2f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="01e2f-108">属性</span><span class="sxs-lookup"><span data-stu-id="01e2f-108">Attributes</span></span>

|<span data-ttu-id="01e2f-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="01e2f-109">**Attribute**</span></span>|<span data-ttu-id="01e2f-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="01e2f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="01e2f-111">BodyType</span><span class="sxs-lookup"><span data-stu-id="01e2f-111">BodyType</span></span>  <br/> |<span data-ttu-id="01e2f-112">本文の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="01e2f-112">Indicates the body type.</span></span> <span data-ttu-id="01e2f-113">**Bodytype**属性の**テキスト**の値は、本文がプレーンテキスト形式であることを示します。</span><span class="sxs-lookup"><span data-stu-id="01e2f-113">The value of **Text** for the **BodyType** attribute indicates that the body is in plain text form.</span></span> <span data-ttu-id="01e2f-114">**Bodytype**属性の**html**の値は、本文が HTML 形式であることを示します。</span><span class="sxs-lookup"><span data-stu-id="01e2f-114">The value of **HTML** for the **BodyType** attribute indicates that the body is in HTML form.</span></span> <span data-ttu-id="01e2f-115">**Bodytype**属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="01e2f-115">The **BodyType** attribute is required.</span></span>  <br/> |
|<span data-ttu-id="01e2f-116">Istrがありません</span><span class="sxs-lookup"><span data-stu-id="01e2f-116">IsTruncated</span></span>  <br/> |<span data-ttu-id="01e2f-117">本文の内容が切り捨てられていることを示します。</span><span class="sxs-lookup"><span data-stu-id="01e2f-117">Indicates that the body contents have been truncated.</span></span> <span data-ttu-id="01e2f-118">**Istruncated** attribute のテキスト値が**false**の場合は、本文のコンテンツが切り捨てられていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="01e2f-118">A text value of **false** for the **IsTruncated** attribute indicates that the body contents have not been truncated.</span></span> <span data-ttu-id="01e2f-119">正規化された本文の長さが、 [Maximumbodysize](maximumbodysize.md)要素で設定された値よりも長い場合は、正規化された本文は切り捨てられます。</span><span class="sxs-lookup"><span data-stu-id="01e2f-119">The normalized body will be truncated if the normalized body length is longer than the value set in the [MaximumBodySize](maximumbodysize.md) element.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="01e2f-120">子要素</span><span class="sxs-lookup"><span data-stu-id="01e2f-120">Child elements</span></span>

<span data-ttu-id="01e2f-121">なし。</span><span class="sxs-lookup"><span data-stu-id="01e2f-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="01e2f-122">親要素</span><span class="sxs-lookup"><span data-stu-id="01e2f-122">Parent elements</span></span>

<span data-ttu-id="01e2f-123">[アイテム](item.md)  | [メッセージ](message-ex15websvcsotherref.md)  | [会議メッセージ](meetingmessage.md)  | [会議の要求](meetingrequest.md)  | [会議の応答](meetingresponse.md)  | [会議のキャンセル](meetingcancellation.md)  | [タスク](task.md)  | [Postitem](postitem.md)  | [Calendaritem](calendaritem.md)  | [連絡先](contact.md)  | [DistributionList](distributionlist.md)</span><span class="sxs-lookup"><span data-stu-id="01e2f-123">[Item](item.md) | [Message](message-ex15websvcsotherref.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [MeetingCancellation](meetingcancellation.md) | [Task](task.md) | [PostItem](postitem.md) | [CalendarItem](calendaritem.md) | [Contact](contact.md) | [DistributionList](distributionlist.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="01e2f-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="01e2f-124">Text value</span></span>

<span data-ttu-id="01e2f-125">**Normalizedbody**要素のテキスト値は、アイテムの正規化された本文です。</span><span class="sxs-lookup"><span data-stu-id="01e2f-125">The text value of the **NormalizedBody** element is the normalized body of the item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="01e2f-126">注釈</span><span class="sxs-lookup"><span data-stu-id="01e2f-126">Remarks</span></span>

<span data-ttu-id="01e2f-127">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="01e2f-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="01e2f-128">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="01e2f-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="01e2f-129">要素の情報</span><span class="sxs-lookup"><span data-stu-id="01e2f-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="01e2f-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="01e2f-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="01e2f-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="01e2f-131">Schema name</span></span>  <br/> |<span data-ttu-id="01e2f-132">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="01e2f-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="01e2f-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="01e2f-133">Validation file</span></span>  <br/> |<span data-ttu-id="01e2f-134">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="01e2f-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="01e2f-135">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="01e2f-135">Can be empty</span></span>  <br/> ||
   

