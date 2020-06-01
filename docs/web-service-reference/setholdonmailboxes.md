---
title: SetHoldOnMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fd5b9f0e-23e8-428c-8168-2d6b4ecd6beb
description: SetHoldOnMailboxes 要素には、SetHoldOnMailboxes 要求が含まれています。
ms.openlocfilehash: c96ff50cb1204d86abc66829e1c5da7124f407f1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44448353"
---
# <a name="setholdonmailboxes"></a><span data-ttu-id="2573a-103">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="2573a-103">SetHoldOnMailboxes</span></span>

<span data-ttu-id="2573a-104">**SetHoldOnMailboxes**要素には、 **SetHoldOnMailboxes**要求が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2573a-104">The **SetHoldOnMailboxes** element contains a **SetHoldOnMailboxes** request.</span></span> 
  
```XML
<SetHoldOnMailboxes>
   <ActionType/>
   <HoldId/>
   <Query/>
   <Mailboxes/>
   <Language/>
   <IncludeNonIndexableItems/>
   <Deduplication/>
   <InPlaceHoldIdentity/>
</SetHoldOnMailboxes>
```

 <span data-ttu-id="2573a-105">**SetHoldOnMailboxesType**</span><span class="sxs-lookup"><span data-stu-id="2573a-105">**SetHoldOnMailboxesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2573a-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="2573a-106">Attributes and elements</span></span>

<span data-ttu-id="2573a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2573a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2573a-108">属性</span><span class="sxs-lookup"><span data-stu-id="2573a-108">Attributes</span></span>

<span data-ttu-id="2573a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2573a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2573a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2573a-110">Child elements</span></span>

<span data-ttu-id="2573a-111">[ActionType (HoldActionType)](actiontype-holdactiontype.md)  | [HoldId](holdid.md)  | [クエリ](query.md)  | [メールボックス (ArrayOfStringsType)](mailboxes-arrayofstringstype.md)  | [言語](language.md)  | 追加[アイテム](includenonindexableitems.md)  | [重複除去](deduplication.md)  | [InPlaceHoldIdentity](inplaceholdidentity.md)</span><span class="sxs-lookup"><span data-stu-id="2573a-111">[ActionType (HoldActionType)](actiontype-holdactiontype.md) | [HoldId](holdid.md) | [Query](query.md) | [Mailboxes (ArrayOfStringsType)](mailboxes-arrayofstringstype.md) | [Language](language.md) | [IncludeNonIndexableItems](includenonindexableitems.md) | [Deduplication](deduplication.md) | [InPlaceHoldIdentity](inplaceholdidentity.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2573a-112">親要素</span><span class="sxs-lookup"><span data-stu-id="2573a-112">Parent elements</span></span>

<span data-ttu-id="2573a-113">なし。</span><span class="sxs-lookup"><span data-stu-id="2573a-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2573a-114">注釈</span><span class="sxs-lookup"><span data-stu-id="2573a-114">Remarks</span></span>

<span data-ttu-id="2573a-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="2573a-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2573a-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2573a-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2573a-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="2573a-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2573a-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="2573a-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2573a-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2573a-119">Schema name</span></span>  <br/> |<span data-ttu-id="2573a-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="2573a-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2573a-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2573a-121">Validation file</span></span>  <br/> |<span data-ttu-id="2573a-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="2573a-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2573a-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2573a-123">Can be empty</span></span>  <br/> ||
   

