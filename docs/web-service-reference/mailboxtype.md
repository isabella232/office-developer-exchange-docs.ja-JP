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
description: MailboxType 要素は、電子メール アドレスで表されるメールボックスの種類を表します。
ms.openlocfilehash: d7232377951e8d9c8f191ac856058bc28467cadd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832305"
---
# <a name="mailboxtype"></a><span data-ttu-id="a79e3-103">MailboxType</span><span class="sxs-lookup"><span data-stu-id="a79e3-103">MailboxType</span></span>

<span data-ttu-id="a79e3-104">**MailboxType**要素は、電子メール アドレスで表されるメールボックスの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="a79e3-104">The **MailboxType** element represents the type of mailbox that is represented by the e-mail address.</span></span> 
  
```XML
<MailboxType>Mailbox | PublicDL | PrivateDL | Contact | PublicFolder | Unknown | OneOff | GroupMailbox</MailboxType>
```

<span data-ttu-id="a79e3-105">**MailboxTypeType**</span><span class="sxs-lookup"><span data-stu-id="a79e3-105">**MailboxTypeType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a79e3-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a79e3-106">Attributes and elements</span></span>

<span data-ttu-id="a79e3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a79e3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a79e3-108">属性</span><span class="sxs-lookup"><span data-stu-id="a79e3-108">Attributes</span></span>

<span data-ttu-id="a79e3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a79e3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a79e3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a79e3-110">Child elements</span></span>

<span data-ttu-id="a79e3-111">なし。</span><span class="sxs-lookup"><span data-stu-id="a79e3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a79e3-112">親要素</span><span class="sxs-lookup"><span data-stu-id="a79e3-112">Parent elements</span></span>

|<span data-ttu-id="a79e3-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="a79e3-113">**Element**</span></span>|<span data-ttu-id="a79e3-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="a79e3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a79e3-115">メールボックス</span><span class="sxs-lookup"><span data-stu-id="a79e3-115">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="a79e3-116">完全に解決された電子メール アドレスを識別します。</span><span class="sxs-lookup"><span data-stu-id="a79e3-116">Identifies a fully resolved e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="a79e3-117">RoomList</span><span class="sxs-lookup"><span data-stu-id="a79e3-117">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="a79e3-118">会議室の一覧を識別します。</span><span class="sxs-lookup"><span data-stu-id="a79e3-118">Identifies a list of meeting rooms.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a79e3-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a79e3-119">Text value</span></span>

<span data-ttu-id="a79e3-120">次の表は、 **MailboxType**要素の値を一覧します。</span><span class="sxs-lookup"><span data-stu-id="a79e3-120">The following table lists the possible values for the **MailboxType** element.</span></span> 
  
|<span data-ttu-id="a79e3-121">**値**</span><span class="sxs-lookup"><span data-stu-id="a79e3-121">**Value**</span></span>|<span data-ttu-id="a79e3-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="a79e3-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a79e3-123">メールボックス</span><span class="sxs-lookup"><span data-stu-id="a79e3-123">Mailbox</span></span>  <br/> |<span data-ttu-id="a79e3-124">メールが有効な Active Directory オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="a79e3-124">Represents a mail-enabled Active Directory object.</span></span>  <br/> |
|<span data-ttu-id="a79e3-125">PublicDL</span><span class="sxs-lookup"><span data-stu-id="a79e3-125">PublicDL</span></span>  <br/> |<span data-ttu-id="a79e3-126">パブリックな配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="a79e3-126">Represents a public distribution list.</span></span>  <br/> |
|<span data-ttu-id="a79e3-127">PrivateDL</span><span class="sxs-lookup"><span data-stu-id="a79e3-127">PrivateDL</span></span>  <br/> |<span data-ttu-id="a79e3-128">ユーザーのメールボックス内の個人用配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="a79e3-128">Represents a private distribution list in a user's mailbox.</span></span>  <br/> |
|<span data-ttu-id="a79e3-129">連絡先</span><span class="sxs-lookup"><span data-stu-id="a79e3-129">Contact</span></span>  <br/> |<span data-ttu-id="a79e3-130">ユーザーのメールボックス内の連絡先を表します。</span><span class="sxs-lookup"><span data-stu-id="a79e3-130">Represents a contact in a user's mailbox.</span></span>  <br/> |
|<span data-ttu-id="a79e3-131">パブリック フォルダー</span><span class="sxs-lookup"><span data-stu-id="a79e3-131">PublicFolder</span></span>  <br/> |<span data-ttu-id="a79e3-132">パブリック フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="a79e3-132">Represents a public folder.</span></span>  <br/> |
|<span data-ttu-id="a79e3-133">Unknown</span><span class="sxs-lookup"><span data-stu-id="a79e3-133">Unknown</span></span>  <br/> |<span data-ttu-id="a79e3-134">メールボックスの不明な型を表します。</span><span class="sxs-lookup"><span data-stu-id="a79e3-134">Represents an unknown type of mailbox.</span></span>  <br/> |
|<span data-ttu-id="a79e3-135">OneOff</span><span class="sxs-lookup"><span data-stu-id="a79e3-135">OneOff</span></span>  <br/> |<span data-ttu-id="a79e3-136">個人用配布リストの 1 回限りのメンバーを表します。</span><span class="sxs-lookup"><span data-stu-id="a79e3-136">Represents a one-off member of a personal distribution list.</span></span>  <br/> |
|<span data-ttu-id="a79e3-137">GroupMailbox</span><span class="sxs-lookup"><span data-stu-id="a79e3-137">GroupMailbox</span></span>  <br/> |<span data-ttu-id="a79e3-138">グループのメールボックスを表します。</span><span class="sxs-lookup"><span data-stu-id="a79e3-138">Represents a group mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a79e3-139">備考</span><span class="sxs-lookup"><span data-stu-id="a79e3-139">Remarks</span></span>

<span data-ttu-id="a79e3-140">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a79e3-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a79e3-141">要素情報</span><span class="sxs-lookup"><span data-stu-id="a79e3-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a79e3-142">名前空間</span><span class="sxs-lookup"><span data-stu-id="a79e3-142">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a79e3-143">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a79e3-143">Schema Name</span></span>  <br/> |<span data-ttu-id="a79e3-144">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="a79e3-144">Types schema</span></span>  <br/> |
|<span data-ttu-id="a79e3-145">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a79e3-145">Validation File</span></span>  <br/> |<span data-ttu-id="a79e3-146">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a79e3-146">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a79e3-147">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a79e3-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="a79e3-148">False</span><span class="sxs-lookup"><span data-stu-id="a79e3-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a79e3-149">関連項目</span><span class="sxs-lookup"><span data-stu-id="a79e3-149">See also</span></span>

- [<span data-ttu-id="a79e3-150">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="a79e3-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

