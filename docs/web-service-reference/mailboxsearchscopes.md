---
title: MailboxSearchScopes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8b9a1979-a364-4c8f-b013-4fc04c0eeb9c
description: MailboxSearchScopes 要素は、1つ以上のメールボックスのリストと、探索検索用に関連付けられた検索範囲を指定します。
ms.openlocfilehash: 172c9d1da46c8c9a8ac73224b3395a026d9e6551
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530552"
---
# <a name="mailboxsearchscopes"></a><span data-ttu-id="c99a1-103">MailboxSearchScopes</span><span class="sxs-lookup"><span data-stu-id="c99a1-103">MailboxSearchScopes</span></span>

<span data-ttu-id="c99a1-104">**MailboxSearchScopes**要素は、1つ以上のメールボックスのリストと、探索検索用に関連付けられた検索範囲を指定します。</span><span class="sxs-lookup"><span data-stu-id="c99a1-104">The **MailboxSearchScopes** element specifies a list of one or more mailboxes and associated search scopes for a discovery search.</span></span> 
  
```XML
<MailboxSearchScopes>
   <MailboxSearchScope/>
<MailboxSearchScope>
```

<span data-ttu-id="c99a1-105">**MailboxSearchScopeType**</span><span class="sxs-lookup"><span data-stu-id="c99a1-105">**MailboxSearchScopeType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="c99a1-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c99a1-106">Attributes and elements</span></span>

<span data-ttu-id="c99a1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c99a1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c99a1-108">属性</span><span class="sxs-lookup"><span data-stu-id="c99a1-108">Attributes</span></span>

<span data-ttu-id="c99a1-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c99a1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c99a1-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c99a1-110">Child elements</span></span>

[<span data-ttu-id="c99a1-111">MailboxSearchScope</span><span class="sxs-lookup"><span data-stu-id="c99a1-111">MailboxSearchScope</span></span>](mailboxsearchscope.md)
  
### <a name="parent-elements"></a><span data-ttu-id="c99a1-112">親要素</span><span class="sxs-lookup"><span data-stu-id="c99a1-112">Parent elements</span></span>

[<span data-ttu-id="c99a1-113">MailboxQuery</span><span class="sxs-lookup"><span data-stu-id="c99a1-113">MailboxQuery</span></span>](mailboxquery.md)
  
## <a name="remarks"></a><span data-ttu-id="c99a1-114">注釈</span><span class="sxs-lookup"><span data-stu-id="c99a1-114">Remarks</span></span>

<span data-ttu-id="c99a1-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="c99a1-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c99a1-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="c99a1-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c99a1-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c99a1-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c99a1-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="c99a1-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c99a1-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c99a1-119">Schema name</span></span>  <br/> |<span data-ttu-id="c99a1-120">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="c99a1-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="c99a1-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c99a1-121">Validation file</span></span>  <br/> |<span data-ttu-id="c99a1-122">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="c99a1-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c99a1-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c99a1-123">Can be empty</span></span>  <br/> |<span data-ttu-id="c99a1-124">false</span><span class="sxs-lookup"><span data-stu-id="c99a1-124">false</span></span>  <br/> |
   

