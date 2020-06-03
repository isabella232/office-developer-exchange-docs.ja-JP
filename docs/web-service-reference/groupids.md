---
title: Groupid
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4d32cb3b-eb84-4816-89cd-26dcf5131bc8
description: GroupIds 要素は、インスタントメッセージンググループ識別子の配列を識別します。
ms.openlocfilehash: 7583a197413063289739f0f32d9410047fc2f23d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530086"
---
# <a name="groupids"></a><span data-ttu-id="93ac8-103">Groupid</span><span class="sxs-lookup"><span data-stu-id="93ac8-103">GroupIds</span></span>

<span data-ttu-id="93ac8-104">**Groupids**要素は、インスタントメッセージンググループ識別子の配列を識別します。</span><span class="sxs-lookup"><span data-stu-id="93ac8-104">The **GroupIds** element identifies an array of instant messaging group identifiers.</span></span> 
  
```XML
<GroupIds>
   <ItemId/>
   <OccurrenceItemId/>
   <RecurringMasterItemId/>
   <RecurringMasterItemIdRanges/>
</GroupIds>
```

 <span data-ttu-id="93ac8-105">**非 Emptyarrayofbaseitemidstype**</span><span class="sxs-lookup"><span data-stu-id="93ac8-105">**NonEmptyArrayOfBaseItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="93ac8-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="93ac8-106">Attributes and elements</span></span>

<span data-ttu-id="93ac8-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="93ac8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="93ac8-108">属性</span><span class="sxs-lookup"><span data-stu-id="93ac8-108">Attributes</span></span>

<span data-ttu-id="93ac8-109">なし。</span><span class="sxs-lookup"><span data-stu-id="93ac8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="93ac8-110">子要素</span><span class="sxs-lookup"><span data-stu-id="93ac8-110">Child elements</span></span>

<span data-ttu-id="93ac8-111">[ItemId](itemid.md)  | [OccurrenceItemId](occurrenceitemid.md)  | [RecurringMasterItemId](recurringmasteritemid.md)  | [RecurringMasterItemIdRanges](recurringmasteritemidranges.md)</span><span class="sxs-lookup"><span data-stu-id="93ac8-111">[ItemId](itemid.md) | [OccurrenceItemId](occurrenceitemid.md) | [RecurringMasterItemId](recurringmasteritemid.md) | [RecurringMasterItemIdRanges](recurringmasteritemidranges.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="93ac8-112">親要素</span><span class="sxs-lookup"><span data-stu-id="93ac8-112">Parent elements</span></span>

[<span data-ttu-id="93ac8-113">GetImItems</span><span class="sxs-lookup"><span data-stu-id="93ac8-113">GetImItems</span></span>](getimitems.md)
  
## <a name="remarks"></a><span data-ttu-id="93ac8-114">注釈</span><span class="sxs-lookup"><span data-stu-id="93ac8-114">Remarks</span></span>

<span data-ttu-id="93ac8-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="93ac8-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="93ac8-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="93ac8-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="93ac8-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="93ac8-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="93ac8-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="93ac8-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="93ac8-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="93ac8-119">Schema name</span></span>  <br/> |<span data-ttu-id="93ac8-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="93ac8-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="93ac8-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="93ac8-121">Validation file</span></span>  <br/> |<span data-ttu-id="93ac8-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="93ac8-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="93ac8-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="93ac8-123">Can be empty</span></span>  <br/> ||
   

