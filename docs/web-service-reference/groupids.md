---
title: GroupIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4d32cb3b-eb84-4816-89cd-26dcf5131bc8
description: GroupIds 要素は、インスタント メッセージングのグループ id の配列を指定します。
ms.openlocfilehash: 0e463a3a74eb3a4996b521f77e1175913b22d16b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831763"
---
# <a name="groupids"></a><span data-ttu-id="5c640-103">GroupIds</span><span class="sxs-lookup"><span data-stu-id="5c640-103">GroupIds</span></span>

<span data-ttu-id="5c640-104">**GroupIds**要素は、インスタント メッセージングのグループ id の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="5c640-104">The **GroupIds** element identifies an array of instant messaging group identifiers.</span></span> 
  
```XML
<GroupIds>
   <ItemId/>
   <OccurrenceItemId/>
   <RecurringMasterItemId/>
   <RecurringMasterItemIdRanges/>
</GroupIds>
```

 <span data-ttu-id="5c640-105">**NonEmptyArrayOfBaseItemIdsType**</span><span class="sxs-lookup"><span data-stu-id="5c640-105">**NonEmptyArrayOfBaseItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5c640-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5c640-106">Attributes and elements</span></span>

<span data-ttu-id="5c640-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5c640-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5c640-108">属性</span><span class="sxs-lookup"><span data-stu-id="5c640-108">Attributes</span></span>

<span data-ttu-id="5c640-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5c640-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5c640-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5c640-110">Child elements</span></span>

<span data-ttu-id="5c640-111">[ItemId](itemid.md) | [OccurrenceItemId](occurrenceitemid.md) | [RecurringMasterItemId](recurringmasteritemid.md) | [RecurringMasterItemIdRanges](recurringmasteritemidranges.md)</span><span class="sxs-lookup"><span data-stu-id="5c640-111">[ItemId](itemid.md) | [OccurrenceItemId](occurrenceitemid.md) | [RecurringMasterItemId](recurringmasteritemid.md) | [RecurringMasterItemIdRanges](recurringmasteritemidranges.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5c640-112">親要素</span><span class="sxs-lookup"><span data-stu-id="5c640-112">Parent elements</span></span>

[<span data-ttu-id="5c640-113">GetImItems</span><span class="sxs-lookup"><span data-stu-id="5c640-113">GetImItems</span></span>](getimitems.md)
  
## <a name="remarks"></a><span data-ttu-id="5c640-114">備考</span><span class="sxs-lookup"><span data-stu-id="5c640-114">Remarks</span></span>

<span data-ttu-id="5c640-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="5c640-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="5c640-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="5c640-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5c640-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="5c640-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5c640-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="5c640-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5c640-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5c640-119">Schema name</span></span>  <br/> |<span data-ttu-id="5c640-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="5c640-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5c640-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5c640-121">Validation file</span></span>  <br/> |<span data-ttu-id="5c640-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5c640-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5c640-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="5c640-123">Can be empty</span></span>  <br/> ||
   

