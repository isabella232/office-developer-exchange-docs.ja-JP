---
title: AssociatedCalendarItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AssociatedCalendarItemId
api_type:
- schema
ms.assetid: 5b29898c-ea59-4e6a-914c-c011ec754032
description: AssociatedCalendarItemId 要素は、会議のメッセージ、会議の依頼、会議の応答、会議の取り消し、または ReminderMessageData に関連付けられている予定表アイテムを表します。
ms.openlocfilehash: 816372c38243ba0fe5a7606c264dd1c5107350f2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460884"
---
# <a name="associatedcalendaritemid"></a><span data-ttu-id="d503a-103">AssociatedCalendarItemId</span><span class="sxs-lookup"><span data-stu-id="d503a-103">AssociatedCalendarItemId</span></span>

<span data-ttu-id="d503a-104">**AssociatedCalendarItemId**要素は、[会議のメッセージ](meetingmessage.md)、[会議の依頼](meetingrequest.md)、会議の[応答](meetingresponse.md)、会議の[取り消し](meetingcancellation.md)、または[ReminderMessageData](remindermessagedata.md)に関連付けられている予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="d503a-104">The **AssociatedCalendarItemId** element represents the calendar item that is associated with a [MeetingMessage](meetingmessage.md), [MeetingRequest](meetingrequest.md), [MeetingResponse](meetingresponse.md), [MeetingCancellation](meetingcancellation.md), or [ReminderMessageData](remindermessagedata.md).</span></span>
  
```XML
<AssociatedCalendarItemId Id="" ChangeKey=""/>
```

 <span data-ttu-id="d503a-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="d503a-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d503a-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d503a-106">Attributes and elements</span></span>

<span data-ttu-id="d503a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d503a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d503a-108">属性</span><span class="sxs-lookup"><span data-stu-id="d503a-108">Attributes</span></span>

|<span data-ttu-id="d503a-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="d503a-109">**Attribute**</span></span>|<span data-ttu-id="d503a-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="d503a-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d503a-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="d503a-111">**Id**</span></span> <br/> |<span data-ttu-id="d503a-112">会議に関連付けられている予定表アイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="d503a-112">Identifies the calendar item that is associated with meeting.</span></span>  <br/> |
|<span data-ttu-id="d503a-113">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="d503a-113">**ChangeKey**</span></span> <br/> |<span data-ttu-id="d503a-114">会議に関連付けられている予定表アイテムの特定のバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="d503a-114">Identifies a specific version of the calendar item that is associated with a meeting.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d503a-115">子要素</span><span class="sxs-lookup"><span data-stu-id="d503a-115">Child elements</span></span>

<span data-ttu-id="d503a-116">なし。</span><span class="sxs-lookup"><span data-stu-id="d503a-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d503a-117">親要素</span><span class="sxs-lookup"><span data-stu-id="d503a-117">Parent elements</span></span>

<span data-ttu-id="d503a-118">[会議メッセージ](meetingmessage.md)  | [会議の要求](meetingrequest.md)  | [会議の応答](meetingresponse.md)  | [会議のキャンセル](meetingcancellation.md)  | [ReminderMessageData](remindermessagedata.md)</span><span class="sxs-lookup"><span data-stu-id="d503a-118">[MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [MeetingCancellation](meetingcancellation.md) | [ReminderMessageData](remindermessagedata.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d503a-119">注釈</span><span class="sxs-lookup"><span data-stu-id="d503a-119">Remarks</span></span>

<span data-ttu-id="d503a-120">ビルド番号15.00.0913.09 以降のバージョンの Exchange では、 **ReminderMessageData**要素の子要素として**AssociatedCalendarItemId**要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="d503a-120">Versions of Exchange starting with build number 15.00.0913.09 can include the **AssociatedCalendarItemId** element as a child element of the **ReminderMessageData** element.</span></span> 
  
<span data-ttu-id="d503a-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d503a-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d503a-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d503a-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d503a-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="d503a-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d503a-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d503a-124">Schema Name</span></span>  <br/> |<span data-ttu-id="d503a-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d503a-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="d503a-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d503a-126">Validation File</span></span>  <br/> |<span data-ttu-id="d503a-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d503a-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d503a-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d503a-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="d503a-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="d503a-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d503a-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="d503a-130">See also</span></span>

- [<span data-ttu-id="d503a-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d503a-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

