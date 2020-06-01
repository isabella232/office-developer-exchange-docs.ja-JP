---
title: Reminder
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 54dd748a-23a5-4ea2-88f2-b74c68a3c48f
description: アラーム要素は、タスクまたは予定表アイテムの事前通知を指定します。
ms.openlocfilehash: 71e54d920a169b8060d22bb7d7d294208c344c2e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457488"
---
# <a name="reminder"></a><span data-ttu-id="d9ef0-103">Reminder</span><span class="sxs-lookup"><span data-stu-id="d9ef0-103">Reminder</span></span>

<span data-ttu-id="d9ef0-104">**アラーム**要素は、タスクまたは予定表アイテムの事前通知を指定します。</span><span class="sxs-lookup"><span data-stu-id="d9ef0-104">The **Reminder** element specifies a reminder for a task or a calendar item.</span></span> 
  
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

 <span data-ttu-id="d9ef0-105">**ReminderType**</span><span class="sxs-lookup"><span data-stu-id="d9ef0-105">**ReminderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d9ef0-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d9ef0-106">Attributes and elements</span></span>

<span data-ttu-id="d9ef0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d9ef0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d9ef0-108">属性</span><span class="sxs-lookup"><span data-stu-id="d9ef0-108">Attributes</span></span>

<span data-ttu-id="d9ef0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d9ef0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d9ef0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d9ef0-110">Child elements</span></span>

<span data-ttu-id="d9ef0-111">[件名](subject.md)  | [場所](location.md)  | [ReminderTime](remindertime.md)  | [StartDate](startdate.md)  | [EndDate (ReminderType)](enddate-remindertype.md)  | [ItemId](itemid.md)  | [RecurringMasterItemId (ItemIdType)](recurringmasteritemid-itemidtype.md)  | [ReminderGroup](remindergroup.md)  | [UID](uid.md)</span><span class="sxs-lookup"><span data-stu-id="d9ef0-111">[Subject](subject.md) | [Location](location.md) | [ReminderTime](remindertime.md) | [StartDate](startdate.md) | [EndDate (ReminderType)](enddate-remindertype.md) | [ItemId](itemid.md) | [RecurringMasterItemId (ItemIdType)](recurringmasteritemid-itemidtype.md) | [ReminderGroup](remindergroup.md) | [UID](uid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d9ef0-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d9ef0-112">Parent elements</span></span>

[<span data-ttu-id="d9ef0-113">Reminders</span><span class="sxs-lookup"><span data-stu-id="d9ef0-113">Reminders</span></span>](reminders.md)
  
## <a name="remarks"></a><span data-ttu-id="d9ef0-114">注釈</span><span class="sxs-lookup"><span data-stu-id="d9ef0-114">Remarks</span></span>

<span data-ttu-id="d9ef0-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d9ef0-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d9ef0-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d9ef0-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d9ef0-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d9ef0-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d9ef0-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="d9ef0-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d9ef0-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d9ef0-119">Schema Name</span></span>  <br/> |<span data-ttu-id="d9ef0-120">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d9ef0-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="d9ef0-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d9ef0-121">Validation File</span></span>  <br/> |<span data-ttu-id="d9ef0-122">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d9ef0-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d9ef0-123">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d9ef0-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="d9ef0-124">正しくない</span><span class="sxs-lookup"><span data-stu-id="d9ef0-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d9ef0-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="d9ef0-125">See also</span></span>



[<span data-ttu-id="d9ef0-126">Reminders</span><span class="sxs-lookup"><span data-stu-id="d9ef0-126">Reminders</span></span>](reminders.md)


- [<span data-ttu-id="d9ef0-127">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d9ef0-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

