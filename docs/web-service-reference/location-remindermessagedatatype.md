---
title: 場所 (ReminderMessageDataType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 173148af-5dda-4322-8d0c-da3ba3780a43
description: 場所 (ReminderMessageDataType) の要素では、アラームは予定表アイテムの場所を指定します。
ms.openlocfilehash: 88cc01e42f01f09933fd060080139a69bec104cc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832242"
---
# <a name="location-remindermessagedatatype"></a><span data-ttu-id="08724-103">場所 (ReminderMessageDataType)</span><span class="sxs-lookup"><span data-stu-id="08724-103">Location (ReminderMessageDataType)</span></span>

<span data-ttu-id="08724-104">**場所 (ReminderMessageDataType)** の要素では、アラームは予定表アイテムの場所を指定します。</span><span class="sxs-lookup"><span data-stu-id="08724-104">The **Location (ReminderMessageDataType)** element specifies the location of the calendar item that the reminder is for.</span></span> 
  
```xml
<Location/>
```

 <span data-ttu-id="08724-105">**string**</span><span class="sxs-lookup"><span data-stu-id="08724-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="08724-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="08724-106">Attributes and elements</span></span>

<span data-ttu-id="08724-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="08724-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="08724-108">属性</span><span class="sxs-lookup"><span data-stu-id="08724-108">Attributes</span></span>

<span data-ttu-id="08724-109">なし。</span><span class="sxs-lookup"><span data-stu-id="08724-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="08724-110">子要素</span><span class="sxs-lookup"><span data-stu-id="08724-110">Child elements</span></span>

<span data-ttu-id="08724-111">なし。</span><span class="sxs-lookup"><span data-stu-id="08724-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="08724-112">親要素</span><span class="sxs-lookup"><span data-stu-id="08724-112">Parent elements</span></span>

[<span data-ttu-id="08724-113">Reminder</span><span class="sxs-lookup"><span data-stu-id="08724-113">Reminder</span></span>](reminder.md)
  
## <a name="text-value"></a><span data-ttu-id="08724-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="08724-114">Text value</span></span>

<span data-ttu-id="08724-115">**Location**要素のテキスト値は、予定表アイテムの場所です。</span><span class="sxs-lookup"><span data-stu-id="08724-115">The text value of the **Location** element is the location of the calendar item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="08724-116">備考</span><span class="sxs-lookup"><span data-stu-id="08724-116">Remarks</span></span>

<span data-ttu-id="08724-117">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="08724-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="08724-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="08724-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="08724-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="08724-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="08724-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="08724-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="08724-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="08724-121">Schema Name</span></span>  <br/> |<span data-ttu-id="08724-122">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="08724-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="08724-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="08724-123">Validation File</span></span>  <br/> |<span data-ttu-id="08724-124">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="08724-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="08724-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="08724-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="08724-126">True</span><span class="sxs-lookup"><span data-stu-id="08724-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="08724-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="08724-127">See also</span></span>



[<span data-ttu-id="08724-128">Reminder</span><span class="sxs-lookup"><span data-stu-id="08724-128">Reminder</span></span>](reminder.md)


- [<span data-ttu-id="08724-129">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="08724-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

