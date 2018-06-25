---
title: MailboxSearchScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ef4a4203-61e5-46b8-9fa4-d1a10e785aa2
description: MailboxSearchScope 要素は、メールボックスの検出検索用の検索範囲を指定します。
ms.openlocfilehash: 657e6dfd4eb6c6c0eabb18546e7090c524e28e5e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832297"
---
# <a name="mailboxsearchscope"></a><span data-ttu-id="78041-103">MailboxSearchScope</span><span class="sxs-lookup"><span data-stu-id="78041-103">MailboxSearchScope</span></span>

<span data-ttu-id="78041-104">**MailboxSearchScope**要素は、メールボックスの検出検索用の検索範囲を指定します。</span><span class="sxs-lookup"><span data-stu-id="78041-104">The **MailboxSearchScope** element specifies a mailbox and a search scope for a discovery search.</span></span> 
  
```XML
<MailboxSearchScope>
   <Mailbox/>
   <SearchScope/>
<MailboxSearchScope>
```

<span data-ttu-id="78041-105">**MailboxSearchScopeType**</span><span class="sxs-lookup"><span data-stu-id="78041-105">**MailboxSearchScopeType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="78041-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="78041-106">Attributes and elements</span></span>

<span data-ttu-id="78041-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="78041-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="78041-108">属性</span><span class="sxs-lookup"><span data-stu-id="78041-108">Attributes</span></span>

<span data-ttu-id="78041-109">なし。</span><span class="sxs-lookup"><span data-stu-id="78041-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="78041-110">子要素</span><span class="sxs-lookup"><span data-stu-id="78041-110">Child elements</span></span>

<span data-ttu-id="78041-111">[メールボックス (文字列)](mailbox-string.md) | [SearchScope](searchscope.md)</span><span class="sxs-lookup"><span data-stu-id="78041-111">[Mailbox (string)](mailbox-string.md) | [SearchScope](searchscope.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="78041-112">親要素</span><span class="sxs-lookup"><span data-stu-id="78041-112">Parent elements</span></span>

[<span data-ttu-id="78041-113">MailboxSearchScopes</span><span class="sxs-lookup"><span data-stu-id="78041-113">MailboxSearchScopes</span></span>](mailboxsearchscopes.md)
  
## <a name="remarks"></a><span data-ttu-id="78041-114">備考</span><span class="sxs-lookup"><span data-stu-id="78041-114">Remarks</span></span>

<span data-ttu-id="78041-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="78041-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="78041-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="78041-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="78041-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="78041-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="78041-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="78041-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="78041-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="78041-119">Schema name</span></span>  <br/> |<span data-ttu-id="78041-120">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="78041-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="78041-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="78041-121">Validation file</span></span>  <br/> |<span data-ttu-id="78041-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="78041-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="78041-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="78041-123">Can be empty</span></span>  <br/> ||
   

