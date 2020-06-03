---
title: ReminderGroup
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3e23c2a1-05d8-4fec-897c-f684a5b97e4c
description: ReminderGroup 要素は、アラームが予定表アイテムまたはタスクのどちらであるかを指定します。
ms.openlocfilehash: be6f4a7d7e9d495ed7b42ed40c60f016468e8c2c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529869"
---
# <a name="remindergroup"></a><span data-ttu-id="d7dcd-103">ReminderGroup</span><span class="sxs-lookup"><span data-stu-id="d7dcd-103">ReminderGroup</span></span>

<span data-ttu-id="d7dcd-104">**ReminderGroup**要素は、アラームが予定表アイテムまたはタスクのどちらであるかを指定します。</span><span class="sxs-lookup"><span data-stu-id="d7dcd-104">The **ReminderGroup** element specifies whether the reminder is for a calendar item or a task.</span></span> 
  
```XML
<ReminderGroup> Calendar | Task </ReminderGroup>
```

 <span data-ttu-id="d7dcd-105">**ReminderGroupType**</span><span class="sxs-lookup"><span data-stu-id="d7dcd-105">**ReminderGroupType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d7dcd-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d7dcd-106">Attributes and elements</span></span>

<span data-ttu-id="d7dcd-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d7dcd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d7dcd-108">属性</span><span class="sxs-lookup"><span data-stu-id="d7dcd-108">Attributes</span></span>

<span data-ttu-id="d7dcd-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d7dcd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d7dcd-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d7dcd-110">Child elements</span></span>

<span data-ttu-id="d7dcd-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d7dcd-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d7dcd-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d7dcd-112">Parent elements</span></span>

[<span data-ttu-id="d7dcd-113">Reminder</span><span class="sxs-lookup"><span data-stu-id="d7dcd-113">Reminder</span></span>](reminder.md)
  
## <a name="text-value"></a><span data-ttu-id="d7dcd-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d7dcd-114">Text value</span></span>

<span data-ttu-id="d7dcd-115">**ReminderGroup**要素のテキスト値は、アラームのグループの種類です。</span><span class="sxs-lookup"><span data-stu-id="d7dcd-115">The text value of the **ReminderGroup** element is the group type of the reminder.</span></span> <span data-ttu-id="d7dcd-116">**予定**表のテキスト値は、予定表アイテムのアラームであることを指定します。</span><span class="sxs-lookup"><span data-stu-id="d7dcd-116">The text value of **Calendar** specifies that the reminder is for a calendar item.</span></span> <span data-ttu-id="d7dcd-117">**タスク**のテキスト値は、タスクアイテムのアラームであることを指定します。</span><span class="sxs-lookup"><span data-stu-id="d7dcd-117">The text value of **Task** specifies that the reminder is for a task item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d7dcd-118">注釈</span><span class="sxs-lookup"><span data-stu-id="d7dcd-118">Remarks</span></span>

<span data-ttu-id="d7dcd-119">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d7dcd-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d7dcd-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d7dcd-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d7dcd-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d7dcd-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d7dcd-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="d7dcd-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d7dcd-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d7dcd-123">Schema Name</span></span>  <br/> |<span data-ttu-id="d7dcd-124">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d7dcd-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="d7dcd-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d7dcd-125">Validation File</span></span>  <br/> |<span data-ttu-id="d7dcd-126">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d7dcd-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d7dcd-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d7dcd-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="d7dcd-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="d7dcd-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d7dcd-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="d7dcd-129">See also</span></span>



[<span data-ttu-id="d7dcd-130">Reminder</span><span class="sxs-lookup"><span data-stu-id="d7dcd-130">Reminder</span></span>](reminder.md)


- [<span data-ttu-id="d7dcd-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d7dcd-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

