---
title: MailboxSearchScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ef4a4203-61e5-46b8-9fa4-d1a10e785aa2
description: MailboxSearchScope 要素は、探索検索のメールボックスと検索範囲を指定します。
ms.openlocfilehash: 20f528ddfb4812de8468af33bcb0b47d7d851f1d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457187"
---
# <a name="mailboxsearchscope"></a><span data-ttu-id="f074d-103">MailboxSearchScope</span><span class="sxs-lookup"><span data-stu-id="f074d-103">MailboxSearchScope</span></span>

<span data-ttu-id="f074d-104">**MailboxSearchScope**要素は、探索検索のメールボックスと検索範囲を指定します。</span><span class="sxs-lookup"><span data-stu-id="f074d-104">The **MailboxSearchScope** element specifies a mailbox and a search scope for a discovery search.</span></span> 
  
```XML
<MailboxSearchScope>
   <Mailbox/>
   <SearchScope/>
<MailboxSearchScope>
```

<span data-ttu-id="f074d-105">**MailboxSearchScopeType**</span><span class="sxs-lookup"><span data-stu-id="f074d-105">**MailboxSearchScopeType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="f074d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f074d-106">Attributes and elements</span></span>

<span data-ttu-id="f074d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f074d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f074d-108">属性</span><span class="sxs-lookup"><span data-stu-id="f074d-108">Attributes</span></span>

<span data-ttu-id="f074d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f074d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f074d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f074d-110">Child elements</span></span>

<span data-ttu-id="f074d-111">[メールボックス (文字列)](mailbox-string.md)  | [Searchscope](searchscope.md)</span><span class="sxs-lookup"><span data-stu-id="f074d-111">[Mailbox (string)](mailbox-string.md) | [SearchScope](searchscope.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f074d-112">親要素</span><span class="sxs-lookup"><span data-stu-id="f074d-112">Parent elements</span></span>

[<span data-ttu-id="f074d-113">MailboxSearchScopes</span><span class="sxs-lookup"><span data-stu-id="f074d-113">MailboxSearchScopes</span></span>](mailboxsearchscopes.md)
  
## <a name="remarks"></a><span data-ttu-id="f074d-114">注釈</span><span class="sxs-lookup"><span data-stu-id="f074d-114">Remarks</span></span>

<span data-ttu-id="f074d-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f074d-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f074d-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f074d-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f074d-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f074d-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f074d-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="f074d-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f074d-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f074d-119">Schema name</span></span>  <br/> |<span data-ttu-id="f074d-120">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="f074d-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="f074d-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f074d-121">Validation file</span></span>  <br/> |<span data-ttu-id="f074d-122">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="f074d-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f074d-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f074d-123">Can be empty</span></span>  <br/> ||
   

