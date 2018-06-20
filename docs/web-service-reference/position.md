---
title: 位置
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 46726ebb-a403-4793-8378-282aa7dc39d0
description: 位置の要素は、メッセージから抽出されたエンティティの位置を指定します。
ms.openlocfilehash: 4bd8f3088891e918e13d5ef1ec8e3e5217cb3fa1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832853"
---
# <a name="position"></a><span data-ttu-id="22f45-103">位置</span><span class="sxs-lookup"><span data-stu-id="22f45-103">Position</span></span>

<span data-ttu-id="22f45-104">**位置**の要素は、メッセージから抽出されたエンティティの位置を指定します。</span><span class="sxs-lookup"><span data-stu-id="22f45-104">The **Position** element specifies the position of an entity extracted from a message.</span></span> 
  
```XML
<Position> LatestReply | Other | Subject | Signature </Position>
```

 <span data-ttu-id="22f45-105">**EmailPositionType**</span><span class="sxs-lookup"><span data-stu-id="22f45-105">**EmailPositionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="22f45-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="22f45-106">Attributes and elements</span></span>

<span data-ttu-id="22f45-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="22f45-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="22f45-108">属性</span><span class="sxs-lookup"><span data-stu-id="22f45-108">Attributes</span></span>

<span data-ttu-id="22f45-109">なし。</span><span class="sxs-lookup"><span data-stu-id="22f45-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="22f45-110">子要素</span><span class="sxs-lookup"><span data-stu-id="22f45-110">Child elements</span></span>

<span data-ttu-id="22f45-111">なし。</span><span class="sxs-lookup"><span data-stu-id="22f45-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="22f45-112">親要素</span><span class="sxs-lookup"><span data-stu-id="22f45-112">Parent elements</span></span>

<span data-ttu-id="22f45-113">[UrlEntity](urlentity.md) | [AddressEntity](addressentity.md) | [EmailAddressEntity](emailaddressentity.md) | [MeetingSuggestion](meetingsuggestion.md) | [連絡先 (ContactType)](contact-contacttype.md) | [電話 (PhoneEntityType)](phone-phoneentitytype.md)  |  [TaskSuggestion](tasksuggestion.md)</span><span class="sxs-lookup"><span data-stu-id="22f45-113">[UrlEntity](urlentity.md) | [AddressEntity](addressentity.md) | [EmailAddressEntity](emailaddressentity.md) | [MeetingSuggestion](meetingsuggestion.md) | [Contact (ContactType)](contact-contacttype.md) | [Phone (PhoneEntityType)](phone-phoneentitytype.md) | [TaskSuggestion](tasksuggestion.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="22f45-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="22f45-114">Text value</span></span>

<span data-ttu-id="22f45-115">**位置**の要素のテキスト値は、送信元のメッセージの抽出されたエンティティが作成される場所です。</span><span class="sxs-lookup"><span data-stu-id="22f45-115">The text value of the **Position** element is the location where an extracted entity originated in the source message.</span></span> <span data-ttu-id="22f45-116">**位置**の要素のテキスト値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="22f45-116">The text values for the **Position** element are:</span></span> 
  
- <span data-ttu-id="22f45-117">**LatestReply**の抽出されたエンティティは、最新の返信メッセージから生成されます。</span><span class="sxs-lookup"><span data-stu-id="22f45-117">**LatestReply** - the extracted entity originates from the latest reply to the message.</span></span> 
    
- <span data-ttu-id="22f45-118">**他**の抽出されたエンティティの発生元、メッセージの部分で定義されていないからです。</span><span class="sxs-lookup"><span data-stu-id="22f45-118">**Other** - the extracted entity originates from an undefined part of the message.</span></span> 
    
- <span data-ttu-id="22f45-119">**件名**の抽出されたエンティティは、メッセージの件名から発生します。</span><span class="sxs-lookup"><span data-stu-id="22f45-119">**Subject** - the extracted entity originates from the message subject.</span></span> 
    
- <span data-ttu-id="22f45-120">**署名**の抽出されたエンティティは、メッセージの署名から発生します。</span><span class="sxs-lookup"><span data-stu-id="22f45-120">**Signature** - the extracted entity originates from the message signature.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="22f45-121">備考</span><span class="sxs-lookup"><span data-stu-id="22f45-121">Remarks</span></span>

<span data-ttu-id="22f45-122">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="22f45-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="22f45-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="22f45-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="22f45-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="22f45-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="22f45-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="22f45-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="22f45-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="22f45-126">Schema name</span></span>  <br/> |<span data-ttu-id="22f45-127">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="22f45-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="22f45-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="22f45-128">Validation file</span></span>  <br/> |<span data-ttu-id="22f45-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="22f45-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="22f45-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="22f45-130">Can be empty</span></span>  <br/> ||
   

