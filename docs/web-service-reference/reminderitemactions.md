---
title: ReminderItemActions
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 135d7fc3-7d5b-4e30-9a6f-62eb02d7ab98
description: ReminderItemActions 要素は、アラームアイテムのアクションを指定します。
ms.openlocfilehash: c9b42e420f81cd0cb15bf1bd17366d9a996f1b0b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458559"
---
# <a name="reminderitemactions"></a><span data-ttu-id="b2b2b-103">ReminderItemActions</span><span class="sxs-lookup"><span data-stu-id="b2b2b-103">ReminderItemActions</span></span>

<span data-ttu-id="b2b2b-104">**ReminderItemActions**要素は、アラームアイテムのアクションを指定します。</span><span class="sxs-lookup"><span data-stu-id="b2b2b-104">The **ReminderItemActions** element specifies the actions for reminder items.</span></span> 
  
```XML
<ReminderItemActions>
   <ReminderItemAction></ReminderItemAction>
</ReminderItemActions>
```

 <span data-ttu-id="b2b2b-105">**NonEmptyArrayOfReminderItemActionType**</span><span class="sxs-lookup"><span data-stu-id="b2b2b-105">**NonEmptyArrayOfReminderItemActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b2b2b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b2b2b-106">Attributes and elements</span></span>

<span data-ttu-id="b2b2b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b2b2b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b2b2b-108">属性</span><span class="sxs-lookup"><span data-stu-id="b2b2b-108">Attributes</span></span>

<span data-ttu-id="b2b2b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b2b2b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b2b2b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b2b2b-110">Child elements</span></span>

[<span data-ttu-id="b2b2b-111">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="b2b2b-111">ReminderItemAction</span></span>](reminderitemaction.md)
  
### <a name="parent-elements"></a><span data-ttu-id="b2b2b-112">親要素</span><span class="sxs-lookup"><span data-stu-id="b2b2b-112">Parent elements</span></span>

[<span data-ttu-id="b2b2b-113">PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="b2b2b-113">PerformReminderAction</span></span>](performreminderaction.md)
  
## <a name="remarks"></a><span data-ttu-id="b2b2b-114">注釈</span><span class="sxs-lookup"><span data-stu-id="b2b2b-114">Remarks</span></span>

<span data-ttu-id="b2b2b-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b2b2b-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b2b2b-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b2b2b-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b2b2b-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b2b2b-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b2b2b-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="b2b2b-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b2b2b-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b2b2b-119">Schema Name</span></span>  <br/> |<span data-ttu-id="b2b2b-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="b2b2b-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b2b2b-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b2b2b-121">Validation File</span></span>  <br/> |<span data-ttu-id="b2b2b-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="b2b2b-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b2b2b-123">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b2b2b-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="b2b2b-124">正しくない</span><span class="sxs-lookup"><span data-stu-id="b2b2b-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b2b2b-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="b2b2b-125">See also</span></span>



[<span data-ttu-id="b2b2b-126">PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="b2b2b-126">PerformReminderAction</span></span>](performreminderaction.md)


- [<span data-ttu-id="b2b2b-127">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="b2b2b-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

