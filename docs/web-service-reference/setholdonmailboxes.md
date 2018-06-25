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
ms.openlocfilehash: 7d226de908c4d5a474129e3e1f2344ec1318f538
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833413"
---
# <a name="setholdonmailboxes"></a><span data-ttu-id="9d03c-103">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="9d03c-103">SetHoldOnMailboxes</span></span>

<span data-ttu-id="9d03c-104">**SetHoldOnMailboxes**要素には、 **SetHoldOnMailboxes**要求が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9d03c-104">The **SetHoldOnMailboxes** element contains a **SetHoldOnMailboxes** request.</span></span> 
  
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

 <span data-ttu-id="9d03c-105">**SetHoldOnMailboxesType**</span><span class="sxs-lookup"><span data-stu-id="9d03c-105">**SetHoldOnMailboxesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9d03c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9d03c-106">Attributes and elements</span></span>

<span data-ttu-id="9d03c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9d03c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9d03c-108">属性</span><span class="sxs-lookup"><span data-stu-id="9d03c-108">Attributes</span></span>

<span data-ttu-id="9d03c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9d03c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9d03c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9d03c-110">Child elements</span></span>

<span data-ttu-id="9d03c-111">[ファイアウォール (HoldActionType)](actiontype-holdactiontype.md) | [HoldId](holdid.md) | [クエリ](query.md) | [メールボックス (ArrayOfStringsType)](mailboxes-arrayofstringstype.md) | [言語](language.md) | [IncludeNonIndexableItems](includenonindexableitems.md) | [の重複除外](deduplication.md)  |  [InPlaceHoldIdentity](inplaceholdidentity.md)</span><span class="sxs-lookup"><span data-stu-id="9d03c-111">[ActionType (HoldActionType)](actiontype-holdactiontype.md) | [HoldId](holdid.md) | [Query](query.md) | [Mailboxes (ArrayOfStringsType)](mailboxes-arrayofstringstype.md) | [Language](language.md) | [IncludeNonIndexableItems](includenonindexableitems.md) | [Deduplication](deduplication.md) | [InPlaceHoldIdentity](inplaceholdidentity.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9d03c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9d03c-112">Parent elements</span></span>

<span data-ttu-id="9d03c-113">なし。</span><span class="sxs-lookup"><span data-stu-id="9d03c-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9d03c-114">備考</span><span class="sxs-lookup"><span data-stu-id="9d03c-114">Remarks</span></span>

<span data-ttu-id="9d03c-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9d03c-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9d03c-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9d03c-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9d03c-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="9d03c-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9d03c-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="9d03c-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9d03c-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9d03c-119">Schema name</span></span>  <br/> |<span data-ttu-id="9d03c-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="9d03c-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9d03c-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9d03c-121">Validation file</span></span>  <br/> |<span data-ttu-id="9d03c-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9d03c-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9d03c-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9d03c-123">Can be empty</span></span>  <br/> ||
   

