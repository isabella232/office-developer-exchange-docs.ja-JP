---
title: MeetingSuggestion
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d6012063-eb67-4e83-a4a6-33482685083f
description: MeetingSuggestion 要素は、提案された会議を指定します。
ms.openlocfilehash: 35b618b32101ea36c35d87ca0737e4a7e04eb3a9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832444"
---
# <a name="meetingsuggestion"></a><span data-ttu-id="7f77c-103">MeetingSuggestion</span><span class="sxs-lookup"><span data-stu-id="7f77c-103">MeetingSuggestion</span></span>

<span data-ttu-id="7f77c-104">**MeetingSuggestion**要素は、提案された会議を指定します。</span><span class="sxs-lookup"><span data-stu-id="7f77c-104">The **MeetingSuggestion** element specifies a proposed meeting.</span></span> 
  
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

 <span data-ttu-id="7f77c-105">**MeetingSuggestionType**</span><span class="sxs-lookup"><span data-stu-id="7f77c-105">**MeetingSuggestionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7f77c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7f77c-106">Attributes and elements</span></span>

<span data-ttu-id="7f77c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7f77c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7f77c-108">属性</span><span class="sxs-lookup"><span data-stu-id="7f77c-108">Attributes</span></span>

<span data-ttu-id="7f77c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7f77c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7f77c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7f77c-110">Child elements</span></span>

<span data-ttu-id="7f77c-111">[参加者](attendees.md) | [の場所](location.md) | [件名](subject.md) | [MeetingString](meetingstring.md) | [開始時刻](starttime.md) | [終了時刻](endtime.md)</span><span class="sxs-lookup"><span data-stu-id="7f77c-111">[Attendees](attendees.md) | [Location](location.md) | [Subject](subject.md) | [MeetingString](meetingstring.md) | [StartTime](starttime.md) | [EndTime](endtime.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7f77c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="7f77c-112">Parent elements</span></span>

[<span data-ttu-id="7f77c-113">MeetingSuggestions</span><span class="sxs-lookup"><span data-stu-id="7f77c-113">MeetingSuggestions</span></span>](meetingsuggestions.md)
  
## <a name="remarks"></a><span data-ttu-id="7f77c-114">備考</span><span class="sxs-lookup"><span data-stu-id="7f77c-114">Remarks</span></span>

<span data-ttu-id="7f77c-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="7f77c-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7f77c-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7f77c-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7f77c-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="7f77c-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7f77c-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="7f77c-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7f77c-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7f77c-119">Schema name</span></span>  <br/> |<span data-ttu-id="7f77c-120">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="7f77c-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="7f77c-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7f77c-121">Validation file</span></span>  <br/> |<span data-ttu-id="7f77c-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7f77c-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7f77c-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="7f77c-123">Can be empty</span></span>  <br/> ||
   

