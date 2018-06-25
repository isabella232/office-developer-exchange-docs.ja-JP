---
title: ActionUrl
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9697f2e5-a5f7-471a-a052-ae79e06eb09d
description: ActionUrl 要素は、AppStatus 要素で示された問題を解決するために、ユーザーが移動する必要がある URL を識別します。
ms.openlocfilehash: b138797aa8f4e277d94e85e2dd13c0d4c6afaa51
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759271"
---
# <a name="actionurl"></a><span data-ttu-id="4b103-103">ActionUrl</span><span class="sxs-lookup"><span data-stu-id="4b103-103">ActionUrl</span></span>

<span data-ttu-id="4b103-104">**ActionUrl**要素は、 [AppStatus](appstatus-ex15websvcsotherref.md)要素で示された問題を解決するために、ユーザーが移動する必要がある URL を識別します。</span><span class="sxs-lookup"><span data-stu-id="4b103-104">The **ActionUrl** element identifies the URL that the user should navigate to, in order to fix an issue indicated by the [AppStatus](appstatus-ex15websvcsotherref.md) element.</span></span> 
  
```XML
<ActionUrl/>
```

 <span data-ttu-id="4b103-105">**string**</span><span class="sxs-lookup"><span data-stu-id="4b103-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4b103-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4b103-106">Attributes and elements</span></span>

<span data-ttu-id="4b103-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4b103-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4b103-108">属性</span><span class="sxs-lookup"><span data-stu-id="4b103-108">Attributes</span></span>

<span data-ttu-id="4b103-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4b103-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4b103-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4b103-110">Child elements</span></span>

<span data-ttu-id="4b103-111">なし。</span><span class="sxs-lookup"><span data-stu-id="4b103-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4b103-112">親要素</span><span class="sxs-lookup"><span data-stu-id="4b103-112">Parent elements</span></span>

[<span data-ttu-id="4b103-113">メタデータ</span><span class="sxs-lookup"><span data-stu-id="4b103-113">Metadata</span></span>](metadata-ex15websvcsotherref.md)
  
## <a name="text-value"></a><span data-ttu-id="4b103-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="4b103-114">Text value</span></span>

<span data-ttu-id="4b103-115">**ActionUrl**要素のテキスト値は、 **AppStatus**要素で示された問題を解決するために、ユーザーが移動する必要がある URL を識別します。</span><span class="sxs-lookup"><span data-stu-id="4b103-115">The text value of the **ActionUrl** element identifies the URL that the user should navigate to, in order to fix an issue indicated by the **AppStatus** element.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="4b103-116">備考</span><span class="sxs-lookup"><span data-stu-id="4b103-116">Remarks</span></span>

<span data-ttu-id="4b103-117">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="4b103-117">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="4b103-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="4b103-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4b103-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="4b103-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4b103-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="4b103-120">Namespace</span></span>  <br/> | http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4b103-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4b103-121">Schema Name</span></span>  <br/> |<span data-ttu-id="4b103-122">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="4b103-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="4b103-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4b103-123">Validation File</span></span>  <br/> |<span data-ttu-id="4b103-124">該当しない</span><span class="sxs-lookup"><span data-stu-id="4b103-124">Not applicable</span></span>  <br/> |
|<span data-ttu-id="4b103-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4b103-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="4b103-126">False</span><span class="sxs-lookup"><span data-stu-id="4b103-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4b103-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="4b103-127">See also</span></span>

- [<span data-ttu-id="4b103-128">メタデータ</span><span class="sxs-lookup"><span data-stu-id="4b103-128">Metadata</span></span>](metadata-ex15websvcsotherref.md)
- [<span data-ttu-id="4b103-129">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="4b103-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

