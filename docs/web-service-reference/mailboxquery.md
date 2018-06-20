---
title: MailboxQuery
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e4b496f7-63fa-479a-b045-73276573f64f
description: MailboxQuery 要素は、クエリと、検索のスコープを指定します。
ms.openlocfilehash: 371cddd8c4f01525b654f0ad9788cf9dd62ac888
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832295"
---
# <a name="mailboxquery"></a><span data-ttu-id="3443a-103">MailboxQuery</span><span class="sxs-lookup"><span data-stu-id="3443a-103">MailboxQuery</span></span>

<span data-ttu-id="3443a-104">**MailboxQuery**要素は、クエリと、検索のスコープを指定します。</span><span class="sxs-lookup"><span data-stu-id="3443a-104">The **MailboxQuery** element specifies a query and the scope of a discovery search.</span></span> 
  
```XML
<MailboxQuery>
   <Query/>
   <MailboxSearchScopes/>
</MailboxQuery>
```

<span data-ttu-id="3443a-105">**MailboxQueryType**</span><span class="sxs-lookup"><span data-stu-id="3443a-105">**MailboxQueryType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="3443a-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="3443a-106">Attributes and elements</span></span>

<span data-ttu-id="3443a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3443a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3443a-108">属性</span><span class="sxs-lookup"><span data-stu-id="3443a-108">Attributes</span></span>

<span data-ttu-id="3443a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3443a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3443a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3443a-110">Child elements</span></span>

<span data-ttu-id="3443a-111">[クエリ](query.md) | [MailboxSearchScopes](mailboxsearchscopes.md)</span><span class="sxs-lookup"><span data-stu-id="3443a-111">[Query](query.md) | [MailboxSearchScopes](mailboxsearchscopes.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3443a-112">親要素</span><span class="sxs-lookup"><span data-stu-id="3443a-112">Parent elements</span></span>

[<span data-ttu-id="3443a-113">SearchQueries</span><span class="sxs-lookup"><span data-stu-id="3443a-113">SearchQueries</span></span>](searchqueries.md)
  
## <a name="remarks"></a><span data-ttu-id="3443a-114">備考</span><span class="sxs-lookup"><span data-stu-id="3443a-114">Remarks</span></span>

<span data-ttu-id="3443a-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="3443a-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3443a-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="3443a-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3443a-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="3443a-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3443a-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="3443a-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3443a-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3443a-119">Schema name</span></span>  <br/> |<span data-ttu-id="3443a-120">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="3443a-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="3443a-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3443a-121">Validation file</span></span>  <br/> |<span data-ttu-id="3443a-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3443a-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3443a-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="3443a-123">Can be empty</span></span>  <br/> ||
   

