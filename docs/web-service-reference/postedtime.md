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
description: PostedTime 要素は、PostItem が投稿された時刻を表します。 この要素は値の取得のみ可能です。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 5fc670bfee97a46700bc4442d489696a4489f88a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459196"
---
# <a name="postedtime"></a><span data-ttu-id="09cc0-105">PostedTime</span><span class="sxs-lookup"><span data-stu-id="09cc0-105">PostedTime</span></span>

<span data-ttu-id="09cc0-106">**PostedTime**要素は、 [postitem](postitem.md)が投稿された時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="09cc0-106">The **PostedTime** element represents the time at which a [PostItem](postitem.md) was posted.</span></span> <span data-ttu-id="09cc0-107">この要素は値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="09cc0-107">This element is read-only.</span></span> <span data-ttu-id="09cc0-108">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="09cc0-108">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<PostedTime/>
```

 <span data-ttu-id="09cc0-109">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="09cc0-109">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="09cc0-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="09cc0-110">Attributes and elements</span></span>

<span data-ttu-id="09cc0-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="09cc0-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="09cc0-112">属性</span><span class="sxs-lookup"><span data-stu-id="09cc0-112">Attributes</span></span>

<span data-ttu-id="09cc0-113">なし。</span><span class="sxs-lookup"><span data-stu-id="09cc0-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="09cc0-114">子要素</span><span class="sxs-lookup"><span data-stu-id="09cc0-114">Child elements</span></span>

<span data-ttu-id="09cc0-115">なし。</span><span class="sxs-lookup"><span data-stu-id="09cc0-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="09cc0-116">親要素</span><span class="sxs-lookup"><span data-stu-id="09cc0-116">Parent elements</span></span>

|<span data-ttu-id="09cc0-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="09cc0-117">**Element**</span></span>|<span data-ttu-id="09cc0-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="09cc0-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="09cc0-119">PostItem</span><span class="sxs-lookup"><span data-stu-id="09cc0-119">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="09cc0-120">Exchange ストアの PostItem を表します。</span><span class="sxs-lookup"><span data-stu-id="09cc0-120">Represents a PostItem in the Exchange store.</span></span> <span data-ttu-id="09cc0-121">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="09cc0-121">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="09cc0-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="09cc0-122">Text value</span></span>

<span data-ttu-id="09cc0-123">テキスト値は、 **Postitem**が投稿された日時を表す dateTime です。</span><span class="sxs-lookup"><span data-stu-id="09cc0-123">The text value is a dateTime that represents when a **PostItem** was posted.</span></span> <span data-ttu-id="09cc0-124">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="09cc0-124">This property is read-only.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="09cc0-125">注釈</span><span class="sxs-lookup"><span data-stu-id="09cc0-125">Remarks</span></span>

<span data-ttu-id="09cc0-126">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="09cc0-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="09cc0-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="09cc0-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="09cc0-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="09cc0-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="09cc0-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="09cc0-129">Schema Name</span></span>  <br/> |<span data-ttu-id="09cc0-130">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="09cc0-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="09cc0-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="09cc0-131">Validation File</span></span>  <br/> |<span data-ttu-id="09cc0-132">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="09cc0-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="09cc0-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="09cc0-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="09cc0-134">正しくない</span><span class="sxs-lookup"><span data-stu-id="09cc0-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="09cc0-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="09cc0-135">See also</span></span>



- [<span data-ttu-id="09cc0-136">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="09cc0-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

