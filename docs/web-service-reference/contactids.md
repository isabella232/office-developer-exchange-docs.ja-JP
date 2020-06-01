---
title: ContactIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c444f818-412b-41ac-9523-50246e50eae0
description: ContactIds 要素には、連絡先アイテムの識別子の配列が含まれています。
ms.openlocfilehash: 5c3b5621808a6931760433148e0cfe3239cd75f1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460191"
---
# <a name="contactids"></a><span data-ttu-id="b14dc-103">ContactIds</span><span class="sxs-lookup"><span data-stu-id="b14dc-103">ContactIds</span></span>

<span data-ttu-id="b14dc-104">**ContactIds**要素には、連絡先アイテムの識別子の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b14dc-104">The **ContactIds** element contains an array of contact item identifiers.</span></span> 
  
```XML
<ContactIds>
   <ItemId/>
   <OccurrenceItemId/>
   <RecurringMasterItemId/>
   <RecurringMasterItemIdRanges/>
</ContactIds>
```

 <span data-ttu-id="b14dc-105">**非 Emptyarrayofbaseitemidstype**</span><span class="sxs-lookup"><span data-stu-id="b14dc-105">**NonEmptyArrayOfBaseItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b14dc-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b14dc-106">Attributes and elements</span></span>

<span data-ttu-id="b14dc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b14dc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b14dc-108">属性</span><span class="sxs-lookup"><span data-stu-id="b14dc-108">Attributes</span></span>

<span data-ttu-id="b14dc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b14dc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b14dc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b14dc-110">Child elements</span></span>

<span data-ttu-id="b14dc-111">[ItemId](itemid.md)  | [OccurrenceItemId](occurrenceitemid.md)  | [RecurringMasterItemId](recurringmasteritemid.md)  | [RecurringMasterItemIdRanges](recurringmasteritemidranges.md)</span><span class="sxs-lookup"><span data-stu-id="b14dc-111">[ItemId](itemid.md) | [OccurrenceItemId](occurrenceitemid.md) | [RecurringMasterItemId](recurringmasteritemid.md) | [RecurringMasterItemIdRanges](recurringmasteritemidranges.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b14dc-112">親要素</span><span class="sxs-lookup"><span data-stu-id="b14dc-112">Parent elements</span></span>

[<span data-ttu-id="b14dc-113">GetImItems</span><span class="sxs-lookup"><span data-stu-id="b14dc-113">GetImItems</span></span>](getimitems.md)
  
## <a name="remarks"></a><span data-ttu-id="b14dc-114">注釈</span><span class="sxs-lookup"><span data-stu-id="b14dc-114">Remarks</span></span>

<span data-ttu-id="b14dc-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b14dc-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b14dc-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b14dc-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b14dc-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b14dc-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b14dc-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="b14dc-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b14dc-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b14dc-119">Schema name</span></span>  <br/> |<span data-ttu-id="b14dc-120">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="b14dc-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="b14dc-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b14dc-121">Validation file</span></span>  <br/> |<span data-ttu-id="b14dc-122">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="b14dc-122">types.xsd</span></span>  <br/> |
|<span data-ttu-id="b14dc-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b14dc-123">Can be empty</span></span>  <br/> |<span data-ttu-id="b14dc-124">false</span><span class="sxs-lookup"><span data-stu-id="b14dc-124">false</span></span>  <br/> |
   

