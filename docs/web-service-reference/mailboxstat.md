---
title: MailboxStat
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5f24dc30-3ac2-4c82-9dfc-be9dbdb585be
description: MailboxStat 要素は、検索の検索対象のメールボックスの統計情報を指定します。
ms.openlocfilehash: 692f15904467ce192074b14f7c2a742b3e76de8e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832296"
---
# <a name="mailboxstat"></a><span data-ttu-id="d0427-103">MailboxStat</span><span class="sxs-lookup"><span data-stu-id="d0427-103">MailboxStat</span></span>

<span data-ttu-id="d0427-104">**MailboxStat**要素は、検索の検索対象のメールボックスの統計情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="d0427-104">The **MailboxStat** element specifies statistics for a mailbox searched by discovery search.</span></span> 
  
```XML
<MailboxStat>
   <MailboxId/>
   <DisplayName/>
   <ItemCount/>
   <Size/>
</MailboxStat>
```

<span data-ttu-id="d0427-105">**MailboxStatisticsItemType**</span><span class="sxs-lookup"><span data-stu-id="d0427-105">**MailboxStatisticsItemType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d0427-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d0427-106">Attributes and elements</span></span>

<span data-ttu-id="d0427-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d0427-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d0427-108">属性</span><span class="sxs-lookup"><span data-stu-id="d0427-108">Attributes</span></span>

<span data-ttu-id="d0427-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d0427-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d0427-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d0427-110">Child elements</span></span>

<span data-ttu-id="d0427-111">[MailboxId](mailboxid.md) | [表示名 (文字列)](displayname-string.md) | [ItemCount](itemcount.md) | [サイズ (長)](size-long.md)</span><span class="sxs-lookup"><span data-stu-id="d0427-111">[MailboxId](mailboxid.md) | [DisplayName (string)](displayname-string.md) | [ItemCount](itemcount.md) | [Size (long)](size-long.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d0427-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d0427-112">Parent elements</span></span>

[<span data-ttu-id="d0427-113">MailboxStats</span><span class="sxs-lookup"><span data-stu-id="d0427-113">MailboxStats</span></span>](mailboxstats.md)
  
## <a name="remarks"></a><span data-ttu-id="d0427-114">備考</span><span class="sxs-lookup"><span data-stu-id="d0427-114">Remarks</span></span>

<span data-ttu-id="d0427-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d0427-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d0427-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d0427-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d0427-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="d0427-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d0427-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="d0427-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d0427-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d0427-119">Schema name</span></span>  <br/> |<span data-ttu-id="d0427-120">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="d0427-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="d0427-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d0427-121">Validation file</span></span>  <br/> |<span data-ttu-id="d0427-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d0427-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d0427-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d0427-123">Can be empty</span></span>  <br/> |<span data-ttu-id="d0427-124">false</span><span class="sxs-lookup"><span data-stu-id="d0427-124">false</span></span>  <br/> |
   

