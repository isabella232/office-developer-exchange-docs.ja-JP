---
title: PostedTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PostedTime
api_type:
- schema
ms.assetid: e8b3813c-fc7e-4674-a4c6-6818c13d2bcf
description: PostedTime 要素は、PostItem が転記された時間を表します。 この要素は、読み取り専用です。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 8280fc26c534b280d0f30f663b6cc3a3958036c5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832860"
---
# <a name="postedtime"></a><span data-ttu-id="bc651-105">PostedTime</span><span class="sxs-lookup"><span data-stu-id="bc651-105">PostedTime</span></span>

<span data-ttu-id="bc651-106">**PostedTime**要素は、 [PostItem](postitem.md)が転記された時間を表します。</span><span class="sxs-lookup"><span data-stu-id="bc651-106">The **PostedTime** element represents the time at which a [PostItem](postitem.md) was posted.</span></span> <span data-ttu-id="bc651-107">この要素は、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="bc651-107">This element is read-only.</span></span> <span data-ttu-id="bc651-108">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="bc651-108">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<PostedTime/>
```

 <span data-ttu-id="bc651-109">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="bc651-109">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bc651-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="bc651-110">Attributes and elements</span></span>

<span data-ttu-id="bc651-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="bc651-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bc651-112">属性</span><span class="sxs-lookup"><span data-stu-id="bc651-112">Attributes</span></span>

<span data-ttu-id="bc651-113">なし。</span><span class="sxs-lookup"><span data-stu-id="bc651-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bc651-114">子要素</span><span class="sxs-lookup"><span data-stu-id="bc651-114">Child elements</span></span>

<span data-ttu-id="bc651-115">なし。</span><span class="sxs-lookup"><span data-stu-id="bc651-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bc651-116">親要素</span><span class="sxs-lookup"><span data-stu-id="bc651-116">Parent elements</span></span>

|<span data-ttu-id="bc651-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="bc651-117">**Element**</span></span>|<span data-ttu-id="bc651-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="bc651-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bc651-119">PostItem</span><span class="sxs-lookup"><span data-stu-id="bc651-119">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="bc651-120">Exchange ストアで、PostItem を表します。</span><span class="sxs-lookup"><span data-stu-id="bc651-120">Represents a PostItem in the Exchange store.</span></span> <span data-ttu-id="bc651-121">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="bc651-121">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bc651-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="bc651-122">Text value</span></span>

<span data-ttu-id="bc651-123">テキスト値では、 **PostItem**がポストされたときを表す dateTime です。</span><span class="sxs-lookup"><span data-stu-id="bc651-123">The text value is a dateTime that represents when a **PostItem** was posted.</span></span> <span data-ttu-id="bc651-124">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="bc651-124">This property is read-only.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="bc651-125">備考</span><span class="sxs-lookup"><span data-stu-id="bc651-125">Remarks</span></span>

<span data-ttu-id="bc651-126">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="bc651-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bc651-127">要素情報</span><span class="sxs-lookup"><span data-stu-id="bc651-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bc651-128">名前空間</span><span class="sxs-lookup"><span data-stu-id="bc651-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bc651-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="bc651-129">Schema Name</span></span>  <br/> |<span data-ttu-id="bc651-130">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="bc651-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="bc651-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="bc651-131">Validation File</span></span>  <br/> |<span data-ttu-id="bc651-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bc651-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bc651-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="bc651-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="bc651-134">False</span><span class="sxs-lookup"><span data-stu-id="bc651-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bc651-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="bc651-135">See also</span></span>



- [<span data-ttu-id="bc651-136">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="bc651-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

