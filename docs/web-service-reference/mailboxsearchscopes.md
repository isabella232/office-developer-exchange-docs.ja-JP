---
title: MailboxSearchScopes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8b9a1979-a364-4c8f-b013-4fc04c0eeb9c
description: MailboxSearchScopes 要素は、1 つまたは複数のメールボックスと関連付けられている検索範囲の検索の検索のリストを指定します。
ms.openlocfilehash: 4d65296e181b6e97e2209a9f6accc7fa5f401b5a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/15/2018
ms.locfileid: "19832294"
---
# <a name="mailboxsearchscopes"></a><span data-ttu-id="8b136-103">MailboxSearchScopes</span><span class="sxs-lookup"><span data-stu-id="8b136-103">MailboxSearchScopes</span></span>

<span data-ttu-id="8b136-104">**MailboxSearchScopes**要素は、1 つまたは複数のメールボックスと関連付けられている検索範囲の検索の検索のリストを指定します。</span><span class="sxs-lookup"><span data-stu-id="8b136-104">The **MailboxSearchScopes** element specifies a list of one or more mailboxes and associated search scopes for a discovery search.</span></span> 
  
```XML
<MailboxSearchScopes>
   <MailboxSearchScope/>
<MailboxSearchScope>
```

<span data-ttu-id="8b136-105">**MailboxSearchScopeType**</span><span class="sxs-lookup"><span data-stu-id="8b136-105">**MailboxSearchScopeType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="8b136-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8b136-106">Attributes and elements</span></span>

<span data-ttu-id="8b136-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8b136-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8b136-108">属性</span><span class="sxs-lookup"><span data-stu-id="8b136-108">Attributes</span></span>

<span data-ttu-id="8b136-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8b136-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8b136-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8b136-110">Child elements</span></span>

[<span data-ttu-id="8b136-111">MailboxSearchScope</span><span class="sxs-lookup"><span data-stu-id="8b136-111">MailboxSearchScope</span></span>](mailboxsearchscope.md)
  
### <a name="parent-elements"></a><span data-ttu-id="8b136-112">親要素</span><span class="sxs-lookup"><span data-stu-id="8b136-112">Parent elements</span></span>

[<span data-ttu-id="8b136-113">MailboxQuery</span><span class="sxs-lookup"><span data-stu-id="8b136-113">MailboxQuery</span></span>](mailboxquery.md)
  
## <a name="remarks"></a><span data-ttu-id="8b136-114">Remarks</span><span class="sxs-lookup"><span data-stu-id="8b136-114">Remarks</span></span>

<span data-ttu-id="8b136-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="8b136-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8b136-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="8b136-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8b136-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="8b136-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8b136-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="8b136-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8b136-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8b136-119">Schema name</span></span>  <br/> |<span data-ttu-id="8b136-120">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="8b136-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="8b136-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8b136-121">Validation file</span></span>  <br/> |<span data-ttu-id="8b136-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8b136-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8b136-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="8b136-123">Can be empty</span></span>  <br/> |<span data-ttu-id="8b136-124">false</span><span class="sxs-lookup"><span data-stu-id="8b136-124">false</span></span>  <br/> |
   

