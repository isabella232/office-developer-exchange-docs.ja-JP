---
title: NonIndexableItemStatistic
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 593e0c79-9ec2-4040-a6a3-3c5c61cbdf7c
description: NonIndexableItemStatistic 要素には、インデックスを作成できないアイテムの1つの統計情報が含まれています。
ms.openlocfilehash: cc7bee9fd2759a16dd16538d6712e40ceb005fec
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462683"
---
# <a name="nonindexableitemstatistic"></a><span data-ttu-id="037a2-103">NonIndexableItemStatistic</span><span class="sxs-lookup"><span data-stu-id="037a2-103">NonIndexableItemStatistic</span></span>

<span data-ttu-id="037a2-104">**Nonindexableitemstatistic**要素には、インデックスを作成できないアイテムの1つの統計情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="037a2-104">The **NonIndexableItemStatistic** element contains a single statistic for an item that could not be indexed</span></span> 
  
```XML
<NonIndexableItemStatistic>
   <Mailbox/>
   <ItemCount/>
   <ErrorMessage/>
</NonIndexableItemStatistic>
```

 <span data-ttu-id="037a2-105">**NonIndexableItemStatisticType**</span><span class="sxs-lookup"><span data-stu-id="037a2-105">**NonIndexableItemStatisticType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="037a2-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="037a2-106">Attributes and elements</span></span>

<span data-ttu-id="037a2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="037a2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="037a2-108">属性</span><span class="sxs-lookup"><span data-stu-id="037a2-108">Attributes</span></span>

<span data-ttu-id="037a2-109">なし。</span><span class="sxs-lookup"><span data-stu-id="037a2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="037a2-110">子要素</span><span class="sxs-lookup"><span data-stu-id="037a2-110">Child elements</span></span>

<span data-ttu-id="037a2-111">[メールボックス (文字列)](mailbox-string.md)  | [ItemCount](itemcount.md)  | [ErrorMessage](errormessage.md)</span><span class="sxs-lookup"><span data-stu-id="037a2-111">[Mailbox (string)](mailbox-string.md) | [ItemCount](itemcount.md) | [ErrorMessage](errormessage.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="037a2-112">親要素</span><span class="sxs-lookup"><span data-stu-id="037a2-112">Parent elements</span></span>

[<span data-ttu-id="037a2-113">NonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="037a2-113">NonIndexableItemStatistics</span></span>](nonindexableitemstatistics.md)
  
## <a name="remarks"></a><span data-ttu-id="037a2-114">注釈</span><span class="sxs-lookup"><span data-stu-id="037a2-114">Remarks</span></span>

<span data-ttu-id="037a2-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="037a2-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="037a2-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="037a2-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="037a2-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="037a2-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="037a2-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="037a2-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="037a2-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="037a2-119">Schema name</span></span>  <br/> |<span data-ttu-id="037a2-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="037a2-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="037a2-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="037a2-121">Validation file</span></span>  <br/> |<span data-ttu-id="037a2-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="037a2-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="037a2-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="037a2-123">Can be empty</span></span>  <br/> |<span data-ttu-id="037a2-124">いいえ</span><span class="sxs-lookup"><span data-stu-id="037a2-124">False</span></span>  <br/> |
   

