---
title: アラーム
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 54dd748a-23a5-4ea2-88f2-b74c68a3c48f
description: アラームの要素は、タスク、または予定表アイテムのアラームを指定します。
ms.openlocfilehash: cfa1160bd25f5045a3da5a98f081c9dcb3debe7b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833056"
---
# <a name="reminder"></a><span data-ttu-id="d57bd-103">アラーム</span><span class="sxs-lookup"><span data-stu-id="d57bd-103">Reminder</span></span>

<span data-ttu-id="d57bd-104">**アラーム**の要素は、タスク、または予定表アイテムのアラームを指定します。</span><span class="sxs-lookup"><span data-stu-id="d57bd-104">The **Reminder** element specifies a reminder for a task or a calendar item.</span></span> 
  
```XML
<Reminder>
   <Subject></Subject>
   <Location></Location>
   <ReminderTime></ReminderTime>
   <StartDate></StartDate>
   <EndDate></EndDate>
   <ItemId></ItemId>
   <RecurringMasterItemId></RecurringMasterItemId>
   <ReminderGroup></ReminderGroup>
   <UID></UID>
</Reminder>

```

 <span data-ttu-id="d57bd-105">**ReminderType**</span><span class="sxs-lookup"><span data-stu-id="d57bd-105">**ReminderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d57bd-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d57bd-106">Attributes and elements</span></span>

<span data-ttu-id="d57bd-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d57bd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d57bd-108">属性</span><span class="sxs-lookup"><span data-stu-id="d57bd-108">Attributes</span></span>

<span data-ttu-id="d57bd-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d57bd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d57bd-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d57bd-110">Child elements</span></span>

<span data-ttu-id="d57bd-111">[件名](subject.md) | [の場所](location.md) | [ReminderTime](remindertime.md) | [開始日](startdate.md) | [終了日 (ReminderType)](enddate-remindertype.md) | [アイテム Id](itemid.md) | [RecurringMasterItemId (ItemIdType)](recurringmasteritemid-itemidtype.md)  |  [ReminderGroup](remindergroup.md) | [UID](uid.md)</span><span class="sxs-lookup"><span data-stu-id="d57bd-111">[Subject](subject.md) | [Location](location.md) | [ReminderTime](remindertime.md) | [StartDate](startdate.md) | [EndDate (ReminderType)](enddate-remindertype.md) | [ItemId](itemid.md) | [RecurringMasterItemId (ItemIdType)](recurringmasteritemid-itemidtype.md) | [ReminderGroup](remindergroup.md) | [UID](uid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d57bd-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d57bd-112">Parent elements</span></span>

[<span data-ttu-id="d57bd-113">Reminders</span><span class="sxs-lookup"><span data-stu-id="d57bd-113">Reminders</span></span>](reminders.md)
  
## <a name="remarks"></a><span data-ttu-id="d57bd-114">備考</span><span class="sxs-lookup"><span data-stu-id="d57bd-114">Remarks</span></span>

<span data-ttu-id="d57bd-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d57bd-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d57bd-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d57bd-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d57bd-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="d57bd-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d57bd-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="d57bd-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d57bd-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d57bd-119">Schema Name</span></span>  <br/> |<span data-ttu-id="d57bd-120">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="d57bd-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="d57bd-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d57bd-121">Validation File</span></span>  <br/> |<span data-ttu-id="d57bd-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d57bd-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d57bd-123">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d57bd-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="d57bd-124">False</span><span class="sxs-lookup"><span data-stu-id="d57bd-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d57bd-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="d57bd-125">See also</span></span>



[<span data-ttu-id="d57bd-126">Reminders</span><span class="sxs-lookup"><span data-stu-id="d57bd-126">Reminders</span></span>](reminders.md)


- [<span data-ttu-id="d57bd-127">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d57bd-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

