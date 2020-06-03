---
title: ReminderType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bfaf84eb-271a-4728-84fc-a20205a100bd
description: ReminderType 要素は、返される通知の種類を指定します。
ms.openlocfilehash: 4ac20143bbfb29fb8f962515f2faba224b2f973f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465528"
---
# <a name="remindertype"></a><span data-ttu-id="03e1d-103">ReminderType</span><span class="sxs-lookup"><span data-stu-id="03e1d-103">ReminderType</span></span>

<span data-ttu-id="03e1d-104">**ReminderType**要素は、返される通知の種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="03e1d-104">The **ReminderType** element specifies the type of reminders to return.</span></span> 
  
```XML
<ReminderType> All | Current | Old </ReminderType>
```

 <span data-ttu-id="03e1d-105">**string**</span><span class="sxs-lookup"><span data-stu-id="03e1d-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="03e1d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="03e1d-106">Attributes and elements</span></span>

<span data-ttu-id="03e1d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="03e1d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="03e1d-108">属性</span><span class="sxs-lookup"><span data-stu-id="03e1d-108">Attributes</span></span>

<span data-ttu-id="03e1d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="03e1d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="03e1d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="03e1d-110">Child elements</span></span>

<span data-ttu-id="03e1d-111">なし。</span><span class="sxs-lookup"><span data-stu-id="03e1d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="03e1d-112">親要素</span><span class="sxs-lookup"><span data-stu-id="03e1d-112">Parent elements</span></span>

[<span data-ttu-id="03e1d-113">GetReminders</span><span class="sxs-lookup"><span data-stu-id="03e1d-113">GetReminders</span></span>](getreminders.md)
  
## <a name="text-value"></a><span data-ttu-id="03e1d-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="03e1d-114">Text value</span></span>

<span data-ttu-id="03e1d-115">**ReminderType**要素のテキスト値は、返される通知の種類 ( **All**、 **Current**、または**Old**) です。</span><span class="sxs-lookup"><span data-stu-id="03e1d-115">The text value of the **ReminderType** element is the type of reminders to return, either **All**, **Current**, or **Old**.</span></span> <span data-ttu-id="03e1d-116">**All**は、この要素に推奨される値です。</span><span class="sxs-lookup"><span data-stu-id="03e1d-116">**All** is the recommended value for this element.</span></span> <span data-ttu-id="03e1d-117">**ReminderType**要素と[Begintime](begintime.md)および[EndTime](endtime-remindermessagedatatype.md)要素の関係の詳細については、「 [getreminders 操作](getreminders-operation.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="03e1d-117">For more information about the relationship between the **ReminderType** element and the [BeginTime](begintime.md) and [EndTime](endtime-remindermessagedatatype.md) elements, see [GetReminders operation](getreminders-operation.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="03e1d-118">注釈</span><span class="sxs-lookup"><span data-stu-id="03e1d-118">Remarks</span></span>

<span data-ttu-id="03e1d-119">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="03e1d-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="03e1d-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="03e1d-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="03e1d-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="03e1d-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="03e1d-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="03e1d-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="03e1d-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="03e1d-123">Schema Name</span></span>  <br/> |<span data-ttu-id="03e1d-124">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="03e1d-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="03e1d-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="03e1d-125">Validation File</span></span>  <br/> |<span data-ttu-id="03e1d-126">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="03e1d-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="03e1d-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="03e1d-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="03e1d-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="03e1d-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="03e1d-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="03e1d-129">See also</span></span>



[<span data-ttu-id="03e1d-130">GetReminders</span><span class="sxs-lookup"><span data-stu-id="03e1d-130">GetReminders</span></span>](getreminders.md)


- [<span data-ttu-id="03e1d-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="03e1d-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

