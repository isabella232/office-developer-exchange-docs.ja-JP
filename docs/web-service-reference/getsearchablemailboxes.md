---
title: GetSearchableMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 949871f7-0d10-498e-84aa-f0652f1193be
description: GetSearchableMailboxes 要素には、クライアントが、電子的証拠開示検索を実行する権限を持っているメールボックスの一覧を取得する要求が含まれています。
ms.openlocfilehash: 8cce18bb62d3840cb9883d20a380cc4f2193303e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760848"
---
# <a name="getsearchablemailboxes"></a><span data-ttu-id="1fc6a-103">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="1fc6a-103">GetSearchableMailboxes</span></span>

<span data-ttu-id="1fc6a-104">**GetSearchableMailboxes**要素には、クライアントが、電子的証拠開示検索を実行する権限を持っているメールボックスの一覧を取得する要求が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1fc6a-104">The **GetSearchableMailboxes** element contains a request to get a list of mailboxes that the client has permission to perform an eDiscovery search.</span></span> 
  
```XML
<GetSearchableMailboxes>
   <SearchFilter/>
   <ExpandGroupMembership/>
</GetSearchableMailboxes>
```

 <span data-ttu-id="1fc6a-105">**GetSearchableMailboxesType**</span><span class="sxs-lookup"><span data-stu-id="1fc6a-105">**GetSearchableMailboxesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1fc6a-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="1fc6a-106">Attributes and elements</span></span>

<span data-ttu-id="1fc6a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1fc6a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1fc6a-108">属性</span><span class="sxs-lookup"><span data-stu-id="1fc6a-108">Attributes</span></span>

<span data-ttu-id="1fc6a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1fc6a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1fc6a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1fc6a-110">Child elements</span></span>

<span data-ttu-id="1fc6a-111">[SearchFilter](searchfilter.md) | [ExpandGroupMembership](expandgroupmembership.md)</span><span class="sxs-lookup"><span data-stu-id="1fc6a-111">[SearchFilter](searchfilter.md) | [ExpandGroupMembership](expandgroupmembership.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1fc6a-112">親要素</span><span class="sxs-lookup"><span data-stu-id="1fc6a-112">Parent elements</span></span>

<span data-ttu-id="1fc6a-113">なし。</span><span class="sxs-lookup"><span data-stu-id="1fc6a-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1fc6a-114">備考</span><span class="sxs-lookup"><span data-stu-id="1fc6a-114">Remarks</span></span>

<span data-ttu-id="1fc6a-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="1fc6a-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1fc6a-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="1fc6a-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1fc6a-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="1fc6a-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1fc6a-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="1fc6a-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1fc6a-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1fc6a-119">Schema name</span></span>  <br/> |<span data-ttu-id="1fc6a-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="1fc6a-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1fc6a-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1fc6a-121">Validation file</span></span>  <br/> |<span data-ttu-id="1fc6a-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1fc6a-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1fc6a-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="1fc6a-123">Can be empty</span></span>  <br/> ||
   

