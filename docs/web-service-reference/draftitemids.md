---
title: DraftItemIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c228f7e7-6dc8-476d-9b8c-99cd5b6f9f0c
description: DraftItemIds 要素には、スレッド内の下書きアイテムのアイテム識別子の配列が含まれています。
ms.openlocfilehash: 5e635e354c9d2d768bab5efaafafde272fe568d3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463574"
---
# <a name="draftitemids"></a><span data-ttu-id="b49e1-103">DraftItemIds</span><span class="sxs-lookup"><span data-stu-id="b49e1-103">DraftItemIds</span></span>

<span data-ttu-id="b49e1-104">**DraftItemIds**要素には、スレッド内の下書きアイテムのアイテム識別子の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b49e1-104">The **DraftItemIds** element contains an array of item identifiers to draft items in a conversation.</span></span> 
  
```XML
<DraftItemIds>
   <ItemId/>
   <OccirrenceItemId/>
   <RecurringMasterItemId/>
   <RecurringMasterItemIdRanges/>
</DraftItemIds>
```

 <span data-ttu-id="b49e1-105">**非 Emptyarrayofbaseitemidstype**</span><span class="sxs-lookup"><span data-stu-id="b49e1-105">**NonEmptyArrayOfBaseItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b49e1-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b49e1-106">Attributes and elements</span></span>

<span data-ttu-id="b49e1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b49e1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b49e1-108">属性</span><span class="sxs-lookup"><span data-stu-id="b49e1-108">Attributes</span></span>

<span data-ttu-id="b49e1-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b49e1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b49e1-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b49e1-110">Child elements</span></span>

<span data-ttu-id="b49e1-111">[ItemId](itemid.md)  | [OccurrenceItemId](occurrenceitemid.md)  | [RecurringMasterItemId](recurringmasteritemid.md)  | [RecurringMasterItemIdRanges](recurringmasteritemidranges.md)</span><span class="sxs-lookup"><span data-stu-id="b49e1-111">[ItemId](itemid.md) | [OccurrenceItemId](occurrenceitemid.md) | [RecurringMasterItemId](recurringmasteritemid.md) | [RecurringMasterItemIdRanges](recurringmasteritemidranges.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b49e1-112">親要素</span><span class="sxs-lookup"><span data-stu-id="b49e1-112">Parent elements</span></span>

[<span data-ttu-id="b49e1-113">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="b49e1-113">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
## <a name="remarks"></a><span data-ttu-id="b49e1-114">注釈</span><span class="sxs-lookup"><span data-stu-id="b49e1-114">Remarks</span></span>

<span data-ttu-id="b49e1-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b49e1-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b49e1-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b49e1-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b49e1-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b49e1-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b49e1-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="b49e1-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b49e1-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b49e1-119">Schema name</span></span>  <br/> |<span data-ttu-id="b49e1-120">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="b49e1-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="b49e1-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b49e1-121">Validation file</span></span>  <br/> |<span data-ttu-id="b49e1-122">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="b49e1-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b49e1-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b49e1-123">Can be empty</span></span>  <br/> ||
   

