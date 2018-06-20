---
title: ファイアウォール (ReminderActionType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0ffcdcf4-8ea3-483c-bb7f-0cd84126120c
description: ファイアウォールの要素では、アラームを実行するアクションを指定します。
ms.openlocfilehash: 361259f733756995fae2c2c2390013a728e475a4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759269"
---
# <a name="actiontype-reminderactiontype"></a><span data-ttu-id="0b3a6-103">ファイアウォール (ReminderActionType)</span><span class="sxs-lookup"><span data-stu-id="0b3a6-103">ActionType (ReminderActionType)</span></span>

<span data-ttu-id="0b3a6-104">**ファイアウォール**の要素では、アラームを実行するアクションを指定します。</span><span class="sxs-lookup"><span data-stu-id="0b3a6-104">The **ActionType** element specifies the action to take on the reminder.</span></span> 
  
```XML
<ActionType> Dismiss | Snooze </ActionType>
```

 <span data-ttu-id="0b3a6-105">**ReminderActionType**</span><span class="sxs-lookup"><span data-stu-id="0b3a6-105">**ReminderActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0b3a6-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="0b3a6-106">Attributes and elements</span></span>

<span data-ttu-id="0b3a6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0b3a6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0b3a6-108">属性</span><span class="sxs-lookup"><span data-stu-id="0b3a6-108">Attributes</span></span>

<span data-ttu-id="0b3a6-109">なし。</span><span class="sxs-lookup"><span data-stu-id="0b3a6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0b3a6-110">子要素</span><span class="sxs-lookup"><span data-stu-id="0b3a6-110">Child elements</span></span>

<span data-ttu-id="0b3a6-111">なし。</span><span class="sxs-lookup"><span data-stu-id="0b3a6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0b3a6-112">親要素</span><span class="sxs-lookup"><span data-stu-id="0b3a6-112">Parent elements</span></span>

[<span data-ttu-id="0b3a6-113">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="0b3a6-113">ReminderItemAction</span></span>](reminderitemaction.md)
  
## <a name="text-value"></a><span data-ttu-id="0b3a6-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="0b3a6-114">Text value</span></span>

<span data-ttu-id="0b3a6-115">**ファイアウォール**の要素のテキスト値は、アラームを実行するアクションを指定します。</span><span class="sxs-lookup"><span data-stu-id="0b3a6-115">The text value of the **ActionType** element specifies the action to take on the reminder.</span></span> <span data-ttu-id="0b3a6-116">**アラームを消す**は、テキスト値では、アラームを終了することを示します。</span><span class="sxs-lookup"><span data-stu-id="0b3a6-116">The text value of **Dismiss** indicates the reminder should be dismissed.</span></span> <span data-ttu-id="0b3a6-117">**再通知**のテキスト値では、アラームを[NewReminderTime](newremindertime.md)要素で指定された時刻まで遅延するかを示します。</span><span class="sxs-lookup"><span data-stu-id="0b3a6-117">The text value of **Snooze** indicates that the reminder should be delayed until the time specified by the [NewReminderTime](newremindertime.md) element.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="0b3a6-118">備考</span><span class="sxs-lookup"><span data-stu-id="0b3a6-118">Remarks</span></span>

<span data-ttu-id="0b3a6-119">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="0b3a6-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0b3a6-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="0b3a6-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0b3a6-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="0b3a6-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0b3a6-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="0b3a6-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0b3a6-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0b3a6-123">Schema Name</span></span>  <br/> |<span data-ttu-id="0b3a6-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="0b3a6-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="0b3a6-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0b3a6-125">Validation File</span></span>  <br/> |<span data-ttu-id="0b3a6-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0b3a6-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0b3a6-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0b3a6-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="0b3a6-128">False</span><span class="sxs-lookup"><span data-stu-id="0b3a6-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0b3a6-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="0b3a6-129">See also</span></span>

- [<span data-ttu-id="0b3a6-130">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="0b3a6-130">ReminderItemAction</span></span>](reminderitemaction.md)
- [<span data-ttu-id="0b3a6-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="0b3a6-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

