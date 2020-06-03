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
ms.openlocfilehash: 1355917005d956d05064bfc095055fb72aa16c57
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462746"
---
# <a name="hasstarttimechanged"></a><span data-ttu-id="e9ad1-103">HasStartTimeChanged</span><span class="sxs-lookup"><span data-stu-id="e9ad1-103">HasStartTimeChanged</span></span>

<span data-ttu-id="e9ad1-104">**Hasstarttimechanged**要素は、会議の開始時刻が変更されたかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e9ad1-104">The **HasStartTimeChanged** element specifies whether the start time for a meeting has changed.</span></span> 
  
```XML
<HasStartTimeChanged> true | false </HasStartTimeChanged>
```

 <span data-ttu-id="e9ad1-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="e9ad1-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e9ad1-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e9ad1-106">Attributes and elements</span></span>

<span data-ttu-id="e9ad1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e9ad1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e9ad1-108">属性</span><span class="sxs-lookup"><span data-stu-id="e9ad1-108">Attributes</span></span>

<span data-ttu-id="e9ad1-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e9ad1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e9ad1-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e9ad1-110">Child elements</span></span>

<span data-ttu-id="e9ad1-111">なし。</span><span class="sxs-lookup"><span data-stu-id="e9ad1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e9ad1-112">親要素</span><span class="sxs-lookup"><span data-stu-id="e9ad1-112">Parent elements</span></span>

|<span data-ttu-id="e9ad1-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="e9ad1-113">**Element**</span></span>|<span data-ttu-id="e9ad1-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="e9ad1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9ad1-115">ChangeHighlights 強調表示</span><span class="sxs-lookup"><span data-stu-id="e9ad1-115">ChangeHighlights</span></span>](changehighlights.md) <br/> |<span data-ttu-id="e9ad1-116">2つのバージョンの会議出席依頼メッセージの間で変更されたものを指定します。</span><span class="sxs-lookup"><span data-stu-id="e9ad1-116">Specifies what has changed between two versions of a meeting request message.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e9ad1-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e9ad1-117">Text value</span></span>

<span data-ttu-id="e9ad1-118">**Hasstarttimechanged**要素のテキスト値が**true の場合**は、会議の開始時刻が変更されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="e9ad1-118">A text value of **true** for the **HasStartTimeChanged** element indicates that the start time for a meeting has changed.</span></span> <span data-ttu-id="e9ad1-119">値が**false**の場合は、開始時刻が変更されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="e9ad1-119">A value of **false** indicates that the start time has not changed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e9ad1-120">注釈</span><span class="sxs-lookup"><span data-stu-id="e9ad1-120">Remarks</span></span>

<span data-ttu-id="e9ad1-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e9ad1-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e9ad1-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e9ad1-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e9ad1-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e9ad1-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e9ad1-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="e9ad1-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e9ad1-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e9ad1-125">Schema Name</span></span>  <br/> |<span data-ttu-id="e9ad1-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="e9ad1-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="e9ad1-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e9ad1-127">Validation File</span></span>  <br/> |<span data-ttu-id="e9ad1-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="e9ad1-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="e9ad1-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e9ad1-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e9ad1-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="e9ad1-130">See also</span></span>



- [<span data-ttu-id="e9ad1-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="e9ad1-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

