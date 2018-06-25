---
title: PerformReminderAction
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cee14262-7153-44da-bb42-b856e380c4d0
description: PerformReminderAction 要素は、アラームのアクションを実行する要求を指定します。
ms.openlocfilehash: d57b7694e9678fc8e096e01c7cca162e5d2d16e8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832723"
---
# <a name="performreminderaction"></a><span data-ttu-id="5bb78-103">PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="5bb78-103">PerformReminderAction</span></span>

<span data-ttu-id="5bb78-104">**PerformReminderAction**要素は、アラームのアクションを実行する要求を指定します。</span><span class="sxs-lookup"><span data-stu-id="5bb78-104">The **PerformReminderAction** element specifies a request to perform a reminder action.</span></span> 
  
```XML
<PerformReminderAction>
   <ReminderItemActions></ReminderItemActions>
</PerformReminderAction>
```

 <span data-ttu-id="5bb78-105">**PerformReminderActionType**</span><span class="sxs-lookup"><span data-stu-id="5bb78-105">**PerformReminderActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5bb78-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5bb78-106">Attributes and elements</span></span>

<span data-ttu-id="5bb78-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5bb78-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5bb78-108">属性</span><span class="sxs-lookup"><span data-stu-id="5bb78-108">Attributes</span></span>

<span data-ttu-id="5bb78-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5bb78-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5bb78-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5bb78-110">Child elements</span></span>

[<span data-ttu-id="5bb78-111">ReminderItemActions</span><span class="sxs-lookup"><span data-stu-id="5bb78-111">ReminderItemActions</span></span>](reminderitemactions.md)
  
### <a name="parent-elements"></a><span data-ttu-id="5bb78-112">親要素</span><span class="sxs-lookup"><span data-stu-id="5bb78-112">Parent elements</span></span>

<span data-ttu-id="5bb78-113">なし。</span><span class="sxs-lookup"><span data-stu-id="5bb78-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5bb78-114">備考</span><span class="sxs-lookup"><span data-stu-id="5bb78-114">Remarks</span></span>

<span data-ttu-id="5bb78-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="5bb78-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="5bb78-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="5bb78-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5bb78-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="5bb78-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5bb78-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="5bb78-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5bb78-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5bb78-119">Schema Name</span></span>  <br/> |<span data-ttu-id="5bb78-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="5bb78-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5bb78-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5bb78-121">Validation File</span></span>  <br/> |<span data-ttu-id="5bb78-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5bb78-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5bb78-123">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5bb78-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="5bb78-124">False</span><span class="sxs-lookup"><span data-stu-id="5bb78-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5bb78-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="5bb78-125">See also</span></span>



- [<span data-ttu-id="5bb78-126">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="5bb78-126">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

