---
title: リマインダー
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 19294300-ab84-4784-8aa7-3395a08de640
description: アラーム要素は、GetReminders 要求に対する応答で返される通知を指定します。
ms.openlocfilehash: 1ddf1c10872dcce103919dbed3d1c5e04cdfca74
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458496"
---
# <a name="reminders"></a><span data-ttu-id="9d419-103">リマインダー</span><span class="sxs-lookup"><span data-stu-id="9d419-103">Reminders</span></span>

<span data-ttu-id="9d419-104">**アラーム**要素は、 **getreminders**要求に対する応答で返される通知を指定します。</span><span class="sxs-lookup"><span data-stu-id="9d419-104">The **Reminders** element specifies the reminders returned in the response to a **GetReminders** request.</span></span> 
  
```XML
<Reminders>
   <Reminder></Reminder>
</Reminders>
```

 <span data-ttu-id="9d419-105">**ArrayOfRemindersType**</span><span class="sxs-lookup"><span data-stu-id="9d419-105">**ArrayOfRemindersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9d419-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9d419-106">Attributes and elements</span></span>

<span data-ttu-id="9d419-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9d419-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9d419-108">属性</span><span class="sxs-lookup"><span data-stu-id="9d419-108">Attributes</span></span>

<span data-ttu-id="9d419-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9d419-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9d419-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9d419-110">Child elements</span></span>

[<span data-ttu-id="9d419-111">Reminder</span><span class="sxs-lookup"><span data-stu-id="9d419-111">Reminder</span></span>](reminder.md)
  
### <a name="parent-elements"></a><span data-ttu-id="9d419-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9d419-112">Parent elements</span></span>

[<span data-ttu-id="9d419-113">GetRemindersResponse</span><span class="sxs-lookup"><span data-stu-id="9d419-113">GetRemindersResponse</span></span>](getremindersresponse.md)
  
## <a name="remarks"></a><span data-ttu-id="9d419-114">注釈</span><span class="sxs-lookup"><span data-stu-id="9d419-114">Remarks</span></span>

<span data-ttu-id="9d419-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9d419-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9d419-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9d419-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9d419-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9d419-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9d419-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="9d419-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9d419-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9d419-119">Schema Name</span></span>  <br/> |<span data-ttu-id="9d419-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="9d419-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9d419-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9d419-121">Validation File</span></span>  <br/> |<span data-ttu-id="9d419-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="9d419-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9d419-123">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9d419-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="9d419-124">正しくない</span><span class="sxs-lookup"><span data-stu-id="9d419-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9d419-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="9d419-125">See also</span></span>



[<span data-ttu-id="9d419-126">GetRemindersResponse</span><span class="sxs-lookup"><span data-stu-id="9d419-126">GetRemindersResponse</span></span>](getremindersresponse.md)


- [<span data-ttu-id="9d419-127">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="9d419-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

