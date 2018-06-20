---
title: HasLocationChanged
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5fd465b4-6070-4cd0-9ac3-ed9d2bfd5951
description: HasLocationChanged 要素は、会議の場所のプロパティが変更されたかどうかを指定します。
ms.openlocfilehash: dbb811b93149be0bb43fbb2f579a5086a396e401
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831804"
---
# <a name="haslocationchanged"></a><span data-ttu-id="d53b8-103">HasLocationChanged</span><span class="sxs-lookup"><span data-stu-id="d53b8-103">HasLocationChanged</span></span>

<span data-ttu-id="d53b8-104">**HasLocationChanged**要素は、会議の場所のプロパティが変更されたかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="d53b8-104">The **HasLocationChanged** element specifies whether the location property of a meeting has changed.</span></span> 
  
```XML
<HasLocationChanged> true | false </HasLocationChanged>
```

 <span data-ttu-id="d53b8-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="d53b8-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d53b8-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d53b8-106">Attributes and elements</span></span>

<span data-ttu-id="d53b8-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d53b8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d53b8-108">属性</span><span class="sxs-lookup"><span data-stu-id="d53b8-108">Attributes</span></span>

<span data-ttu-id="d53b8-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d53b8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d53b8-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d53b8-110">Child elements</span></span>

<span data-ttu-id="d53b8-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d53b8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d53b8-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d53b8-112">Parent elements</span></span>

|<span data-ttu-id="d53b8-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="d53b8-113">**Element**</span></span>|<span data-ttu-id="d53b8-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="d53b8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d53b8-115">ChangeHighlights</span><span class="sxs-lookup"><span data-stu-id="d53b8-115">ChangeHighlights</span></span>](changehighlights.md) <br/> |<span data-ttu-id="d53b8-116">会議の 2 つのバージョン間で変更内容を指定する要求メッセージ。</span><span class="sxs-lookup"><span data-stu-id="d53b8-116">Specifies what has changed between two versions of a meeting request message.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d53b8-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d53b8-117">Text value</span></span>

<span data-ttu-id="d53b8-118">の**場合は true** 、 **HasLocationChanged**要素のテキスト値は、会議の場所のプロパティが変更されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="d53b8-118">A text value of **true** for the **HasLocationChanged** element indicates that the location property of a meeting has changed.</span></span> <span data-ttu-id="d53b8-119">値**false**は、会議の場所のプロパティが変更されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="d53b8-119">A value **false** indicates that the location property of a meeting has not changed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d53b8-120">備考</span><span class="sxs-lookup"><span data-stu-id="d53b8-120">Remarks</span></span>

<span data-ttu-id="d53b8-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d53b8-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d53b8-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d53b8-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d53b8-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="d53b8-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d53b8-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="d53b8-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d53b8-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d53b8-125">Schema Name</span></span>  <br/> |<span data-ttu-id="d53b8-126">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="d53b8-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="d53b8-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d53b8-127">Validation File</span></span>  <br/> |<span data-ttu-id="d53b8-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="d53b8-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="d53b8-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d53b8-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="d53b8-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="d53b8-130">See also</span></span>



- [<span data-ttu-id="d53b8-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d53b8-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

