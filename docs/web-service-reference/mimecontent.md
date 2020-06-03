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
description: MimeContent 要素には、base64Binary 形式で表され、[RFC2045] をサポートするオブジェクトの ASCII MIME ストリームが含まれています。
ms.openlocfilehash: 039ef1245d48e4cf13141970921dd210f4bd7d06
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530437"
---
# <a name="mimecontent"></a><span data-ttu-id="d9017-103">MimeContent</span><span class="sxs-lookup"><span data-stu-id="d9017-103">MimeContent</span></span>

<span data-ttu-id="d9017-104">**MimeContent**要素には、base64Binary 形式で表され、 [[RFC2045]](http://www.rfc-editor.org/rfc/rfc2045.txt)をサポートするオブジェクトの ASCII MIME ストリームが含まれています。</span><span class="sxs-lookup"><span data-stu-id="d9017-104">The **MimeContent** element contains the ASCII MIME stream of an object that is represented in base64Binary format and supports [[RFC2045]](http://www.rfc-editor.org/rfc/rfc2045.txt).</span></span>
  
```xml
<MimeContent CharacterSet="" />
```

 <span data-ttu-id="d9017-105">**MimeContentType**</span><span class="sxs-lookup"><span data-stu-id="d9017-105">**MimeContentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d9017-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d9017-106">Attributes and elements</span></span>

<span data-ttu-id="d9017-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d9017-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d9017-108">属性</span><span class="sxs-lookup"><span data-stu-id="d9017-108">Attributes</span></span>

|<span data-ttu-id="d9017-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="d9017-109">**Attribute**</span></span>|<span data-ttu-id="d9017-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="d9017-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d9017-111">**CharacterSet**</span><span class="sxs-lookup"><span data-stu-id="d9017-111">**CharacterSet**</span></span> <br/> |<span data-ttu-id="d9017-112">設定した場合、この属性の値はサーバーによって無視されます。</span><span class="sxs-lookup"><span data-stu-id="d9017-112">If set, the value for this attribute is ignored by the server.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d9017-113">子要素</span><span class="sxs-lookup"><span data-stu-id="d9017-113">Child elements</span></span>

<span data-ttu-id="d9017-114">なし。</span><span class="sxs-lookup"><span data-stu-id="d9017-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d9017-115">親要素</span><span class="sxs-lookup"><span data-stu-id="d9017-115">Parent elements</span></span>

<span data-ttu-id="d9017-116">[Calendaritem](calendaritem.md)  | [連絡先](contact.md)  | [DistributionList](distributionlist.md)  | [アイテム](item.md)  | [会議のキャンセル](meetingcancellation.md)  | [会議メッセージ](meetingmessage.md)  | [会議の要求](meetingrequest.md)  | [会議の応答](meetingresponse.md)  | [メッセージ](message-ex15websvcsotherref.md)  | [Removeitem](removeitem.md)  | [タスク](task.md)</span><span class="sxs-lookup"><span data-stu-id="d9017-116">[CalendarItem](calendaritem.md) | [Contact](contact.md) | [DistributionList](distributionlist.md) | [Item](item.md) | [MeetingCancellation](meetingcancellation.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [Message](message-ex15websvcsotherref.md) | [RemoveItem](removeitem.md) | [Task](task.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="d9017-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d9017-117">Text value</span></span>

<span data-ttu-id="d9017-118">この要素を使用する場合は、base64Binary MIME ストリームを表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="d9017-118">A text value that represents a base64Binary MIME stream is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d9017-119">注釈</span><span class="sxs-lookup"><span data-stu-id="d9017-119">Remarks</span></span>

<span data-ttu-id="d9017-120">メッセージコンテンツは、 **MimeContent**値に格納される前に、次の3つのエンコードレベルで行われます。</span><span class="sxs-lookup"><span data-stu-id="d9017-120">The message content goes through the following three levels of encoding before it is stored in the **MimeContent** value:</span></span> 
  
1. <span data-ttu-id="d9017-121">メッセージテキスト: これは、日本語の文字の iso-2022-jp などの本文のエンコードです。</span><span class="sxs-lookup"><span data-stu-id="d9017-121">Message text — This is the body encoding, such as iso-2022-jp for Japanese characters.</span></span>
    
2. <span data-ttu-id="d9017-122">MIME ストリーム—これは、 **MimeContent**要素のメッセージテキストの ASCII エンコード、または[MimeContentUTF8](mimecontentutf8.md)要素のメッセージテキストの UTF8 エンコードです。</span><span class="sxs-lookup"><span data-stu-id="d9017-122">MIME stream — This is the ASCII encoding of the message text for the **MimeContent** element, or the UTF8 encoding of the message text for the [MimeContentUTF8](mimecontentutf8.md) element.</span></span> 
    
3. <span data-ttu-id="d9017-123">XML ドキュメント—これは常に MIME ストリームの base64 でエンコードされた ASCII ストリームです。これは、XML に意味のある ' ' のような文字 \< が xml パーサーに表示されません。</span><span class="sxs-lookup"><span data-stu-id="d9017-123">XML document — This is always the base64-encoded ASCII stream of the MIME stream, where characters such as '\<', which are meaningful to XML, are hidden from XML parsers.</span></span>
    
<span data-ttu-id="d9017-124">各レベルは、その前にあるレベルから独立しています。</span><span class="sxs-lookup"><span data-stu-id="d9017-124">Each level is independent of the level that precedes it.</span></span>
  
<span data-ttu-id="d9017-125">**MimeContent**要素には、アイテムによって返されるその他のプロパティと同じデータが含まれている場合があります。</span><span class="sxs-lookup"><span data-stu-id="d9017-125">The **MimeContent** element might contain the same data that other properties that are returned with an item contain.</span></span> 
  
<span data-ttu-id="d9017-126">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d9017-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d9017-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d9017-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d9017-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="d9017-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d9017-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d9017-129">Schema Name</span></span>  <br/> |<span data-ttu-id="d9017-130">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d9017-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="d9017-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d9017-131">Validation File</span></span>  <br/> |<span data-ttu-id="d9017-132">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d9017-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d9017-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d9017-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="d9017-134">正しくない</span><span class="sxs-lookup"><span data-stu-id="d9017-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d9017-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="d9017-135">See also</span></span>



- [<span data-ttu-id="d9017-136">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d9017-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

