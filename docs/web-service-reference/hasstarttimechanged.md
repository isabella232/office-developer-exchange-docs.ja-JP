---
title: HasStartTimeChanged
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 04a6968d-7fb5-47ee-b66e-dc99c35dbb63
description: HasStartTimeChanged 要素は、会議の開始時刻が変更されたかどうかを指定します。
ms.openlocfilehash: 2096084f4ec8848a63d10e0e80fdc7a37e473cd8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831809"
---
# <a name="hasstarttimechanged"></a><span data-ttu-id="d6633-103">HasStartTimeChanged</span><span class="sxs-lookup"><span data-stu-id="d6633-103">HasStartTimeChanged</span></span>

<span data-ttu-id="d6633-104">**HasStartTimeChanged**要素は、会議の開始時刻が変更されたかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="d6633-104">The **HasStartTimeChanged** element specifies whether the start time for a meeting has changed.</span></span> 
  
```XML
<HasStartTimeChanged> true | false </HasStartTimeChanged>
```

 <span data-ttu-id="d6633-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="d6633-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d6633-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d6633-106">Attributes and elements</span></span>

<span data-ttu-id="d6633-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d6633-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d6633-108">属性</span><span class="sxs-lookup"><span data-stu-id="d6633-108">Attributes</span></span>

<span data-ttu-id="d6633-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d6633-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d6633-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d6633-110">Child elements</span></span>

<span data-ttu-id="d6633-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d6633-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d6633-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d6633-112">Parent elements</span></span>

|<span data-ttu-id="d6633-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="d6633-113">**Element**</span></span>|<span data-ttu-id="d6633-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="d6633-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d6633-115">ChangeHighlights</span><span class="sxs-lookup"><span data-stu-id="d6633-115">ChangeHighlights</span></span>](changehighlights.md) <br/> |<span data-ttu-id="d6633-116">会議の 2 つのバージョン間で変更内容を指定する要求メッセージ。</span><span class="sxs-lookup"><span data-stu-id="d6633-116">Specifies what has changed between two versions of a meeting request message.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d6633-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d6633-117">Text value</span></span>

<span data-ttu-id="d6633-118">の**場合は true** 、 **HasStartTimeChanged**要素のテキスト値は、会議の開始時刻が変更されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="d6633-118">A text value of **true** for the **HasStartTimeChanged** element indicates that the start time for a meeting has changed.</span></span> <span data-ttu-id="d6633-119">**False**の値を開始時刻が変更されないことを示します。</span><span class="sxs-lookup"><span data-stu-id="d6633-119">A value of **false** indicates that the start time has not changed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d6633-120">備考</span><span class="sxs-lookup"><span data-stu-id="d6633-120">Remarks</span></span>

<span data-ttu-id="d6633-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d6633-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d6633-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d6633-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d6633-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="d6633-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d6633-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="d6633-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d6633-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d6633-125">Schema Name</span></span>  <br/> |<span data-ttu-id="d6633-126">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="d6633-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="d6633-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d6633-127">Validation File</span></span>  <br/> |<span data-ttu-id="d6633-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="d6633-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="d6633-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d6633-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="d6633-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="d6633-130">See also</span></span>



- [<span data-ttu-id="d6633-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d6633-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

