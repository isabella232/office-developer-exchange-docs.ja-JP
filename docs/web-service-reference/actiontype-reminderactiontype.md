---
title: ActionType (ReminderActionType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0ffcdcf4-8ea3-483c-bb7f-0cd84126120c
description: ActionType 要素は、アラームに対して実行するアクションを指定します。
ms.openlocfilehash: 5c62b2dd945b23a5ff2bb824385c45dbc617a5a5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465059"
---
# <a name="actiontype-reminderactiontype"></a><span data-ttu-id="98809-103">ActionType (ReminderActionType)</span><span class="sxs-lookup"><span data-stu-id="98809-103">ActionType (ReminderActionType)</span></span>

<span data-ttu-id="98809-104">**ActionType**要素は、アラームに対して実行するアクションを指定します。</span><span class="sxs-lookup"><span data-stu-id="98809-104">The **ActionType** element specifies the action to take on the reminder.</span></span> 
  
```XML
<ActionType> Dismiss | Snooze </ActionType>
```

 <span data-ttu-id="98809-105">**ReminderActionType**</span><span class="sxs-lookup"><span data-stu-id="98809-105">**ReminderActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="98809-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="98809-106">Attributes and elements</span></span>

<span data-ttu-id="98809-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="98809-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="98809-108">属性</span><span class="sxs-lookup"><span data-stu-id="98809-108">Attributes</span></span>

<span data-ttu-id="98809-109">なし。</span><span class="sxs-lookup"><span data-stu-id="98809-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="98809-110">子要素</span><span class="sxs-lookup"><span data-stu-id="98809-110">Child elements</span></span>

<span data-ttu-id="98809-111">なし。</span><span class="sxs-lookup"><span data-stu-id="98809-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="98809-112">親要素</span><span class="sxs-lookup"><span data-stu-id="98809-112">Parent elements</span></span>

[<span data-ttu-id="98809-113">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="98809-113">ReminderItemAction</span></span>](reminderitemaction.md)
  
## <a name="text-value"></a><span data-ttu-id="98809-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="98809-114">Text value</span></span>

<span data-ttu-id="98809-115">**ActionType**要素のテキスト値は、アラームに対して実行するアクションを指定します。</span><span class="sxs-lookup"><span data-stu-id="98809-115">The text value of the **ActionType** element specifies the action to take on the reminder.</span></span> <span data-ttu-id="98809-116">[閉じる] のテキスト値は、アラームを**消す**必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="98809-116">The text value of **Dismiss** indicates the reminder should be dismissed.</span></span> <span data-ttu-id="98809-117">[再**通知**] のテキスト値は、 [NewReminderTime](newremindertime.md)要素によって指定された時間までアラームを遅延させる必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="98809-117">The text value of **Snooze** indicates that the reminder should be delayed until the time specified by the [NewReminderTime](newremindertime.md) element.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="98809-118">注釈</span><span class="sxs-lookup"><span data-stu-id="98809-118">Remarks</span></span>

<span data-ttu-id="98809-119">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="98809-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="98809-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="98809-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="98809-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="98809-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="98809-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="98809-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="98809-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="98809-123">Schema Name</span></span>  <br/> |<span data-ttu-id="98809-124">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="98809-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="98809-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="98809-125">Validation File</span></span>  <br/> |<span data-ttu-id="98809-126">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="98809-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="98809-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="98809-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="98809-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="98809-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="98809-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="98809-129">See also</span></span>

- [<span data-ttu-id="98809-130">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="98809-130">ReminderItemAction</span></span>](reminderitemaction.md)
- [<span data-ttu-id="98809-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="98809-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

