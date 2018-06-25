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
ms.openlocfilehash: 6703c909d0a7b4e83e190807fc3202ecd4699e7f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832288"
---
# <a name="mailboxholdstatus"></a><span data-ttu-id="c9adb-103">MailboxHoldStatus</span><span class="sxs-lookup"><span data-stu-id="c9adb-103">MailboxHoldStatus</span></span>

<span data-ttu-id="c9adb-104">**MailboxHoldStatus**要素は、メールボックスの保留状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="c9adb-104">The **MailboxHoldStatus** element specifies the hold status of the mailbox.</span></span> 
  
```XML
<MailboxHoldStatus>
   <Mailbox/>
   <Status/>
   <AdditionalInfo/>
</MailboxHoldStatus>
```

<span data-ttu-id="c9adb-105">**MailboxHoldStatusType**</span><span class="sxs-lookup"><span data-stu-id="c9adb-105">**MailboxHoldStatusType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="c9adb-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="c9adb-106">Attributes and elements</span></span>

<span data-ttu-id="c9adb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c9adb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c9adb-108">属性</span><span class="sxs-lookup"><span data-stu-id="c9adb-108">Attributes</span></span>

<span data-ttu-id="c9adb-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c9adb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c9adb-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c9adb-110">Child elements</span></span>

<span data-ttu-id="c9adb-111">[メールボックス (文字列)](mailbox-string.md) | [状態 (HoldStatusType)](status-holdstatustype.md) | [AdditionalInfo](additionalinfo.md)</span><span class="sxs-lookup"><span data-stu-id="c9adb-111">[Mailbox (string)](mailbox-string.md) | [Status (HoldStatusType)](status-holdstatustype.md) | [AdditionalInfo](additionalinfo.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c9adb-112">親要素</span><span class="sxs-lookup"><span data-stu-id="c9adb-112">Parent elements</span></span>

[<span data-ttu-id="c9adb-113">MailboxHoldStatuses</span><span class="sxs-lookup"><span data-stu-id="c9adb-113">MailboxHoldStatuses</span></span>](mailboxholdstatuses.md)
  
## <a name="remarks"></a><span data-ttu-id="c9adb-114">備考</span><span class="sxs-lookup"><span data-stu-id="c9adb-114">Remarks</span></span>

<span data-ttu-id="c9adb-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="c9adb-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c9adb-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="c9adb-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c9adb-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="c9adb-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c9adb-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="c9adb-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c9adb-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c9adb-119">Schema name</span></span>  <br/> |<span data-ttu-id="c9adb-120">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="c9adb-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="c9adb-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c9adb-121">Validation file</span></span>  <br/> |<span data-ttu-id="c9adb-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c9adb-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c9adb-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c9adb-123">Can be empty</span></span>  <br/> ||
   

