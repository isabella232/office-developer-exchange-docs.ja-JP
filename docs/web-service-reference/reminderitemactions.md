---
title: ReminderItemActions
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 135d7fc3-7d5b-4e30-9a6f-62eb02d7ab98
description: ReminderItemActions 要素は、アイテムのアクションを指定します。
ms.openlocfilehash: b35bad0ed6fa56c82ff2e7c723f692589e229ce3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833073"
---
# <a name="reminderitemactions"></a><span data-ttu-id="a03c9-103">ReminderItemActions</span><span class="sxs-lookup"><span data-stu-id="a03c9-103">ReminderItemActions</span></span>

<span data-ttu-id="a03c9-104">**ReminderItemActions**要素は、アイテムのアクションを指定します。</span><span class="sxs-lookup"><span data-stu-id="a03c9-104">The **ReminderItemActions** element specifies the actions for reminder items.</span></span> 
  
```XML
<ReminderItemActions>
   <ReminderItemAction></ReminderItemAction>
</ReminderItemActions>
```

 <span data-ttu-id="a03c9-105">**NonEmptyArrayOfReminderItemActionType**</span><span class="sxs-lookup"><span data-stu-id="a03c9-105">**NonEmptyArrayOfReminderItemActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a03c9-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a03c9-106">Attributes and elements</span></span>

<span data-ttu-id="a03c9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a03c9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a03c9-108">属性</span><span class="sxs-lookup"><span data-stu-id="a03c9-108">Attributes</span></span>

<span data-ttu-id="a03c9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a03c9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a03c9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a03c9-110">Child elements</span></span>

[<span data-ttu-id="a03c9-111">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="a03c9-111">ReminderItemAction</span></span>](reminderitemaction.md)
  
### <a name="parent-elements"></a><span data-ttu-id="a03c9-112">親要素</span><span class="sxs-lookup"><span data-stu-id="a03c9-112">Parent elements</span></span>

[<span data-ttu-id="a03c9-113">PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="a03c9-113">PerformReminderAction</span></span>](performreminderaction.md)
  
## <a name="remarks"></a><span data-ttu-id="a03c9-114">備考</span><span class="sxs-lookup"><span data-stu-id="a03c9-114">Remarks</span></span>

<span data-ttu-id="a03c9-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="a03c9-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a03c9-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a03c9-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a03c9-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="a03c9-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a03c9-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="a03c9-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a03c9-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a03c9-119">Schema Name</span></span>  <br/> |<span data-ttu-id="a03c9-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="a03c9-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a03c9-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a03c9-121">Validation File</span></span>  <br/> |<span data-ttu-id="a03c9-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a03c9-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a03c9-123">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a03c9-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="a03c9-124">False</span><span class="sxs-lookup"><span data-stu-id="a03c9-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a03c9-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="a03c9-125">See also</span></span>



[<span data-ttu-id="a03c9-126">PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="a03c9-126">PerformReminderAction</span></span>](performreminderaction.md)


- [<span data-ttu-id="a03c9-127">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="a03c9-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

