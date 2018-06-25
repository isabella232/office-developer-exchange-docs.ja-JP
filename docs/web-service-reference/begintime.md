---
title: BeginTime
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2a60c89c-9c21-4041-9593-b244ac1608ef
description: BeginTime 要素では、事前通知を照会する期間の開始を指定します。
ms.openlocfilehash: c6204dc0395e012cf511e6183856215b0d5ea6da
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759498"
---
# <a name="begintime"></a><span data-ttu-id="7f6cb-103">BeginTime</span><span class="sxs-lookup"><span data-stu-id="7f6cb-103">BeginTime</span></span>

<span data-ttu-id="7f6cb-104">**BeginTime**要素では、事前通知を照会する期間の開始を指定します。</span><span class="sxs-lookup"><span data-stu-id="7f6cb-104">The **BeginTime** element specifies the beginning of the time span to query for reminders.</span></span> 
  
```XML
<BeginTime/>
```

 <span data-ttu-id="7f6cb-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="7f6cb-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7f6cb-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7f6cb-106">Attributes and elements</span></span>

<span data-ttu-id="7f6cb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7f6cb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7f6cb-108">属性</span><span class="sxs-lookup"><span data-stu-id="7f6cb-108">Attributes</span></span>

<span data-ttu-id="7f6cb-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7f6cb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7f6cb-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7f6cb-110">Child elements</span></span>

<span data-ttu-id="7f6cb-111">なし。</span><span class="sxs-lookup"><span data-stu-id="7f6cb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7f6cb-112">親要素</span><span class="sxs-lookup"><span data-stu-id="7f6cb-112">Parent elements</span></span>

[<span data-ttu-id="7f6cb-113">GetReminders</span><span class="sxs-lookup"><span data-stu-id="7f6cb-113">GetReminders</span></span>](getreminders.md)
  
## <a name="text-value"></a><span data-ttu-id="7f6cb-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7f6cb-114">Text value</span></span>

<span data-ttu-id="7f6cb-115">**BeginTime**要素のテキスト値は最初のアイテムのアラームの時刻用です。</span><span class="sxs-lookup"><span data-stu-id="7f6cb-115">The text value of the **BeginTime** element is the beginning time of the item the reminder is for.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="7f6cb-116">備考</span><span class="sxs-lookup"><span data-stu-id="7f6cb-116">Remarks</span></span>

<span data-ttu-id="7f6cb-117">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="7f6cb-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7f6cb-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7f6cb-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7f6cb-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="7f6cb-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7f6cb-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="7f6cb-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7f6cb-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7f6cb-121">Schema Name</span></span>  <br/> |<span data-ttu-id="7f6cb-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="7f6cb-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7f6cb-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7f6cb-123">Validation File</span></span>  <br/> |<span data-ttu-id="7f6cb-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7f6cb-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7f6cb-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7f6cb-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="7f6cb-126">False</span><span class="sxs-lookup"><span data-stu-id="7f6cb-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7f6cb-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="7f6cb-127">See also</span></span>



[<span data-ttu-id="7f6cb-128">GetReminders</span><span class="sxs-lookup"><span data-stu-id="7f6cb-128">GetReminders</span></span>](getreminders.md)


- [<span data-ttu-id="7f6cb-129">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="7f6cb-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

