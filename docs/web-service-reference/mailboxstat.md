---
title: MailboxStat
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5f24dc30-3ac2-4c82-9dfc-be9dbdb585be
description: MailboxStat 要素は、探索検索で検索されたメールボックスの統計情報を指定します。
ms.openlocfilehash: 417f63f5e1aa34c2157b1d5ad868461113afec7b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44451433"
---
# <a name="mailboxstat"></a><span data-ttu-id="9fdd0-103">MailboxStat</span><span class="sxs-lookup"><span data-stu-id="9fdd0-103">MailboxStat</span></span>

<span data-ttu-id="9fdd0-104">**MailboxStat**要素は、探索検索で検索されたメールボックスの統計情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="9fdd0-104">The **MailboxStat** element specifies statistics for a mailbox searched by discovery search.</span></span> 
  
```XML
<MailboxStat>
   <MailboxId/>
   <DisplayName/>
   <ItemCount/>
   <Size/>
</MailboxStat>
```

<span data-ttu-id="9fdd0-105">**MailboxStatisticsItemType**</span><span class="sxs-lookup"><span data-stu-id="9fdd0-105">**MailboxStatisticsItemType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="9fdd0-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9fdd0-106">Attributes and elements</span></span>

<span data-ttu-id="9fdd0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9fdd0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9fdd0-108">属性</span><span class="sxs-lookup"><span data-stu-id="9fdd0-108">Attributes</span></span>

<span data-ttu-id="9fdd0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9fdd0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9fdd0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9fdd0-110">Child elements</span></span>

<span data-ttu-id="9fdd0-111">[MailboxId](mailboxid.md)  | [DisplayName (文字列)](displayname-string.md)  | [ItemCount](itemcount.md)  | [サイズ (長い)](size-long.md)</span><span class="sxs-lookup"><span data-stu-id="9fdd0-111">[MailboxId](mailboxid.md) | [DisplayName (string)](displayname-string.md) | [ItemCount](itemcount.md) | [Size (long)](size-long.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9fdd0-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9fdd0-112">Parent elements</span></span>

[<span data-ttu-id="9fdd0-113">MailboxStats</span><span class="sxs-lookup"><span data-stu-id="9fdd0-113">MailboxStats</span></span>](mailboxstats.md)
  
## <a name="remarks"></a><span data-ttu-id="9fdd0-114">注釈</span><span class="sxs-lookup"><span data-stu-id="9fdd0-114">Remarks</span></span>

<span data-ttu-id="9fdd0-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9fdd0-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9fdd0-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9fdd0-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9fdd0-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9fdd0-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9fdd0-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="9fdd0-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9fdd0-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9fdd0-119">Schema name</span></span>  <br/> |<span data-ttu-id="9fdd0-120">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="9fdd0-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="9fdd0-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9fdd0-121">Validation file</span></span>  <br/> |<span data-ttu-id="9fdd0-122">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="9fdd0-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9fdd0-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9fdd0-123">Can be empty</span></span>  <br/> |<span data-ttu-id="9fdd0-124">false</span><span class="sxs-lookup"><span data-stu-id="9fdd0-124">false</span></span>  <br/> |
   

