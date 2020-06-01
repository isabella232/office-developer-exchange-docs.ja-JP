---
title: MailboxHoldStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 92608b77-8aa4-403b-a4de-01e3a60af3e0
description: MailboxHoldStatus 要素は、メールボックスの保留状態を指定します。
ms.openlocfilehash: 2ac575275fc00d2e3ba38cb4ec7335567ee82da6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468811"
---
# <a name="mailboxholdstatus"></a><span data-ttu-id="9f57c-103">MailboxHoldStatus</span><span class="sxs-lookup"><span data-stu-id="9f57c-103">MailboxHoldStatus</span></span>

<span data-ttu-id="9f57c-104">**MailboxHoldStatus**要素は、メールボックスの保留状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="9f57c-104">The **MailboxHoldStatus** element specifies the hold status of the mailbox.</span></span> 
  
```XML
<MailboxHoldStatus>
   <Mailbox/>
   <Status/>
   <AdditionalInfo/>
</MailboxHoldStatus>
```

<span data-ttu-id="9f57c-105">**MailboxHoldStatusType**</span><span class="sxs-lookup"><span data-stu-id="9f57c-105">**MailboxHoldStatusType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="9f57c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9f57c-106">Attributes and elements</span></span>

<span data-ttu-id="9f57c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9f57c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9f57c-108">属性</span><span class="sxs-lookup"><span data-stu-id="9f57c-108">Attributes</span></span>

<span data-ttu-id="9f57c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9f57c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9f57c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9f57c-110">Child elements</span></span>

<span data-ttu-id="9f57c-111">[メールボックス (文字列)](mailbox-string.md)  | [状態 (HoldStatusType)](status-holdstatustype.md)  | [Additionalinfo](additionalinfo.md)</span><span class="sxs-lookup"><span data-stu-id="9f57c-111">[Mailbox (string)](mailbox-string.md) | [Status (HoldStatusType)](status-holdstatustype.md) | [AdditionalInfo](additionalinfo.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9f57c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9f57c-112">Parent elements</span></span>

[<span data-ttu-id="9f57c-113">MailboxHoldStatuses</span><span class="sxs-lookup"><span data-stu-id="9f57c-113">MailboxHoldStatuses</span></span>](mailboxholdstatuses.md)
  
## <a name="remarks"></a><span data-ttu-id="9f57c-114">注釈</span><span class="sxs-lookup"><span data-stu-id="9f57c-114">Remarks</span></span>

<span data-ttu-id="9f57c-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9f57c-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9f57c-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9f57c-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9f57c-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9f57c-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9f57c-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="9f57c-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9f57c-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9f57c-119">Schema name</span></span>  <br/> |<span data-ttu-id="9f57c-120">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="9f57c-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="9f57c-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9f57c-121">Validation file</span></span>  <br/> |<span data-ttu-id="9f57c-122">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="9f57c-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9f57c-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9f57c-123">Can be empty</span></span>  <br/> ||
   

