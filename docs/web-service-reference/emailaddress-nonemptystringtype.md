---
title: EmailAddress (NonEmptyStringType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- EmailAddress
api_type:
- schema
ms.assetid: c0c708d1-b016-4902-a294-9af44aea2050
description: EmailAddress 要素は、メールボックスのユーザーのプライマリ SMTP アドレスを定義します。
ms.openlocfilehash: fcf2839c1e2e40a22d6b6a856608f52f2c9c2a1a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760223"
---
# <a name="emailaddress-nonemptystringtype"></a><span data-ttu-id="058f3-103">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="058f3-103">EmailAddress (NonEmptyStringType)</span></span>

<span data-ttu-id="058f3-104">**EmailAddress**要素は、メールボックスのユーザーのプライマリ SMTP アドレスを定義します。</span><span class="sxs-lookup"><span data-stu-id="058f3-104">The **EmailAddress** element defines the primary SMTP address of a mailbox user.</span></span> 
  
```XML
<EmailAddress/>
```

 <span data-ttu-id="058f3-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="058f3-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="058f3-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="058f3-106">Attributes and elements</span></span>

<span data-ttu-id="058f3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="058f3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="058f3-108">属性</span><span class="sxs-lookup"><span data-stu-id="058f3-108">Attributes</span></span>

<span data-ttu-id="058f3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="058f3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="058f3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="058f3-110">Child elements</span></span>

<span data-ttu-id="058f3-111">なし。</span><span class="sxs-lookup"><span data-stu-id="058f3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="058f3-112">親要素</span><span class="sxs-lookup"><span data-stu-id="058f3-112">Parent elements</span></span>

|<span data-ttu-id="058f3-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="058f3-113">**Element**</span></span>|<span data-ttu-id="058f3-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="058f3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="058f3-115">ActingAs</span><span class="sxs-lookup"><span data-stu-id="058f3-115">ActingAs</span></span>](actingas.md) <br/> |<span data-ttu-id="058f3-116">として送信する呼び出し元を識別します。</span><span class="sxs-lookup"><span data-stu-id="058f3-116">Identifies who the caller is sending as.</span></span>  <br/> |
|[<span data-ttu-id="058f3-117">メールボックス</span><span class="sxs-lookup"><span data-stu-id="058f3-117">Mailbox</span></span>](mailbox.md) <br/> | <span data-ttu-id="058f3-118">完全に解決された電子メール アドレスを識別します。</span><span class="sxs-lookup"><span data-stu-id="058f3-118">Identifies a fully resolved e-mail address.</span></span>  <br/><br/><span data-ttu-id="058f3-119">この要素にいくつかの XPath 式は、次のように。</span><span class="sxs-lookup"><span data-stu-id="058f3-119">The following are some XPath expressions to this element:</span></span><br/><br/>`/CreateItem/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`/CreateFolder/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`CreateItem/Items/AcceptItem/ToRecipients/Mailbox`<br/><br/>`SyncFolderItemsResponseMessage/Changes/Create/CalendarItem/ConflictingMeetings/AcceptItem/CcRecipients/Mailbox`<br/><br/><span data-ttu-id="058f3-120">メールボックス要素の他の親要素は、次のように。</span><span class="sxs-lookup"><span data-stu-id="058f3-120">The following are additional parent elements of the Mailbox element:</span></span><br/><br/><span data-ttu-id="058f3-121">- [BccRecipients](bccrecipients.md)</span><span class="sxs-lookup"><span data-stu-id="058f3-121">- [BccRecipients](bccrecipients.md)</span></span> <br/><span data-ttu-id="058f3-122">- [ReplyTo](replyto.md)</span><span class="sxs-lookup"><span data-stu-id="058f3-122">- [ReplyTo](replyto.md)</span></span> <br/><span data-ttu-id="058f3-123">- [送信者](sender.md)</span><span class="sxs-lookup"><span data-stu-id="058f3-123">- [Sender](sender.md)</span></span> <br/><span data-ttu-id="058f3-124">- [差出人](from.md)</span><span class="sxs-lookup"><span data-stu-id="058f3-124">- [From](from.md)</span></span> <br/><span data-ttu-id="058f3-125">- [開催者](organizer.md)</span><span class="sxs-lookup"><span data-stu-id="058f3-125">- [Organizer](organizer.md)</span></span> <br/><span data-ttu-id="058f3-126">- [DistinguishedFolderId](distinguishedfolderid.md)</span><span class="sxs-lookup"><span data-stu-id="058f3-126">- [DistinguishedFolderId](distinguishedfolderid.md)</span></span> <br/><span data-ttu-id="058f3-127">- [解像度](resolution.md)</span><span class="sxs-lookup"><span data-stu-id="058f3-127">- [Resolution](resolution.md)</span></span> <br/><span data-ttu-id="058f3-128">- [DLExpansion](dlexpansion.md)</span><span class="sxs-lookup"><span data-stu-id="058f3-128">- [DLExpansion](dlexpansion.md)</span></span> <br/><span data-ttu-id="058f3-129">- [出席者](attendee.md)</span><span class="sxs-lookup"><span data-stu-id="058f3-129">- [Attendee](attendee.md)</span></span> <br/> |
|[<span data-ttu-id="058f3-130">RoomList</span><span class="sxs-lookup"><span data-stu-id="058f3-130">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="058f3-131">電子メール アドレスを使用して会議室の一覧を識別します。</span><span class="sxs-lookup"><span data-stu-id="058f3-131">Identifies a list of meeting rooms by email address.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="058f3-132">テキスト値</span><span class="sxs-lookup"><span data-stu-id="058f3-132">Text value</span></span>

<span data-ttu-id="058f3-133">SMTP アドレスを表す文字列値は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="058f3-133">A text value that represents an SMTP address is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="058f3-134">備考</span><span class="sxs-lookup"><span data-stu-id="058f3-134">Remarks</span></span>

<span data-ttu-id="058f3-135">**EmailAddress**要素は、SMTP を表すことができますまたは従来の Exchange 識別名 (DN とも呼ばれます) のアドレスです。</span><span class="sxs-lookup"><span data-stu-id="058f3-135">The **EmailAddress** element can represent SMTP or legacy Exchange distinguished name (also known as DN) addresses.</span></span> <span data-ttu-id="058f3-136">**EmailAddress**要素は、唯一の必要な[メールボックス](mailbox.md)の要素です。</span><span class="sxs-lookup"><span data-stu-id="058f3-136">The **EmailAddress** element is the only required [Mailbox](mailbox.md) element.</span></span> 
  
<span data-ttu-id="058f3-137">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="058f3-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="058f3-138">要素情報</span><span class="sxs-lookup"><span data-stu-id="058f3-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="058f3-139">名前空間</span><span class="sxs-lookup"><span data-stu-id="058f3-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="058f3-140">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="058f3-140">Schema Name</span></span>  <br/> |<span data-ttu-id="058f3-141">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="058f3-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="058f3-142">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="058f3-142">Validation File</span></span>  <br/> |<span data-ttu-id="058f3-143">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="058f3-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="058f3-144">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="058f3-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="058f3-145">いいえ</span><span class="sxs-lookup"><span data-stu-id="058f3-145">False</span></span>  <br/> |
   

