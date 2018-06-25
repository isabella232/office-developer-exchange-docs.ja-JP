---
title: ReminderGroup
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3e23c2a1-05d8-4fec-897c-f684a5b97e4c
description: ReminderGroup 要素は、アラームは予定表アイテムや仕事かどうかを指定します。
ms.openlocfilehash: d9d31cdab482d04149428021ad44cc742108053a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833060"
---
# <a name="remindergroup"></a><span data-ttu-id="667ba-103">ReminderGroup</span><span class="sxs-lookup"><span data-stu-id="667ba-103">ReminderGroup</span></span>

<span data-ttu-id="667ba-104">**ReminderGroup**要素は、アラームは予定表アイテムや仕事かどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="667ba-104">The **ReminderGroup** element specifies whether the reminder is for a calendar item or a task.</span></span> 
  
```XML
<ReminderGroup> Calendar | Task </ReminderGroup>
```

 <span data-ttu-id="667ba-105">**ReminderGroupType**</span><span class="sxs-lookup"><span data-stu-id="667ba-105">**ReminderGroupType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="667ba-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="667ba-106">Attributes and elements</span></span>

<span data-ttu-id="667ba-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="667ba-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="667ba-108">属性</span><span class="sxs-lookup"><span data-stu-id="667ba-108">Attributes</span></span>

<span data-ttu-id="667ba-109">なし。</span><span class="sxs-lookup"><span data-stu-id="667ba-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="667ba-110">子要素</span><span class="sxs-lookup"><span data-stu-id="667ba-110">Child elements</span></span>

<span data-ttu-id="667ba-111">なし。</span><span class="sxs-lookup"><span data-stu-id="667ba-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="667ba-112">親要素</span><span class="sxs-lookup"><span data-stu-id="667ba-112">Parent elements</span></span>

[<span data-ttu-id="667ba-113">Reminder</span><span class="sxs-lookup"><span data-stu-id="667ba-113">Reminder</span></span>](reminder.md)
  
## <a name="text-value"></a><span data-ttu-id="667ba-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="667ba-114">Text value</span></span>

<span data-ttu-id="667ba-115">**ReminderGroup**要素のテキスト値は、アラームのグループの種類です。</span><span class="sxs-lookup"><span data-stu-id="667ba-115">The text value of the **ReminderGroup** element is the group type of the reminder.</span></span> <span data-ttu-id="667ba-116">**予定表**のテキスト値は、アラームは予定表アイテムのことを指定します。</span><span class="sxs-lookup"><span data-stu-id="667ba-116">The text value of **Calendar** specifies that the reminder is for a calendar item.</span></span> <span data-ttu-id="667ba-117">**タスク**のテキスト値は、アラームが、作業項目を指定します。</span><span class="sxs-lookup"><span data-stu-id="667ba-117">The text value of **Task** specifies that the reminder is for a task item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="667ba-118">備考</span><span class="sxs-lookup"><span data-stu-id="667ba-118">Remarks</span></span>

<span data-ttu-id="667ba-119">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="667ba-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="667ba-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="667ba-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="667ba-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="667ba-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="667ba-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="667ba-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="667ba-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="667ba-123">Schema Name</span></span>  <br/> |<span data-ttu-id="667ba-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="667ba-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="667ba-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="667ba-125">Validation File</span></span>  <br/> |<span data-ttu-id="667ba-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="667ba-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="667ba-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="667ba-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="667ba-128">False</span><span class="sxs-lookup"><span data-stu-id="667ba-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="667ba-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="667ba-129">See also</span></span>



[<span data-ttu-id="667ba-130">Reminder</span><span class="sxs-lookup"><span data-stu-id="667ba-130">Reminder</span></span>](reminder.md)


- [<span data-ttu-id="667ba-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="667ba-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

