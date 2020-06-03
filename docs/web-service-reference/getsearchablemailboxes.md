---
title: GetSearchableMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 949871f7-0d10-498e-84aa-f0652f1193be
description: GetSearchableMailboxes 要素には、クライアントが電子情報開示検索を実行するためのアクセス許可を持っているメールボックスの一覧を取得する要求が含まれます。
ms.openlocfilehash: a327f8766e53e9f1fae6928179d5a4b8e3d044a8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530191"
---
# <a name="getsearchablemailboxes"></a><span data-ttu-id="8a613-103">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="8a613-103">GetSearchableMailboxes</span></span>

<span data-ttu-id="8a613-104">**Getsearchablemailboxes**要素には、クライアントが電子情報開示検索を実行するためのアクセス許可を持っているメールボックスの一覧を取得する要求が含まれます。</span><span class="sxs-lookup"><span data-stu-id="8a613-104">The **GetSearchableMailboxes** element contains a request to get a list of mailboxes that the client has permission to perform an eDiscovery search.</span></span> 
  
```XML
<GetSearchableMailboxes>
   <SearchFilter/>
   <ExpandGroupMembership/>
</GetSearchableMailboxes>
```

 <span data-ttu-id="8a613-105">**Getsearchablemailboxestoff**</span><span class="sxs-lookup"><span data-stu-id="8a613-105">**GetSearchableMailboxesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8a613-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="8a613-106">Attributes and elements</span></span>

<span data-ttu-id="8a613-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8a613-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8a613-108">属性</span><span class="sxs-lookup"><span data-stu-id="8a613-108">Attributes</span></span>

<span data-ttu-id="8a613-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8a613-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8a613-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8a613-110">Child elements</span></span>

<span data-ttu-id="8a613-111">[Searchfilter](searchfilter.md)  | [Expandgroupmembership](expandgroupmembership.md)</span><span class="sxs-lookup"><span data-stu-id="8a613-111">[SearchFilter](searchfilter.md) | [ExpandGroupMembership](expandgroupmembership.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8a613-112">親要素</span><span class="sxs-lookup"><span data-stu-id="8a613-112">Parent elements</span></span>

<span data-ttu-id="8a613-113">なし。</span><span class="sxs-lookup"><span data-stu-id="8a613-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8a613-114">注釈</span><span class="sxs-lookup"><span data-stu-id="8a613-114">Remarks</span></span>

<span data-ttu-id="8a613-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="8a613-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8a613-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="8a613-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8a613-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="8a613-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8a613-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="8a613-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8a613-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8a613-119">Schema name</span></span>  <br/> |<span data-ttu-id="8a613-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="8a613-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8a613-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8a613-121">Validation file</span></span>  <br/> |<span data-ttu-id="8a613-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="8a613-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8a613-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="8a613-123">Can be empty</span></span>  <br/> ||
   

