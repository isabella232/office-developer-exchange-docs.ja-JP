---
title: ContactIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c444f818-412b-41ac-9523-50246e50eae0
description: アイテム識別子を要素の配列を格納する ContactIds に問い合わせてください。
ms.openlocfilehash: 8580a1aca908f0b116ef8011a8d81e6c967fc3b4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759671"
---
# <a name="contactids"></a><span data-ttu-id="8d03b-103">ContactIds</span><span class="sxs-lookup"><span data-stu-id="8d03b-103">ContactIds</span></span>

<span data-ttu-id="8d03b-104">**ContactIds**要素には、連絡先アイテムの識別子の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8d03b-104">The **ContactIds** element contains an array of contact item identifiers.</span></span> 
  
```XML
<ContactIds>
   <ItemId/>
   <OccurrenceItemId/>
   <RecurringMasterItemId/>
   <RecurringMasterItemIdRanges/>
</ContactIds>
```

 <span data-ttu-id="8d03b-105">**NonEmptyArrayOfBaseItemIdsType**</span><span class="sxs-lookup"><span data-stu-id="8d03b-105">**NonEmptyArrayOfBaseItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8d03b-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8d03b-106">Attributes and elements</span></span>

<span data-ttu-id="8d03b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8d03b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8d03b-108">属性</span><span class="sxs-lookup"><span data-stu-id="8d03b-108">Attributes</span></span>

<span data-ttu-id="8d03b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8d03b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8d03b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8d03b-110">Child elements</span></span>

<span data-ttu-id="8d03b-111">[ItemId](itemid.md) | [OccurrenceItemId](occurrenceitemid.md) | [RecurringMasterItemId](recurringmasteritemid.md) | [RecurringMasterItemIdRanges](recurringmasteritemidranges.md)</span><span class="sxs-lookup"><span data-stu-id="8d03b-111">[ItemId](itemid.md) | [OccurrenceItemId](occurrenceitemid.md) | [RecurringMasterItemId](recurringmasteritemid.md) | [RecurringMasterItemIdRanges](recurringmasteritemidranges.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8d03b-112">親要素</span><span class="sxs-lookup"><span data-stu-id="8d03b-112">Parent elements</span></span>

[<span data-ttu-id="8d03b-113">GetImItems</span><span class="sxs-lookup"><span data-stu-id="8d03b-113">GetImItems</span></span>](getimitems.md)
  
## <a name="remarks"></a><span data-ttu-id="8d03b-114">備考</span><span class="sxs-lookup"><span data-stu-id="8d03b-114">Remarks</span></span>

<span data-ttu-id="8d03b-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="8d03b-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8d03b-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="8d03b-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8d03b-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="8d03b-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8d03b-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="8d03b-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8d03b-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8d03b-119">Schema name</span></span>  <br/> |<span data-ttu-id="8d03b-120">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="8d03b-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="8d03b-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8d03b-121">Validation file</span></span>  <br/> |<span data-ttu-id="8d03b-122">types.xsd</span><span class="sxs-lookup"><span data-stu-id="8d03b-122">types.xsd</span></span>  <br/> |
|<span data-ttu-id="8d03b-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="8d03b-123">Can be empty</span></span>  <br/> |<span data-ttu-id="8d03b-124">false</span><span class="sxs-lookup"><span data-stu-id="8d03b-124">false</span></span>  <br/> |
   

