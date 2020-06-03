---
title: RetentionDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0c1df5e2-b56a-4947-a047-2b73b32e5fb7
description: RetentionDate 要素は、アイテムを保持する必要がある最後の日付を指定します。
ms.openlocfilehash: a1b109414d02814f9ede74c59796d5a1ff042da5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465227"
---
# <a name="retentiondate"></a><span data-ttu-id="a0988-103">RetentionDate</span><span class="sxs-lookup"><span data-stu-id="a0988-103">RetentionDate</span></span>

<span data-ttu-id="a0988-104">**RetentionDate**要素は、アイテムを保持する必要がある最後の日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="a0988-104">The **RetentionDate** element specifies the last date that an item must be retained.</span></span> 
  
```XML
<RetentionDate></RetentionDate>
```

 <span data-ttu-id="a0988-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="a0988-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a0988-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a0988-106">Attributes and elements</span></span>

<span data-ttu-id="a0988-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a0988-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a0988-108">属性</span><span class="sxs-lookup"><span data-stu-id="a0988-108">Attributes</span></span>

<span data-ttu-id="a0988-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a0988-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a0988-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a0988-110">Child elements</span></span>

<span data-ttu-id="a0988-111">なし。</span><span class="sxs-lookup"><span data-stu-id="a0988-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a0988-112">親要素</span><span class="sxs-lookup"><span data-stu-id="a0988-112">Parent elements</span></span>

<span data-ttu-id="a0988-113">[Searchプレビューアイテム](searchpreviewitem.md)  | [アイテム](item.md)  | [連絡先](contact.md)  | [メッセージ](message-ex15websvcsotherref.md)  | [DistributionList](distributionlist.md)  | [Calendaritem](calendaritem.md)  | [Postitem](postitem.md)  | [タスク](task.md)</span><span class="sxs-lookup"><span data-stu-id="a0988-113">[SearchPreviewItem](searchpreviewitem.md) | [Item](item.md) | [Contact](contact.md) | [Message](message-ex15websvcsotherref.md) | [DistributionList](distributionlist.md) | [CalendarItem](calendaritem.md) | [PostItem](postitem.md) | [Task](task.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="a0988-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a0988-114">Text value</span></span>

<span data-ttu-id="a0988-115">**RetentionDate**要素のテキスト値は、アイテムが保持されなくなる日付を表します。</span><span class="sxs-lookup"><span data-stu-id="a0988-115">The text value of the **RetentionDate** element represents the date when an item should no longer be retained.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a0988-116">注釈</span><span class="sxs-lookup"><span data-stu-id="a0988-116">Remarks</span></span>

<span data-ttu-id="a0988-117">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="a0988-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a0988-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a0988-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a0988-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a0988-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a0988-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="a0988-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a0988-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a0988-121">Schema name</span></span>  <br/> |<span data-ttu-id="a0988-122">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="a0988-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="a0988-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a0988-123">Validation file</span></span>  <br/> |<span data-ttu-id="a0988-124">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="a0988-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a0988-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a0988-125">Can be empty</span></span>  <br/> ||
   

