---
title: DraftItemIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c228f7e7-6dc8-476d-9b8c-99cd5b6f9f0c
description: DraftItemIds 要素には、会話の下書きアイテムをアイテムの識別子の配列が含まれています。
ms.openlocfilehash: f6639b20641ff68fff989d2de5fa4ec2c550d5ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760163"
---
# <a name="draftitemids"></a><span data-ttu-id="ef85f-103">DraftItemIds</span><span class="sxs-lookup"><span data-stu-id="ef85f-103">DraftItemIds</span></span>

<span data-ttu-id="ef85f-104">**DraftItemIds**要素には、会話の下書きアイテムをアイテムの識別子の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ef85f-104">The **DraftItemIds** element contains an array of item identifiers to draft items in a conversation.</span></span> 
  
```XML
<DraftItemIds>
   <ItemId/>
   <OccirrenceItemId/>
   <RecurringMasterItemId/>
   <RecurringMasterItemIdRanges/>
</DraftItemIds>
```

 <span data-ttu-id="ef85f-105">**NonEmptyArrayOfBaseItemIdsType**</span><span class="sxs-lookup"><span data-stu-id="ef85f-105">**NonEmptyArrayOfBaseItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ef85f-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ef85f-106">Attributes and elements</span></span>

<span data-ttu-id="ef85f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ef85f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ef85f-108">属性</span><span class="sxs-lookup"><span data-stu-id="ef85f-108">Attributes</span></span>

<span data-ttu-id="ef85f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ef85f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ef85f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ef85f-110">Child elements</span></span>

<span data-ttu-id="ef85f-111">[ItemId](itemid.md) | [OccurrenceItemId](occurrenceitemid.md) | [RecurringMasterItemId](recurringmasteritemid.md) | [RecurringMasterItemIdRanges](recurringmasteritemidranges.md)</span><span class="sxs-lookup"><span data-stu-id="ef85f-111">[ItemId](itemid.md) | [OccurrenceItemId](occurrenceitemid.md) | [RecurringMasterItemId](recurringmasteritemid.md) | [RecurringMasterItemIdRanges](recurringmasteritemidranges.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ef85f-112">親要素</span><span class="sxs-lookup"><span data-stu-id="ef85f-112">Parent elements</span></span>

[<span data-ttu-id="ef85f-113">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="ef85f-113">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
## <a name="remarks"></a><span data-ttu-id="ef85f-114">備考</span><span class="sxs-lookup"><span data-stu-id="ef85f-114">Remarks</span></span>

<span data-ttu-id="ef85f-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="ef85f-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ef85f-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ef85f-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ef85f-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="ef85f-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ef85f-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="ef85f-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ef85f-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ef85f-119">Schema name</span></span>  <br/> |<span data-ttu-id="ef85f-120">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="ef85f-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="ef85f-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ef85f-121">Validation file</span></span>  <br/> |<span data-ttu-id="ef85f-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ef85f-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ef85f-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="ef85f-123">Can be empty</span></span>  <br/> ||
   

