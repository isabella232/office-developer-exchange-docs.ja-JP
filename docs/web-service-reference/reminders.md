---
title: アラーム
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 19294300-ab84-4784-8aa7-3395a08de640
description: アラームの要素は、GetReminders 要求への応答で返されるメッセージを指定します。
ms.openlocfilehash: 955fc568dc919d591076271382a8c9bbd1d146ad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833071"
---
# <a name="reminders"></a><span data-ttu-id="7c12e-103">アラーム</span><span class="sxs-lookup"><span data-stu-id="7c12e-103">Reminders</span></span>

<span data-ttu-id="7c12e-104">**アラーム**の要素は、 **GetReminders**要求への応答で返されるメッセージを指定します。</span><span class="sxs-lookup"><span data-stu-id="7c12e-104">The **Reminders** element specifies the reminders returned in the response to a **GetReminders** request.</span></span> 
  
```XML
<Reminders>
   <Reminder></Reminder>
</Reminders>
```

 <span data-ttu-id="7c12e-105">**ArrayOfRemindersType**</span><span class="sxs-lookup"><span data-stu-id="7c12e-105">**ArrayOfRemindersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7c12e-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7c12e-106">Attributes and elements</span></span>

<span data-ttu-id="7c12e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7c12e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7c12e-108">属性</span><span class="sxs-lookup"><span data-stu-id="7c12e-108">Attributes</span></span>

<span data-ttu-id="7c12e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7c12e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7c12e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7c12e-110">Child elements</span></span>

[<span data-ttu-id="7c12e-111">Reminder</span><span class="sxs-lookup"><span data-stu-id="7c12e-111">Reminder</span></span>](reminder.md)
  
### <a name="parent-elements"></a><span data-ttu-id="7c12e-112">親要素</span><span class="sxs-lookup"><span data-stu-id="7c12e-112">Parent elements</span></span>

[<span data-ttu-id="7c12e-113">GetRemindersResponse</span><span class="sxs-lookup"><span data-stu-id="7c12e-113">GetRemindersResponse</span></span>](getremindersresponse.md)
  
## <a name="remarks"></a><span data-ttu-id="7c12e-114">備考</span><span class="sxs-lookup"><span data-stu-id="7c12e-114">Remarks</span></span>

<span data-ttu-id="7c12e-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="7c12e-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7c12e-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7c12e-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7c12e-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="7c12e-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7c12e-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="7c12e-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7c12e-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7c12e-119">Schema Name</span></span>  <br/> |<span data-ttu-id="7c12e-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="7c12e-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7c12e-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7c12e-121">Validation File</span></span>  <br/> |<span data-ttu-id="7c12e-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7c12e-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7c12e-123">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7c12e-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="7c12e-124">False</span><span class="sxs-lookup"><span data-stu-id="7c12e-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7c12e-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="7c12e-125">See also</span></span>



[<span data-ttu-id="7c12e-126">GetRemindersResponse</span><span class="sxs-lookup"><span data-stu-id="7c12e-126">GetRemindersResponse</span></span>](getremindersresponse.md)


- [<span data-ttu-id="7c12e-127">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="7c12e-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

