---
title: UserMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1d47141c-3c3f-45b8-90c5-33a44adb34b2
description: UserMailbox 要素は、ユーザーメールボックスを識別します。
ms.openlocfilehash: 9bb1b08320f5e6f4843383a8e3aff96fc3dcccad
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465318"
---
# <a name="usermailbox"></a><span data-ttu-id="15ca5-103">UserMailbox</span><span class="sxs-lookup"><span data-stu-id="15ca5-103">UserMailbox</span></span>

<span data-ttu-id="15ca5-104">**Usermailbox**要素は、ユーザーメールボックスを識別します。</span><span class="sxs-lookup"><span data-stu-id="15ca5-104">The **UserMailbox** element identifies a user mailbox.</span></span> 
  
```XML
<UserMailbox Id="" IsArchive=""/>
```

 <span data-ttu-id="15ca5-105">**UserMailboxType**</span><span class="sxs-lookup"><span data-stu-id="15ca5-105">**UserMailboxType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="15ca5-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="15ca5-106">Attributes and elements</span></span>

<span data-ttu-id="15ca5-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="15ca5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="15ca5-108">属性</span><span class="sxs-lookup"><span data-stu-id="15ca5-108">Attributes</span></span>

|<span data-ttu-id="15ca5-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="15ca5-109">**Attribute**</span></span>|<span data-ttu-id="15ca5-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="15ca5-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="15ca5-111">ID</span><span class="sxs-lookup"><span data-stu-id="15ca5-111">Id</span></span>  <br/> |<span data-ttu-id="15ca5-112">**Id**属性のテキスト値は、メールボックスの識別子です。</span><span class="sxs-lookup"><span data-stu-id="15ca5-112">The text value of the **Id** attribute is the identifier of the mailbox.</span></span>  <br/> |
|<span data-ttu-id="15ca5-113">IsArchive</span><span class="sxs-lookup"><span data-stu-id="15ca5-113">IsArchive</span></span>  <br/> |<span data-ttu-id="15ca5-114">**Isarchive**属性のテキスト値は、メールボックスがアーカイブメールボックスであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="15ca5-114">The text value of the **IsArchive** attribute indicates whether the mailbox is an archive mailbox.</span></span> <span data-ttu-id="15ca5-115">**Isarchive**属性のテキスト値が**true の場合**は、メールボックスがアーカイブメールボックスであることを示します。</span><span class="sxs-lookup"><span data-stu-id="15ca5-115">A text value of **true** for the **IsArchive** attribute indicates that the mailbox is an archive mailbox.</span></span> <span data-ttu-id="15ca5-116">**Isarchive**属性の値が**false**の場合は、メールボックスがプライマリメールボックスであることを示します。</span><span class="sxs-lookup"><span data-stu-id="15ca5-116">A value of **false** for the **IsArchive** attribute indicates that the mailbox is a primary mailbox.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="15ca5-117">子要素</span><span class="sxs-lookup"><span data-stu-id="15ca5-117">Child elements</span></span>

<span data-ttu-id="15ca5-118">なし。</span><span class="sxs-lookup"><span data-stu-id="15ca5-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="15ca5-119">親要素</span><span class="sxs-lookup"><span data-stu-id="15ca5-119">Parent elements</span></span>

<span data-ttu-id="15ca5-120">[メールボックス (ArrayOfUserMailboxesType)](mailboxes-arrayofusermailboxestype.md)  | [MailboxStatisticsSearchResult](mailboxstatisticssearchresult.md)</span><span class="sxs-lookup"><span data-stu-id="15ca5-120">[Mailboxes (ArrayOfUserMailboxesType)](mailboxes-arrayofusermailboxestype.md) | [MailboxStatisticsSearchResult](mailboxstatisticssearchresult.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="15ca5-121">注釈</span><span class="sxs-lookup"><span data-stu-id="15ca5-121">Remarks</span></span>

<span data-ttu-id="15ca5-122">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="15ca5-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="15ca5-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="15ca5-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="15ca5-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="15ca5-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="15ca5-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="15ca5-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="15ca5-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="15ca5-126">Schema name</span></span>  <br/> |<span data-ttu-id="15ca5-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="15ca5-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="15ca5-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="15ca5-128">Validation file</span></span>  <br/> |<span data-ttu-id="15ca5-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="15ca5-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="15ca5-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="15ca5-130">Can be empty</span></span>  <br/> |<span data-ttu-id="15ca5-131">true</span><span class="sxs-lookup"><span data-stu-id="15ca5-131">true</span></span>  <br/> |
   

