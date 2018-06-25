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
description: AssociatedCalendarItemId 要素は、MeetingMessage、MeetingRequest、MeetingResponse、MeetingCancellation、または ReminderMessageData に関連付けられている予定表アイテムを表します。
ms.openlocfilehash: 4445da88d6fec42c1e02cd8de4d2e423485a4472
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759448"
---
# <a name="associatedcalendaritemid"></a><span data-ttu-id="bfd97-103">AssociatedCalendarItemId</span><span class="sxs-lookup"><span data-stu-id="bfd97-103">AssociatedCalendarItemId</span></span>

<span data-ttu-id="bfd97-104">**AssociatedCalendarItemId**要素は、 [MeetingMessage](meetingmessage.md)、 [MeetingRequest](meetingrequest.md)、 [MeetingResponse](meetingresponse.md)、 [MeetingCancellation](meetingcancellation.md)、または[ReminderMessageData](remindermessagedata.md)に関連付けられている予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="bfd97-104">The **AssociatedCalendarItemId** element represents the calendar item that is associated with a [MeetingMessage](meetingmessage.md), [MeetingRequest](meetingrequest.md), [MeetingResponse](meetingresponse.md), [MeetingCancellation](meetingcancellation.md), or [ReminderMessageData](remindermessagedata.md).</span></span>
  
```XML
<AssociatedCalendarItemId Id="" ChangeKey=""/>
```

 <span data-ttu-id="bfd97-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="bfd97-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bfd97-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="bfd97-106">Attributes and elements</span></span>

<span data-ttu-id="bfd97-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="bfd97-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bfd97-108">属性</span><span class="sxs-lookup"><span data-stu-id="bfd97-108">Attributes</span></span>

|<span data-ttu-id="bfd97-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="bfd97-109">**Attribute**</span></span>|<span data-ttu-id="bfd97-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="bfd97-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bfd97-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="bfd97-111">**Id**</span></span> <br/> |<span data-ttu-id="bfd97-112">会議に関連付けられている予定表アイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="bfd97-112">Identifies the calendar item that is associated with meeting.</span></span>  <br/> |
|<span data-ttu-id="bfd97-113">**変更キー**</span><span class="sxs-lookup"><span data-stu-id="bfd97-113">**ChangeKey**</span></span> <br/> |<span data-ttu-id="bfd97-114">会議に関連付けられている予定表アイテムの特定のバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="bfd97-114">Identifies a specific version of the calendar item that is associated with a meeting.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="bfd97-115">子要素</span><span class="sxs-lookup"><span data-stu-id="bfd97-115">Child elements</span></span>

<span data-ttu-id="bfd97-116">なし。</span><span class="sxs-lookup"><span data-stu-id="bfd97-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bfd97-117">親要素</span><span class="sxs-lookup"><span data-stu-id="bfd97-117">Parent elements</span></span>

<span data-ttu-id="bfd97-118">[MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [MeetingCancellation](meetingcancellation.md) | [ReminderMessageData](remindermessagedata.md)</span><span class="sxs-lookup"><span data-stu-id="bfd97-118">[MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [MeetingCancellation](meetingcancellation.md) | [ReminderMessageData](remindermessagedata.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bfd97-119">備考</span><span class="sxs-lookup"><span data-stu-id="bfd97-119">Remarks</span></span>

<span data-ttu-id="bfd97-120">Exchange のビルド番号 15.00.0913.09 以降のバージョンでは、 **ReminderMessageData**要素の子要素として**AssociatedCalendarItemId**の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="bfd97-120">Versions of Exchange starting with build number 15.00.0913.09 can include the **AssociatedCalendarItemId** element as a child element of the **ReminderMessageData** element.</span></span> 
  
<span data-ttu-id="bfd97-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="bfd97-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bfd97-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="bfd97-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bfd97-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="bfd97-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bfd97-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="bfd97-124">Schema Name</span></span>  <br/> |<span data-ttu-id="bfd97-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="bfd97-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="bfd97-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="bfd97-126">Validation File</span></span>  <br/> |<span data-ttu-id="bfd97-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bfd97-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bfd97-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="bfd97-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="bfd97-129">False</span><span class="sxs-lookup"><span data-stu-id="bfd97-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bfd97-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="bfd97-130">See also</span></span>

- [<span data-ttu-id="bfd97-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="bfd97-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

