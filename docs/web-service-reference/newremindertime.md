---
title: NewReminderTime
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ff1b6b1c-3557-41d4-8aa6-9528fdb3a21a
description: NewReminderTime 要素は、アラームの新しい時刻を指定します。
ms.openlocfilehash: a10f7e481b474501f33dba4c09060766568952b0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465955"
---
# <a name="newremindertime"></a><span data-ttu-id="e2bc6-103">NewReminderTime</span><span class="sxs-lookup"><span data-stu-id="e2bc6-103">NewReminderTime</span></span>

<span data-ttu-id="e2bc6-104">**NewReminderTime**要素は、アラームの新しい時刻を指定します。</span><span class="sxs-lookup"><span data-stu-id="e2bc6-104">The **NewReminderTime** element specifies a new time for a reminder.</span></span> 
  
```XML
<NewReminderTime/>
```

 <span data-ttu-id="e2bc6-105">**string**</span><span class="sxs-lookup"><span data-stu-id="e2bc6-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e2bc6-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e2bc6-106">Attributes and elements</span></span>

<span data-ttu-id="e2bc6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e2bc6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e2bc6-108">属性</span><span class="sxs-lookup"><span data-stu-id="e2bc6-108">Attributes</span></span>

<span data-ttu-id="e2bc6-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e2bc6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e2bc6-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e2bc6-110">Child elements</span></span>

<span data-ttu-id="e2bc6-111">なし。</span><span class="sxs-lookup"><span data-stu-id="e2bc6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e2bc6-112">親要素</span><span class="sxs-lookup"><span data-stu-id="e2bc6-112">Parent elements</span></span>

[<span data-ttu-id="e2bc6-113">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="e2bc6-113">ReminderItemAction</span></span>](reminderitemaction.md)
  
## <a name="text-value"></a><span data-ttu-id="e2bc6-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e2bc6-114">Text value</span></span>

<span data-ttu-id="e2bc6-115">**NewReminderTime**要素のテキスト値は、アラームの新しい時刻です。</span><span class="sxs-lookup"><span data-stu-id="e2bc6-115">The text value of the **NewReminderTime** element is a new time for the reminder.</span></span> <span data-ttu-id="e2bc6-116">**NewReminderTime**要素は、[アラームを遅延させるために[ActionType](actiontype-reminderactiontype.md)要素を再**通知**する] に設定されている場合に使用します。</span><span class="sxs-lookup"><span data-stu-id="e2bc6-116">The **NewReminderTime** element is used when the [ActionType](actiontype-reminderactiontype.md) element is set to **Snooze**, in order to delay the reminder.</span></span> <span data-ttu-id="e2bc6-117">**NewReminderTime**の値は、 [getreminders 操作](getreminders-operation.md)によって返される[ReminderTime](remindertime.md)より大きい必要があります。</span><span class="sxs-lookup"><span data-stu-id="e2bc6-117">The value of the **NewReminderTime** must be greater than the [ReminderTime](remindertime.md) returned by the [GetReminders operation](getreminders-operation.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e2bc6-118">注釈</span><span class="sxs-lookup"><span data-stu-id="e2bc6-118">Remarks</span></span>

<span data-ttu-id="e2bc6-119">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e2bc6-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e2bc6-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e2bc6-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e2bc6-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e2bc6-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e2bc6-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="e2bc6-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e2bc6-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e2bc6-123">Schema Name</span></span>  <br/> |<span data-ttu-id="e2bc6-124">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="e2bc6-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="e2bc6-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e2bc6-125">Validation File</span></span>  <br/> |<span data-ttu-id="e2bc6-126">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="e2bc6-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e2bc6-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e2bc6-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="e2bc6-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="e2bc6-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e2bc6-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="e2bc6-129">See also</span></span>



[<span data-ttu-id="e2bc6-130">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="e2bc6-130">ReminderItemAction</span></span>](reminderitemaction.md)


- [<span data-ttu-id="e2bc6-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="e2bc6-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

