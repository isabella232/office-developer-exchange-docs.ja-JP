---
title: GetRemindersResponse
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1b1c7288-2a98-4142-8961-4d2ebca5c37c
description: GetRemindersResponse 要素は、GetReminders 要求への応答を指定します。
ms.openlocfilehash: 1882ab377365908c0bc272059ab4e007c43d788c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760842"
---
# <a name="getremindersresponse"></a><span data-ttu-id="07a1d-103">GetRemindersResponse</span><span class="sxs-lookup"><span data-stu-id="07a1d-103">GetRemindersResponse</span></span>

<span data-ttu-id="07a1d-104">**GetRemindersResponse**要素は、 **GetReminders**要求への応答を指定します。</span><span class="sxs-lookup"><span data-stu-id="07a1d-104">The **GetRemindersResponse** element specifies the response to a **GetReminders** request.</span></span> 
  
```XML
<GetRemindersResponse>
   <Reminders></Reminders>
</GetRemindersResponse>

```

 <span data-ttu-id="07a1d-105">**GetRemindersResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="07a1d-105">**GetRemindersResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="07a1d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="07a1d-106">Attributes and elements</span></span>

<span data-ttu-id="07a1d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="07a1d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="07a1d-108">属性</span><span class="sxs-lookup"><span data-stu-id="07a1d-108">Attributes</span></span>

<span data-ttu-id="07a1d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="07a1d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="07a1d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="07a1d-110">Child elements</span></span>

[<span data-ttu-id="07a1d-111">Reminders</span><span class="sxs-lookup"><span data-stu-id="07a1d-111">Reminders</span></span>](reminders.md)
  
### <a name="parent-elements"></a><span data-ttu-id="07a1d-112">親要素</span><span class="sxs-lookup"><span data-stu-id="07a1d-112">Parent elements</span></span>

[<span data-ttu-id="07a1d-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="07a1d-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="07a1d-114">Remarks</span><span class="sxs-lookup"><span data-stu-id="07a1d-114">Remarks</span></span>

<span data-ttu-id="07a1d-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="07a1d-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="07a1d-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="07a1d-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="07a1d-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="07a1d-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="07a1d-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="07a1d-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="07a1d-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="07a1d-119">Schema Name</span></span>  <br/> |<span data-ttu-id="07a1d-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="07a1d-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="07a1d-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="07a1d-121">Validation File</span></span>  <br/> |<span data-ttu-id="07a1d-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="07a1d-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="07a1d-123">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="07a1d-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="07a1d-124">False</span><span class="sxs-lookup"><span data-stu-id="07a1d-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="07a1d-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="07a1d-125">See also</span></span>



[<span data-ttu-id="07a1d-126">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="07a1d-126">ResponseMessages</span></span>](responsemessages.md)


- [<span data-ttu-id="07a1d-127">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="07a1d-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

