---
title: ReminderType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bfaf84eb-271a-4728-84fc-a20205a100bd
description: ReminderType 要素は、取得するのにはアラームの種類を指定します。
ms.openlocfilehash: 11739d2068a1009b2840b2169e86b113151cbfa9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833077"
---
# <a name="remindertype"></a><span data-ttu-id="04f0d-103">ReminderType</span><span class="sxs-lookup"><span data-stu-id="04f0d-103">ReminderType</span></span>

<span data-ttu-id="04f0d-104">**ReminderType**要素は、取得するのにはアラームの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="04f0d-104">The **ReminderType** element specifies the type of reminders to return.</span></span> 
  
```XML
<ReminderType> All | Current | Old </ReminderType>
```

 <span data-ttu-id="04f0d-105">**string**</span><span class="sxs-lookup"><span data-stu-id="04f0d-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="04f0d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="04f0d-106">Attributes and elements</span></span>

<span data-ttu-id="04f0d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="04f0d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="04f0d-108">属性</span><span class="sxs-lookup"><span data-stu-id="04f0d-108">Attributes</span></span>

<span data-ttu-id="04f0d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="04f0d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="04f0d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="04f0d-110">Child elements</span></span>

<span data-ttu-id="04f0d-111">なし。</span><span class="sxs-lookup"><span data-stu-id="04f0d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="04f0d-112">親要素</span><span class="sxs-lookup"><span data-stu-id="04f0d-112">Parent elements</span></span>

[<span data-ttu-id="04f0d-113">GetReminders</span><span class="sxs-lookup"><span data-stu-id="04f0d-113">GetReminders</span></span>](getreminders.md)
  
## <a name="text-value"></a><span data-ttu-id="04f0d-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="04f0d-114">Text value</span></span>

<span data-ttu-id="04f0d-115">**ReminderType**要素のテキスト値は、戻るには、**すべて**、**現在**、または**以前**のいずれかのアラームの種類です。</span><span class="sxs-lookup"><span data-stu-id="04f0d-115">The text value of the **ReminderType** element is the type of reminders to return, either **All**, **Current**, or **Old**.</span></span> <span data-ttu-id="04f0d-116">**すべて**は、この要素に推奨される値です。</span><span class="sxs-lookup"><span data-stu-id="04f0d-116">**All** is the recommended value for this element.</span></span> <span data-ttu-id="04f0d-117">**ReminderType**要素と[形式の BeginTime](begintime.md)と[終了時刻](endtime-remindermessagedatatype.md)の要素間のリレーションシップの詳細については、 [GetReminders の操作](getreminders-operation.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="04f0d-117">For more information about the relationship between the **ReminderType** element and the [BeginTime](begintime.md) and [EndTime](endtime-remindermessagedatatype.md) elements, see [GetReminders operation](getreminders-operation.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="04f0d-118">備考</span><span class="sxs-lookup"><span data-stu-id="04f0d-118">Remarks</span></span>

<span data-ttu-id="04f0d-119">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="04f0d-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="04f0d-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="04f0d-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="04f0d-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="04f0d-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="04f0d-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="04f0d-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="04f0d-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="04f0d-123">Schema Name</span></span>  <br/> |<span data-ttu-id="04f0d-124">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="04f0d-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="04f0d-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="04f0d-125">Validation File</span></span>  <br/> |<span data-ttu-id="04f0d-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="04f0d-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="04f0d-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="04f0d-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="04f0d-128">False</span><span class="sxs-lookup"><span data-stu-id="04f0d-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="04f0d-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="04f0d-129">See also</span></span>



[<span data-ttu-id="04f0d-130">GetReminders</span><span class="sxs-lookup"><span data-stu-id="04f0d-130">GetReminders</span></span>](getreminders.md)


- [<span data-ttu-id="04f0d-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="04f0d-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

