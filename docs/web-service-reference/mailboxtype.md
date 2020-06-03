---
title: MailboxType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailboxType
api_type:
- schema
ms.assetid: 696e5fdb-d8c5-40f0-9e79-885eae65dfa4
description: MailboxType 要素は、電子メールアドレスによって表されるメールボックスの種類を表します。
ms.openlocfilehash: 8c322ab8a87730832f5d199698a369656b058a9a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459799"
---
# <a name="mailboxtype"></a><span data-ttu-id="6422c-103">MailboxType</span><span class="sxs-lookup"><span data-stu-id="6422c-103">MailboxType</span></span>

<span data-ttu-id="6422c-104">**MailboxType**要素は、電子メールアドレスによって表されるメールボックスの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="6422c-104">The **MailboxType** element represents the type of mailbox that is represented by the e-mail address.</span></span> 
  
```XML
<MailboxType>Mailbox | PublicDL | PrivateDL | Contact | PublicFolder | Unknown | OneOff | GroupMailbox</MailboxType>
```

<span data-ttu-id="6422c-105">**MailboxTypeType**</span><span class="sxs-lookup"><span data-stu-id="6422c-105">**MailboxTypeType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="6422c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6422c-106">Attributes and elements</span></span>

<span data-ttu-id="6422c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6422c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6422c-108">属性</span><span class="sxs-lookup"><span data-stu-id="6422c-108">Attributes</span></span>

<span data-ttu-id="6422c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6422c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6422c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6422c-110">Child elements</span></span>

<span data-ttu-id="6422c-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6422c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6422c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6422c-112">Parent elements</span></span>

|<span data-ttu-id="6422c-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="6422c-113">**Element**</span></span>|<span data-ttu-id="6422c-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="6422c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6422c-115">メールボックス</span><span class="sxs-lookup"><span data-stu-id="6422c-115">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="6422c-116">完全に解決された電子メールアドレスを識別します。</span><span class="sxs-lookup"><span data-stu-id="6422c-116">Identifies a fully resolved e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="6422c-117">RoomList</span><span class="sxs-lookup"><span data-stu-id="6422c-117">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="6422c-118">会議室のリストを識別します。</span><span class="sxs-lookup"><span data-stu-id="6422c-118">Identifies a list of meeting rooms.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6422c-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6422c-119">Text value</span></span>

<span data-ttu-id="6422c-120">次の表に、 **MailboxType**要素に指定できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="6422c-120">The following table lists the possible values for the **MailboxType** element.</span></span> 
  
|<span data-ttu-id="6422c-121">**値**</span><span class="sxs-lookup"><span data-stu-id="6422c-121">**Value**</span></span>|<span data-ttu-id="6422c-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="6422c-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6422c-123">メールボックス</span><span class="sxs-lookup"><span data-stu-id="6422c-123">Mailbox</span></span>  <br/> |<span data-ttu-id="6422c-124">メールが有効な Active Directory オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="6422c-124">Represents a mail-enabled Active Directory object.</span></span>  <br/> |
|<span data-ttu-id="6422c-125">PublicDL</span><span class="sxs-lookup"><span data-stu-id="6422c-125">PublicDL</span></span>  <br/> |<span data-ttu-id="6422c-126">パブリック配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="6422c-126">Represents a public distribution list.</span></span>  <br/> |
|<span data-ttu-id="6422c-127">PrivateDL</span><span class="sxs-lookup"><span data-stu-id="6422c-127">PrivateDL</span></span>  <br/> |<span data-ttu-id="6422c-128">ユーザーのメールボックス内のプライベート配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="6422c-128">Represents a private distribution list in a user's mailbox.</span></span>  <br/> |
|<span data-ttu-id="6422c-129">Contact</span><span class="sxs-lookup"><span data-stu-id="6422c-129">Contact</span></span>  <br/> |<span data-ttu-id="6422c-130">ユーザーのメールボックス内の連絡先を表します。</span><span class="sxs-lookup"><span data-stu-id="6422c-130">Represents a contact in a user's mailbox.</span></span>  <br/> |
|<span data-ttu-id="6422c-131">New-publicfolder</span><span class="sxs-lookup"><span data-stu-id="6422c-131">PublicFolder</span></span>  <br/> |<span data-ttu-id="6422c-132">パブリックフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="6422c-132">Represents a public folder.</span></span>  <br/> |
|<span data-ttu-id="6422c-133">不明</span><span class="sxs-lookup"><span data-stu-id="6422c-133">Unknown</span></span>  <br/> |<span data-ttu-id="6422c-134">不明な種類のメールボックスを表します。</span><span class="sxs-lookup"><span data-stu-id="6422c-134">Represents an unknown type of mailbox.</span></span>  <br/> |
|<span data-ttu-id="6422c-135">OneOff</span><span class="sxs-lookup"><span data-stu-id="6422c-135">OneOff</span></span>  <br/> |<span data-ttu-id="6422c-136">個人用配布リストの1回限りのメンバーを表します。</span><span class="sxs-lookup"><span data-stu-id="6422c-136">Represents a one-off member of a personal distribution list.</span></span>  <br/> |
|<span data-ttu-id="6422c-137">GroupMailbox</span><span class="sxs-lookup"><span data-stu-id="6422c-137">GroupMailbox</span></span>  <br/> |<span data-ttu-id="6422c-138">グループメールボックスを表します。</span><span class="sxs-lookup"><span data-stu-id="6422c-138">Represents a group mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6422c-139">注釈</span><span class="sxs-lookup"><span data-stu-id="6422c-139">Remarks</span></span>

<span data-ttu-id="6422c-140">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6422c-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6422c-141">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6422c-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6422c-142">Namespace</span><span class="sxs-lookup"><span data-stu-id="6422c-142">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6422c-143">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6422c-143">Schema Name</span></span>  <br/> |<span data-ttu-id="6422c-144">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="6422c-144">Types schema</span></span>  <br/> |
|<span data-ttu-id="6422c-145">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6422c-145">Validation File</span></span>  <br/> |<span data-ttu-id="6422c-146">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="6422c-146">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6422c-147">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6422c-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="6422c-148">正しくない</span><span class="sxs-lookup"><span data-stu-id="6422c-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6422c-149">関連項目</span><span class="sxs-lookup"><span data-stu-id="6422c-149">See also</span></span>

- [<span data-ttu-id="6422c-150">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="6422c-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

