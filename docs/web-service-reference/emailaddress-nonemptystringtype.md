---
title: EmailAddress (非 Emptystringtype)
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
description: EmailAddress 要素は、メールボックスユーザーのプライマリ SMTP アドレスを定義します。
ms.openlocfilehash: fcc3e650d5fc32344022ed6f015d4096a4461f63
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463133"
---
# <a name="emailaddress-nonemptystringtype"></a><span data-ttu-id="0a222-103">EmailAddress (非 Emptystringtype)</span><span class="sxs-lookup"><span data-stu-id="0a222-103">EmailAddress (NonEmptyStringType)</span></span>

<span data-ttu-id="0a222-104">**EmailAddress**要素は、メールボックスユーザーのプライマリ SMTP アドレスを定義します。</span><span class="sxs-lookup"><span data-stu-id="0a222-104">The **EmailAddress** element defines the primary SMTP address of a mailbox user.</span></span> 
  
```XML
<EmailAddress/>
```

 <span data-ttu-id="0a222-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="0a222-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0a222-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0a222-106">Attributes and elements</span></span>

<span data-ttu-id="0a222-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0a222-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0a222-108">属性</span><span class="sxs-lookup"><span data-stu-id="0a222-108">Attributes</span></span>

<span data-ttu-id="0a222-109">なし。</span><span class="sxs-lookup"><span data-stu-id="0a222-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0a222-110">子要素</span><span class="sxs-lookup"><span data-stu-id="0a222-110">Child elements</span></span>

<span data-ttu-id="0a222-111">なし。</span><span class="sxs-lookup"><span data-stu-id="0a222-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0a222-112">親要素</span><span class="sxs-lookup"><span data-stu-id="0a222-112">Parent elements</span></span>

|<span data-ttu-id="0a222-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="0a222-113">**Element**</span></span>|<span data-ttu-id="0a222-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="0a222-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0a222-115">ActingAs</span><span class="sxs-lookup"><span data-stu-id="0a222-115">ActingAs</span></span>](actingas.md) <br/> |<span data-ttu-id="0a222-116">発信者が送信者として送信しているユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="0a222-116">Identifies who the caller is sending as.</span></span>  <br/> |
|[<span data-ttu-id="0a222-117">メールボックス</span><span class="sxs-lookup"><span data-stu-id="0a222-117">Mailbox</span></span>](mailbox.md) <br/> | <span data-ttu-id="0a222-118">完全に解決された電子メールアドレスを識別します。</span><span class="sxs-lookup"><span data-stu-id="0a222-118">Identifies a fully resolved e-mail address.</span></span>  <br/><br/><span data-ttu-id="0a222-119">この要素のいくつかの XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0a222-119">The following are some XPath expressions to this element:</span></span><br/><br/>`/CreateItem/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`/CreateFolder/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`CreateItem/Items/AcceptItem/ToRecipients/Mailbox`<br/><br/>`SyncFolderItemsResponseMessage/Changes/Create/CalendarItem/ConflictingMeetings/AcceptItem/CcRecipients/Mailbox`<br/><br/><span data-ttu-id="0a222-120">Mailbox 要素の追加の親要素は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="0a222-120">The following are additional parent elements of the Mailbox element:</span></span><br/><br/><span data-ttu-id="0a222-121">- [BccRecipients](bccrecipients.md)</span><span class="sxs-lookup"><span data-stu-id="0a222-121">- [BccRecipients](bccrecipients.md)</span></span> <br/><span data-ttu-id="0a222-122">- [ReplyTo](replyto.md)</span><span class="sxs-lookup"><span data-stu-id="0a222-122">- [ReplyTo](replyto.md)</span></span> <br/><span data-ttu-id="0a222-123">- [者](sender.md)</span><span class="sxs-lookup"><span data-stu-id="0a222-123">- [Sender](sender.md)</span></span> <br/><span data-ttu-id="0a222-124">- [差出人](from.md)</span><span class="sxs-lookup"><span data-stu-id="0a222-124">- [From](from.md)</span></span> <br/><span data-ttu-id="0a222-125">- [者](organizer.md)</span><span class="sxs-lookup"><span data-stu-id="0a222-125">- [Organizer](organizer.md)</span></span> <br/><span data-ttu-id="0a222-126">- [DistinguishedFolderId](distinguishedfolderid.md)</span><span class="sxs-lookup"><span data-stu-id="0a222-126">- [DistinguishedFolderId](distinguishedfolderid.md)</span></span> <br/><span data-ttu-id="0a222-127">- [画質](resolution.md)</span><span class="sxs-lookup"><span data-stu-id="0a222-127">- [Resolution](resolution.md)</span></span> <br/><span data-ttu-id="0a222-128">- [DLExpansion 展開](dlexpansion.md)</span><span class="sxs-lookup"><span data-stu-id="0a222-128">- [DLExpansion](dlexpansion.md)</span></span> <br/><span data-ttu-id="0a222-129">- [出席](attendee.md)</span><span class="sxs-lookup"><span data-stu-id="0a222-129">- [Attendee](attendee.md)</span></span> <br/> |
|[<span data-ttu-id="0a222-130">RoomList</span><span class="sxs-lookup"><span data-stu-id="0a222-130">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="0a222-131">メールアドレスによって会議室のリストを識別します。</span><span class="sxs-lookup"><span data-stu-id="0a222-131">Identifies a list of meeting rooms by email address.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0a222-132">テキスト値</span><span class="sxs-lookup"><span data-stu-id="0a222-132">Text value</span></span>

<span data-ttu-id="0a222-133">SMTP アドレスを表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="0a222-133">A text value that represents an SMTP address is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0a222-134">注釈</span><span class="sxs-lookup"><span data-stu-id="0a222-134">Remarks</span></span>

<span data-ttu-id="0a222-135">**EmailAddress**要素は、SMTP または従来の Exchange 識別名 (DN) アドレスを表すことができます。</span><span class="sxs-lookup"><span data-stu-id="0a222-135">The **EmailAddress** element can represent SMTP or legacy Exchange distinguished name (also known as DN) addresses.</span></span> <span data-ttu-id="0a222-136">**EmailAddress**要素は、唯一必要な[Mailbox](mailbox.md)要素です。</span><span class="sxs-lookup"><span data-stu-id="0a222-136">The **EmailAddress** element is the only required [Mailbox](mailbox.md) element.</span></span> 
  
<span data-ttu-id="0a222-137">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="0a222-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0a222-138">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0a222-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0a222-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="0a222-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0a222-140">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0a222-140">Schema Name</span></span>  <br/> |<span data-ttu-id="0a222-141">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="0a222-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="0a222-142">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0a222-142">Validation File</span></span>  <br/> |<span data-ttu-id="0a222-143">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="0a222-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0a222-144">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0a222-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="0a222-145">いいえ</span><span class="sxs-lookup"><span data-stu-id="0a222-145">False</span></span>  <br/> |
   

