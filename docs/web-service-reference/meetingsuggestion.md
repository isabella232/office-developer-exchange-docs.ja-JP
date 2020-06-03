---
title: MeetingSuggestion
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d6012063-eb67-4e83-a4a6-33482685083f
description: 会議提案要素は、提案された会議を指定します。
ms.openlocfilehash: 132ed907886c0ee9f3c4f46cc835d4b4fc6aa621
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466312"
---
# <a name="meetingsuggestion"></a><span data-ttu-id="82313-103">MeetingSuggestion</span><span class="sxs-lookup"><span data-stu-id="82313-103">MeetingSuggestion</span></span>

<span data-ttu-id="82313-104">会議**提案**要素は、提案された会議を指定します。</span><span class="sxs-lookup"><span data-stu-id="82313-104">The **MeetingSuggestion** element specifies a proposed meeting.</span></span> 
  
```XML
<MeetingSuggestion>
   <Attendees/>
   <Location/>
   <Subject/>
   <MeetingString/>
   <StartTime/>
   <EndTime/>
</MeetingSuggestion>
```

 <span data-ttu-id="82313-105">**MeetingSuggestionType**</span><span class="sxs-lookup"><span data-stu-id="82313-105">**MeetingSuggestionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="82313-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="82313-106">Attributes and elements</span></span>

<span data-ttu-id="82313-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="82313-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="82313-108">属性</span><span class="sxs-lookup"><span data-stu-id="82313-108">Attributes</span></span>

<span data-ttu-id="82313-109">なし。</span><span class="sxs-lookup"><span data-stu-id="82313-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="82313-110">子要素</span><span class="sxs-lookup"><span data-stu-id="82313-110">Child elements</span></span>

<span data-ttu-id="82313-111">[出席者](attendees.md)  | [場所](location.md)  | [件名](subject.md)  | [会議の文字列](meetingstring.md)  | [StartTime](starttime.md)  | [EndTime](endtime.md)</span><span class="sxs-lookup"><span data-stu-id="82313-111">[Attendees](attendees.md) | [Location](location.md) | [Subject](subject.md) | [MeetingString](meetingstring.md) | [StartTime](starttime.md) | [EndTime](endtime.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="82313-112">親要素</span><span class="sxs-lookup"><span data-stu-id="82313-112">Parent elements</span></span>

[<span data-ttu-id="82313-113">MeetingSuggestions</span><span class="sxs-lookup"><span data-stu-id="82313-113">MeetingSuggestions</span></span>](meetingsuggestions.md)
  
## <a name="remarks"></a><span data-ttu-id="82313-114">注釈</span><span class="sxs-lookup"><span data-stu-id="82313-114">Remarks</span></span>

<span data-ttu-id="82313-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="82313-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="82313-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="82313-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="82313-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="82313-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="82313-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="82313-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="82313-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="82313-119">Schema name</span></span>  <br/> |<span data-ttu-id="82313-120">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="82313-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="82313-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="82313-121">Validation file</span></span>  <br/> |<span data-ttu-id="82313-122">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="82313-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="82313-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="82313-123">Can be empty</span></span>  <br/> ||
   

