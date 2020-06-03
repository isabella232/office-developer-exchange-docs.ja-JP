---
title: ActionUrl
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9697f2e5-a5f7-471a-a052-ae79e06eb09d
description: ActionUrl 要素は、AppStatus 要素によって示された問題を修正するために、ユーザーが移動する必要のある URL を識別します。
ms.openlocfilehash: 2335595b4be6452f41c25f15d359e6939609c9b9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529673"
---
# <a name="actionurl"></a><span data-ttu-id="9d228-103">ActionUrl</span><span class="sxs-lookup"><span data-stu-id="9d228-103">ActionUrl</span></span>

<span data-ttu-id="9d228-104">**Actionurl**要素は、 [appstatus](appstatus-ex15websvcsotherref.md)要素によって示された問題を修正するために、ユーザーが移動する必要のある url を識別します。</span><span class="sxs-lookup"><span data-stu-id="9d228-104">The **ActionUrl** element identifies the URL that the user should navigate to, in order to fix an issue indicated by the [AppStatus](appstatus-ex15websvcsotherref.md) element.</span></span> 
  
```XML
<ActionUrl/>
```

 <span data-ttu-id="9d228-105">**string**</span><span class="sxs-lookup"><span data-stu-id="9d228-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9d228-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9d228-106">Attributes and elements</span></span>

<span data-ttu-id="9d228-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9d228-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9d228-108">属性</span><span class="sxs-lookup"><span data-stu-id="9d228-108">Attributes</span></span>

<span data-ttu-id="9d228-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9d228-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9d228-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9d228-110">Child elements</span></span>

<span data-ttu-id="9d228-111">なし。</span><span class="sxs-lookup"><span data-stu-id="9d228-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9d228-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9d228-112">Parent elements</span></span>

[<span data-ttu-id="9d228-113">メタデータ</span><span class="sxs-lookup"><span data-stu-id="9d228-113">Metadata</span></span>](metadata-ex15websvcsotherref.md)
  
## <a name="text-value"></a><span data-ttu-id="9d228-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9d228-114">Text value</span></span>

<span data-ttu-id="9d228-115">**Actionurl**要素のテキスト値は、 **appstatus**要素によって示された問題を修正するために、ユーザーが移動する必要のある url を示します。</span><span class="sxs-lookup"><span data-stu-id="9d228-115">The text value of the **ActionUrl** element identifies the URL that the user should navigate to, in order to fix an issue indicated by the **AppStatus** element.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="9d228-116">注釈</span><span class="sxs-lookup"><span data-stu-id="9d228-116">Remarks</span></span>

<span data-ttu-id="9d228-117">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9d228-117">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="9d228-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9d228-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9d228-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9d228-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9d228-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="9d228-120">Namespace</span></span>  <br/> | https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9d228-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9d228-121">Schema Name</span></span>  <br/> |<span data-ttu-id="9d228-122">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="9d228-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="9d228-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9d228-123">Validation File</span></span>  <br/> |<span data-ttu-id="9d228-124">該当なし</span><span class="sxs-lookup"><span data-stu-id="9d228-124">Not applicable</span></span>  <br/> |
|<span data-ttu-id="9d228-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9d228-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="9d228-126">正しくない</span><span class="sxs-lookup"><span data-stu-id="9d228-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9d228-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="9d228-127">See also</span></span>

- [<span data-ttu-id="9d228-128">メタデータ</span><span class="sxs-lookup"><span data-stu-id="9d228-128">Metadata</span></span>](metadata-ex15websvcsotherref.md)
- [<span data-ttu-id="9d228-129">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="9d228-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

