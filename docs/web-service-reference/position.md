---
title: Position
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 46726ebb-a403-4793-8378-282aa7dc39d0
description: Position 要素は、メッセージから抽出されたエンティティの位置を指定します。
ms.openlocfilehash: 9acd965c3e0c29f3fa91df338c0671749192b38b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465423"
---
# <a name="position"></a><span data-ttu-id="7b8b9-103">Position</span><span class="sxs-lookup"><span data-stu-id="7b8b9-103">Position</span></span>

<span data-ttu-id="7b8b9-104">**Position**要素は、メッセージから抽出されたエンティティの位置を指定します。</span><span class="sxs-lookup"><span data-stu-id="7b8b9-104">The **Position** element specifies the position of an entity extracted from a message.</span></span> 
  
```XML
<Position> LatestReply | Other | Subject | Signature </Position>
```

 <span data-ttu-id="7b8b9-105">**EmailPositionType**</span><span class="sxs-lookup"><span data-stu-id="7b8b9-105">**EmailPositionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7b8b9-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7b8b9-106">Attributes and elements</span></span>

<span data-ttu-id="7b8b9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7b8b9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7b8b9-108">属性</span><span class="sxs-lookup"><span data-stu-id="7b8b9-108">Attributes</span></span>

<span data-ttu-id="7b8b9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7b8b9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7b8b9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7b8b9-110">Child elements</span></span>

<span data-ttu-id="7b8b9-111">なし。</span><span class="sxs-lookup"><span data-stu-id="7b8b9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7b8b9-112">親要素</span><span class="sxs-lookup"><span data-stu-id="7b8b9-112">Parent elements</span></span>

<span data-ttu-id="7b8b9-113">[Urlentity](urlentity.md)  | [Addressentity](addressentity.md)  | [Emailaddressentity](emailaddressentity.md)  | [会議の提案](meetingsuggestion.md)  | [Contact (ContactType)](contact-contacttype.md)  | [Phone (通し entitytype)](phone-phoneentitytype.md)  | [Tasksuggestion](tasksuggestion.md)</span><span class="sxs-lookup"><span data-stu-id="7b8b9-113">[UrlEntity](urlentity.md) | [AddressEntity](addressentity.md) | [EmailAddressEntity](emailaddressentity.md) | [MeetingSuggestion](meetingsuggestion.md) | [Contact (ContactType)](contact-contacttype.md) | [Phone (PhoneEntityType)](phone-phoneentitytype.md) | [TaskSuggestion](tasksuggestion.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="7b8b9-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7b8b9-114">Text value</span></span>

<span data-ttu-id="7b8b9-115">**Position**要素のテキスト値は、抽出されたエンティティがソースメッセージ内で発生した場所です。</span><span class="sxs-lookup"><span data-stu-id="7b8b9-115">The text value of the **Position** element is the location where an extracted entity originated in the source message.</span></span> <span data-ttu-id="7b8b9-116">**Position**要素のテキスト値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="7b8b9-116">The text values for the **Position** element are:</span></span> 
  
- <span data-ttu-id="7b8b9-117">**LatestReply** -抽出されたエンティティは、メッセージに対する最新の返信から発信されます。</span><span class="sxs-lookup"><span data-stu-id="7b8b9-117">**LatestReply** - the extracted entity originates from the latest reply to the message.</span></span> 
    
- <span data-ttu-id="7b8b9-118">**その他**-抽出されたエンティティは、メッセージの未定義の部分から生成されます。</span><span class="sxs-lookup"><span data-stu-id="7b8b9-118">**Other** - the extracted entity originates from an undefined part of the message.</span></span> 
    
- <span data-ttu-id="7b8b9-119">**Subject** -抽出されたエンティティは、メッセージの件名から発信されます。</span><span class="sxs-lookup"><span data-stu-id="7b8b9-119">**Subject** - the extracted entity originates from the message subject.</span></span> 
    
- <span data-ttu-id="7b8b9-120">**Signature** -抽出されたエンティティは、メッセージの署名から発信されます。</span><span class="sxs-lookup"><span data-stu-id="7b8b9-120">**Signature** - the extracted entity originates from the message signature.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="7b8b9-121">注釈</span><span class="sxs-lookup"><span data-stu-id="7b8b9-121">Remarks</span></span>

<span data-ttu-id="7b8b9-122">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="7b8b9-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7b8b9-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7b8b9-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7b8b9-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7b8b9-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7b8b9-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="7b8b9-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7b8b9-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7b8b9-126">Schema name</span></span>  <br/> |<span data-ttu-id="7b8b9-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="7b8b9-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="7b8b9-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7b8b9-128">Validation file</span></span>  <br/> |<span data-ttu-id="7b8b9-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="7b8b9-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7b8b9-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="7b8b9-130">Can be empty</span></span>  <br/> ||
   

