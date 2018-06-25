---
title: HasEndTimeChanged
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a0eb444d-8e2e-478b-b785-2b9787ffb226
description: HasEndTimeChanged 要素は、会議の終了時刻が変更されたかどうかを指定します。
ms.openlocfilehash: 046bb302d6f7052c6f1757ce393583b305311e2f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831805"
---
# <a name="hasendtimechanged"></a><span data-ttu-id="d64f3-103">HasEndTimeChanged</span><span class="sxs-lookup"><span data-stu-id="d64f3-103">HasEndTimeChanged</span></span>

<span data-ttu-id="d64f3-104">**HasEndTimeChanged**要素は、会議の終了時刻が変更されたかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="d64f3-104">The **HasEndTimeChanged** element specifies whether the end time for a meeting has changed.</span></span> 
  
```XML
<HasEndTimeChanged>true | false</HasEndTimeChanged>
```

 <span data-ttu-id="d64f3-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="d64f3-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d64f3-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d64f3-106">Attributes and elements</span></span>

<span data-ttu-id="d64f3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d64f3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d64f3-108">属性</span><span class="sxs-lookup"><span data-stu-id="d64f3-108">Attributes</span></span>

<span data-ttu-id="d64f3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d64f3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d64f3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d64f3-110">Child elements</span></span>

<span data-ttu-id="d64f3-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d64f3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d64f3-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d64f3-112">Parent elements</span></span>

|<span data-ttu-id="d64f3-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="d64f3-113">**Element**</span></span>|<span data-ttu-id="d64f3-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="d64f3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d64f3-115">ChangeHighlights</span><span class="sxs-lookup"><span data-stu-id="d64f3-115">ChangeHighlights</span></span>](changehighlights.md) <br/> |<span data-ttu-id="d64f3-116">会議の 2 つのバージョン間で変更内容を指定する要求メッセージ。</span><span class="sxs-lookup"><span data-stu-id="d64f3-116">Specifies what has changed between two versions of a meeting request message.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d64f3-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d64f3-117">Text value</span></span>

<span data-ttu-id="d64f3-118">の**場合は true** 、 **HasEndTimeChanged**要素のテキスト値は、会議の終了時刻が変更されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="d64f3-118">A text value of **true** for the **HasEndTimeChanged** element indicates that the end time of a meeting has changed.</span></span> <span data-ttu-id="d64f3-119">**False**の値は、会議の終了時刻が変更されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="d64f3-119">A value of **false** indicates that the end time of a meeting has not changed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d64f3-120">備考</span><span class="sxs-lookup"><span data-stu-id="d64f3-120">Remarks</span></span>

<span data-ttu-id="d64f3-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d64f3-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d64f3-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d64f3-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d64f3-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="d64f3-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d64f3-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="d64f3-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d64f3-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d64f3-125">Schema Name</span></span>  <br/> |<span data-ttu-id="d64f3-126">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="d64f3-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="d64f3-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d64f3-127">Validation File</span></span>  <br/> |<span data-ttu-id="d64f3-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="d64f3-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="d64f3-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d64f3-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="d64f3-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="d64f3-130">See also</span></span>



- [<span data-ttu-id="d64f3-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d64f3-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

