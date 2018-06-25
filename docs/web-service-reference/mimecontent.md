---
title: MimeContent
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MimeContent
api_type:
- schema
ms.assetid: 4f472a08-5653-4c54-ba65-831dfe32f20f
description: MimeContent 要素には、ASCII の MIME ストリーム base64Binary の形式で表され、[RFC2045] をサポートしているオブジェクトが含まれています。
ms.openlocfilehash: 60f2d42f09347611559137c494d93036f1192829
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832465"
---
# <a name="mimecontent"></a><span data-ttu-id="69707-103">MimeContent</span><span class="sxs-lookup"><span data-stu-id="69707-103">MimeContent</span></span>

<span data-ttu-id="69707-104">**MimeContent**要素には、ASCII の MIME ストリーム base64Binary の形式で表され、 [[RFC2045]](http://www.rfc-editor.org/rfc/rfc2045.txt)をサポートしているオブジェクトが含まれています。</span><span class="sxs-lookup"><span data-stu-id="69707-104">The **MimeContent** element contains the ASCII MIME stream of an object that is represented in base64Binary format and supports [[RFC2045]](http://www.rfc-editor.org/rfc/rfc2045.txt).</span></span>
  
```xml
<MimeContent CharacterSet="" />
```

 <span data-ttu-id="69707-105">**MimeContentType**</span><span class="sxs-lookup"><span data-stu-id="69707-105">**MimeContentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="69707-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="69707-106">Attributes and elements</span></span>

<span data-ttu-id="69707-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="69707-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="69707-108">属性</span><span class="sxs-lookup"><span data-stu-id="69707-108">Attributes</span></span>

|<span data-ttu-id="69707-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="69707-109">**Attribute**</span></span>|<span data-ttu-id="69707-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="69707-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="69707-111">**文字セット**</span><span class="sxs-lookup"><span data-stu-id="69707-111">**CharacterSet**</span></span> <br/> |<span data-ttu-id="69707-112">かどうか、この属性の値は無視されます、サーバーがします。</span><span class="sxs-lookup"><span data-stu-id="69707-112">If set, the value for this attribute is ignored by the server.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="69707-113">子要素</span><span class="sxs-lookup"><span data-stu-id="69707-113">Child elements</span></span>

<span data-ttu-id="69707-114">なし。</span><span class="sxs-lookup"><span data-stu-id="69707-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="69707-115">親要素</span><span class="sxs-lookup"><span data-stu-id="69707-115">Parent elements</span></span>

<span data-ttu-id="69707-116">[カレンダー項目](calendaritem.md) | [連絡先](contact.md) | [DistributionList](distributionlist.md) | [アイテム](item.md) | [MeetingCancellation](meetingcancellation.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md)  |  [MeetingResponse](meetingresponse.md) | [メッセージ](message-ex15websvcsotherref.md) | [での RemoveItem](removeitem.md) | [タスク](task.md)</span><span class="sxs-lookup"><span data-stu-id="69707-116">[CalendarItem](calendaritem.md) | [Contact](contact.md) | [DistributionList](distributionlist.md) | [Item](item.md) | [MeetingCancellation](meetingcancellation.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [Message](message-ex15websvcsotherref.md) | [RemoveItem](removeitem.md) | [Task](task.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="69707-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="69707-117">Text value</span></span>

<span data-ttu-id="69707-118">Base64Binary の MIME ストリームを表すテキスト値は、この要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="69707-118">A text value that represents a base64Binary MIME stream is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="69707-119">備考</span><span class="sxs-lookup"><span data-stu-id="69707-119">Remarks</span></span>

<span data-ttu-id="69707-120">メッセージの内容のエンコーディングの**MimeContent**値に格納される前に次の 3 つのレベルを通過します。</span><span class="sxs-lookup"><span data-stu-id="69707-120">The message content goes through the following three levels of encoding before it is stored in the **MimeContent** value:</span></span> 
  
1. <span data-ttu-id="69707-121">メッセージ テキスト、本文のエンコーディングには、iso 2022 の jp 日本語の文字などは、これ。</span><span class="sxs-lookup"><span data-stu-id="69707-121">Message text — This is the body encoding, such as iso-2022-jp for Japanese characters.</span></span>
    
2. <span data-ttu-id="69707-122">MIME ストリーム- **MimeContent**要素のメッセージ テキストの ASCII エンコードまたは[MimeContentUTF8](mimecontentutf8.md)要素のメッセージ テキストの UTF8 エンコードします。</span><span class="sxs-lookup"><span data-stu-id="69707-122">MIME stream — This is the ASCII encoding of the message text for the **MimeContent** element, or the UTF8 encoding of the message text for the [MimeContentUTF8](mimecontentutf8.md) element.</span></span> 
    
3. <span data-ttu-id="69707-123">XML ドキュメント-これは、常に base64 でエンコードされた ASCII ストリーム、MIME ストリームの場所などの文字 '\<'、XML パーサーから非表示には、xml では、意味のあります。</span><span class="sxs-lookup"><span data-stu-id="69707-123">XML document — This is always the base64-encoded ASCII stream of the MIME stream, where characters such as '\<', which are meaningful to XML, are hidden from XML parsers.</span></span>
    
<span data-ttu-id="69707-124">各レベルでは、その前にあるレベルの独立しています。</span><span class="sxs-lookup"><span data-stu-id="69707-124">Each level is independent of the level that precedes it.</span></span>
  
<span data-ttu-id="69707-125">**MimeContent**要素には、アイテムが返されるその他のプロパティが含まれている同じデータが含まれて可能性があります。</span><span class="sxs-lookup"><span data-stu-id="69707-125">The **MimeContent** element might contain the same data that other properties that are returned with an item contain.</span></span> 
  
<span data-ttu-id="69707-126">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="69707-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="69707-127">要素情報</span><span class="sxs-lookup"><span data-stu-id="69707-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="69707-128">名前空間</span><span class="sxs-lookup"><span data-stu-id="69707-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="69707-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="69707-129">Schema Name</span></span>  <br/> |<span data-ttu-id="69707-130">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="69707-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="69707-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="69707-131">Validation File</span></span>  <br/> |<span data-ttu-id="69707-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="69707-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="69707-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="69707-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="69707-134">False</span><span class="sxs-lookup"><span data-stu-id="69707-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="69707-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="69707-135">See also</span></span>



- [<span data-ttu-id="69707-136">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="69707-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

