---
title: MimeContentUTF8
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 31544c95-5231-4b57-958c-2a689464d29b
description: MimeContentUTF8 要素には、base64Binary の形式で表されるオブジェクトの UTF-8 の MIME ストリームが含まれているし、e メール アドレスの国際化をサポートし、[RFC6530]。
ms.openlocfilehash: 47599b6634738fd488e5b020f69e36d5fcf550a6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832466"
---
# <a name="mimecontentutf8"></a><span data-ttu-id="648b2-103">MimeContentUTF8</span><span class="sxs-lookup"><span data-stu-id="648b2-103">MimeContentUTF8</span></span>

<span data-ttu-id="648b2-104">**MimeContentUTF8**要素には、base64Binary の形式で表され、 [[RFC6530]](http://www.rfc-editor.org/rfc/rfc6530.txt)電子メール アドレスの国際化をサポートしているオブジェクトの UTF-8 の MIME ストリームが含まれています。</span><span class="sxs-lookup"><span data-stu-id="648b2-104">The **MimeContentUTF8** element contains the UTF-8 MIME stream of an object that is represented in base64Binary format and supports email address internationalization and [[RFC6530]](http://www.rfc-editor.org/rfc/rfc6530.txt).</span></span>
  
```XML
<MimeContentUTF8 CharacterSet="" />
```

 <span data-ttu-id="648b2-105">**MimeContentType**</span><span class="sxs-lookup"><span data-stu-id="648b2-105">**MimeContentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="648b2-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="648b2-106">Attributes and elements</span></span>

<span data-ttu-id="648b2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="648b2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="648b2-108">属性</span><span class="sxs-lookup"><span data-stu-id="648b2-108">Attributes</span></span>

|<span data-ttu-id="648b2-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="648b2-109">**Attribute**</span></span>|<span data-ttu-id="648b2-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="648b2-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="648b2-111">**文字セット**</span><span class="sxs-lookup"><span data-stu-id="648b2-111">**CharacterSet**</span></span> <br/> |<span data-ttu-id="648b2-112">かどうか、この属性の値は無視されます、サーバーがします。</span><span class="sxs-lookup"><span data-stu-id="648b2-112">If set, the value for this attribute is ignored by the server.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="648b2-113">子要素</span><span class="sxs-lookup"><span data-stu-id="648b2-113">Child elements</span></span>

<span data-ttu-id="648b2-114">なし。</span><span class="sxs-lookup"><span data-stu-id="648b2-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="648b2-115">親要素</span><span class="sxs-lookup"><span data-stu-id="648b2-115">Parent elements</span></span>

<span data-ttu-id="648b2-116">[カレンダー項目](calendaritem.md) | [連絡先](contact.md) | [DistributionList](distributionlist.md) | [アイテム](item.md) | [MeetingCancellation](meetingcancellation.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md)  |  [MeetingResponse](meetingresponse.md) | [メッセージ](message-ex15websvcsotherref.md) | [での RemoveItem](removeitem.md) | [タスク](task.md)</span><span class="sxs-lookup"><span data-stu-id="648b2-116">[CalendarItem](calendaritem.md) | [Contact](contact.md) | [DistributionList](distributionlist.md) | [Item](item.md) | [MeetingCancellation](meetingcancellation.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [Message](message-ex15websvcsotherref.md) | [RemoveItem](removeitem.md) | [Task](task.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="648b2-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="648b2-117">Text value</span></span>

<span data-ttu-id="648b2-118">Base64binary の MIME ストリームを表すテキスト値は、この要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="648b2-118">A text value that represents a base64binary MIME stream is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="648b2-119">備考</span><span class="sxs-lookup"><span data-stu-id="648b2-119">Remarks</span></span>

<span data-ttu-id="648b2-120">メッセージの内容は次の 3 つのレベルの**MimeContentUTF8**の値に格納される前にエンコードします。</span><span class="sxs-lookup"><span data-stu-id="648b2-120">The message content goes through the following three levels of encoding before it is stored in the **MimeContentUTF8** value:</span></span> 
  
1. <span data-ttu-id="648b2-121">メッセージ テキスト、本文のエンコーディングには、iso 2022 の jp 日本語の文字などは、これ。</span><span class="sxs-lookup"><span data-stu-id="648b2-121">Message text — This is the body encoding, such as iso-2022-jp for Japanese characters.</span></span>
    
2. <span data-ttu-id="648b2-122">MIME ストリーム-これは、UTF8 エンコーディングのメッセージ要素のテキスト、 **MimeContentUTF8** 、または[MimeContent](mimecontent.md)要素のメッセージ テキストの ASCII エンコードします。</span><span class="sxs-lookup"><span data-stu-id="648b2-122">MIME stream — This is the UTF8 encoding of the message text for the **MimeContentUTF8** element, or the ASCII encoding of the message text for the [MimeContent](mimecontent.md) element.</span></span> 
    
3. <span data-ttu-id="648b2-123">XML ドキュメント-これは、常に base64 でエンコードされた ASCII ストリーム、MIME ストリームの場所などの文字 '\<'、XML パーサーから非表示には、xml では、意味のあります。</span><span class="sxs-lookup"><span data-stu-id="648b2-123">XML document — This is always the base64-encoded ASCII stream of the MIME stream, where characters such as '\<', which are meaningful to XML, are hidden from XML parsers.</span></span>
    
<span data-ttu-id="648b2-124">各レベルでは、その前にあるレベルの独立しています。</span><span class="sxs-lookup"><span data-stu-id="648b2-124">Each level is independent of the level that precedes it.</span></span>
  
<span data-ttu-id="648b2-125">**MimeContentUTF8**要素には、アイテムが返されるその他のプロパティが含まれている同じデータが含まれて可能性があります。</span><span class="sxs-lookup"><span data-stu-id="648b2-125">The **MimeContentUTF8** element might contain the same data that other properties that are returned with an item contain.</span></span> 
  
<span data-ttu-id="648b2-126">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="648b2-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="648b2-127">バージョンの相違点</span><span class="sxs-lookup"><span data-stu-id="648b2-127">Version differences</span></span>

<span data-ttu-id="648b2-128">この要素は、Exchange のビルド 15.00.0986.00 以降のバージョンで利用できます。</span><span class="sxs-lookup"><span data-stu-id="648b2-128">This element is available in versions of Exchange starting with build 15.00.0986.00.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="648b2-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="648b2-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="648b2-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="648b2-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="648b2-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="648b2-131">Schema Name</span></span>  <br/> |<span data-ttu-id="648b2-132">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="648b2-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="648b2-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="648b2-133">Validation File</span></span>  <br/> |<span data-ttu-id="648b2-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="648b2-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="648b2-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="648b2-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="648b2-136">False</span><span class="sxs-lookup"><span data-stu-id="648b2-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="648b2-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="648b2-137">See also</span></span>



- [<span data-ttu-id="648b2-138">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="648b2-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

