---
title: ReminderItemAction
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fe67512c-5b15-4f07-8628-74cf873c2d71
description: ReminderItemAction 要素は、アラームのアイテムのアクションを指定します。
ms.openlocfilehash: f44e8d354aedca2c1f950238d87ab5c2d6387954
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833069"
---
# <a name="reminderitemaction"></a><span data-ttu-id="fb58c-103">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="fb58c-103">ReminderItemAction</span></span>

<span data-ttu-id="fb58c-104">**ReminderItemAction**要素は、アラームのアイテムのアクションを指定します。</span><span class="sxs-lookup"><span data-stu-id="fb58c-104">The **ReminderItemAction** element specifies the action for a reminder item.</span></span> 
  
```XML
<ReminderItemAction>
   <ActionType></ActionType>
   <ItemId></ItemId>
   <NewReminderTime></NewReminderTime>
</ReminderItemAction>
```

 <span data-ttu-id="fb58c-105">**ReminderItemActionType**</span><span class="sxs-lookup"><span data-stu-id="fb58c-105">**ReminderItemActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fb58c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="fb58c-106">Attributes and elements</span></span>

<span data-ttu-id="fb58c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fb58c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fb58c-108">属性</span><span class="sxs-lookup"><span data-stu-id="fb58c-108">Attributes</span></span>

<span data-ttu-id="fb58c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="fb58c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fb58c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="fb58c-110">Child elements</span></span>

<span data-ttu-id="fb58c-111">[ファイアウォール (ReminderActionType)](actiontype-reminderactiontype.md) | [アイテム Id](itemid.md) | [NewReminderTime](newremindertime.md)</span><span class="sxs-lookup"><span data-stu-id="fb58c-111">[ActionType (ReminderActionType)](actiontype-reminderactiontype.md) | [ItemId](itemid.md) | [NewReminderTime](newremindertime.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fb58c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="fb58c-112">Parent elements</span></span>

[<span data-ttu-id="fb58c-113">ReminderItemActions</span><span class="sxs-lookup"><span data-stu-id="fb58c-113">ReminderItemActions</span></span>](reminderitemactions.md)
  
## <a name="remarks"></a><span data-ttu-id="fb58c-114">備考</span><span class="sxs-lookup"><span data-stu-id="fb58c-114">Remarks</span></span>

<span data-ttu-id="fb58c-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="fb58c-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="fb58c-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="fb58c-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fb58c-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="fb58c-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fb58c-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="fb58c-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fb58c-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fb58c-119">Schema Name</span></span>  <br/> |<span data-ttu-id="fb58c-120">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="fb58c-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="fb58c-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fb58c-121">Validation File</span></span>  <br/> |<span data-ttu-id="fb58c-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fb58c-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fb58c-123">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="fb58c-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="fb58c-124">False</span><span class="sxs-lookup"><span data-stu-id="fb58c-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fb58c-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="fb58c-125">See also</span></span>



[<span data-ttu-id="fb58c-126">ReminderItemActions</span><span class="sxs-lookup"><span data-stu-id="fb58c-126">ReminderItemActions</span></span>](reminderitemactions.md)


- [<span data-ttu-id="fb58c-127">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="fb58c-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

