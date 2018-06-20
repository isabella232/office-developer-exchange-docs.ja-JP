---
title: NewReminderTime
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ff1b6b1c-3557-41d4-8aa6-9528fdb3a21a
description: NewReminderTime 要素は、新しいアラームの時刻を指定します。
ms.openlocfilehash: 9f3f509942c673c916cc646cd9519240aef6ea06
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832531"
---
# <a name="newremindertime"></a><span data-ttu-id="5a69c-103">NewReminderTime</span><span class="sxs-lookup"><span data-stu-id="5a69c-103">NewReminderTime</span></span>

<span data-ttu-id="5a69c-104">**NewReminderTime**要素は、新しいアラームの時刻を指定します。</span><span class="sxs-lookup"><span data-stu-id="5a69c-104">The **NewReminderTime** element specifies a new time for a reminder.</span></span> 
  
```XML
<NewReminderTime/>
```

 <span data-ttu-id="5a69c-105">**string**</span><span class="sxs-lookup"><span data-stu-id="5a69c-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5a69c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5a69c-106">Attributes and elements</span></span>

<span data-ttu-id="5a69c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5a69c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5a69c-108">属性</span><span class="sxs-lookup"><span data-stu-id="5a69c-108">Attributes</span></span>

<span data-ttu-id="5a69c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5a69c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5a69c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5a69c-110">Child elements</span></span>

<span data-ttu-id="5a69c-111">なし。</span><span class="sxs-lookup"><span data-stu-id="5a69c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5a69c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="5a69c-112">Parent elements</span></span>

[<span data-ttu-id="5a69c-113">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="5a69c-113">ReminderItemAction</span></span>](reminderitemaction.md)
  
## <a name="text-value"></a><span data-ttu-id="5a69c-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="5a69c-114">Text value</span></span>

<span data-ttu-id="5a69c-115">**NewReminderTime**要素のテキスト値とは、新しいアラームの時刻です。</span><span class="sxs-lookup"><span data-stu-id="5a69c-115">The text value of the **NewReminderTime** element is a new time for the reminder.</span></span> <span data-ttu-id="5a69c-116">**NewReminderTime**要素は、[ファイアウォール](actiontype-reminderactiontype.md)の要素に設定すると**再通知**、アラームを延期するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="5a69c-116">The **NewReminderTime** element is used when the [ActionType](actiontype-reminderactiontype.md) element is set to **Snooze**, in order to delay the reminder.</span></span> <span data-ttu-id="5a69c-117">**NewReminderTime**の値は、 [GetReminders 操作](getreminders-operation.md)によって返される[ReminderTime](remindertime.md)よりも大きい必要があります。</span><span class="sxs-lookup"><span data-stu-id="5a69c-117">The value of the **NewReminderTime** must be greater than the [ReminderTime](remindertime.md) returned by the [GetReminders operation](getreminders-operation.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5a69c-118">備考</span><span class="sxs-lookup"><span data-stu-id="5a69c-118">Remarks</span></span>

<span data-ttu-id="5a69c-119">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="5a69c-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="5a69c-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="5a69c-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5a69c-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="5a69c-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5a69c-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="5a69c-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5a69c-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5a69c-123">Schema Name</span></span>  <br/> |<span data-ttu-id="5a69c-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="5a69c-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="5a69c-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5a69c-125">Validation File</span></span>  <br/> |<span data-ttu-id="5a69c-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5a69c-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5a69c-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5a69c-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="5a69c-128">False</span><span class="sxs-lookup"><span data-stu-id="5a69c-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5a69c-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="5a69c-129">See also</span></span>



[<span data-ttu-id="5a69c-130">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="5a69c-130">ReminderItemAction</span></span>](reminderitemaction.md)


- [<span data-ttu-id="5a69c-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="5a69c-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

