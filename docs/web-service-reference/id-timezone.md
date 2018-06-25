---
title: Id (タイムゾーン)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Id
api_type:
- schema
ms.assetid: 4c7350b4-ffa1-4e7d-9433-80b4383bd0d2
description: Id 要素は、単一のタイム ゾーン定義を識別します。
ms.openlocfilehash: 4f2e18ca8a582a930cce9e0565821d9732daf555
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831854"
---
# <a name="id-timezone"></a><span data-ttu-id="5bc09-103">Id (タイムゾーン)</span><span class="sxs-lookup"><span data-stu-id="5bc09-103">Id (TimeZone)</span></span>

<span data-ttu-id="5bc09-104">**Id**要素は、単一のタイム ゾーン定義を識別します。</span><span class="sxs-lookup"><span data-stu-id="5bc09-104">The **Id** element identifies a single time zone definition.</span></span> 
  
```xml
<Id>...</Id>
```

 <span data-ttu-id="5bc09-105">**string**</span><span class="sxs-lookup"><span data-stu-id="5bc09-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5bc09-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5bc09-106">Attributes and elements</span></span>

<span data-ttu-id="5bc09-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5bc09-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5bc09-108">属性</span><span class="sxs-lookup"><span data-stu-id="5bc09-108">Attributes</span></span>

<span data-ttu-id="5bc09-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5bc09-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5bc09-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5bc09-110">Child elements</span></span>

<span data-ttu-id="5bc09-111">なし。</span><span class="sxs-lookup"><span data-stu-id="5bc09-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5bc09-112">親要素</span><span class="sxs-lookup"><span data-stu-id="5bc09-112">Parent elements</span></span>

|<span data-ttu-id="5bc09-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="5bc09-113">**Element**</span></span>|<span data-ttu-id="5bc09-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="5bc09-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5bc09-115">Id</span><span class="sxs-lookup"><span data-stu-id="5bc09-115">Ids</span></span>](ids.md) <br/> |<span data-ttu-id="5bc09-116">タイム ゾーン定義の識別子の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5bc09-116">Contains an array of time zone definition identifiers.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5bc09-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="5bc09-117">Text value</span></span>

<span data-ttu-id="5bc09-118">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="5bc09-118">A text value is required.</span></span> <span data-ttu-id="5bc09-119">テキスト値は、タイム ゾーン定義の一意の識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="5bc09-119">The text value represents the unique identifier for time zone definition.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5bc09-120">備考</span><span class="sxs-lookup"><span data-stu-id="5bc09-120">Remarks</span></span>

<span data-ttu-id="5bc09-121">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="5bc09-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5bc09-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="5bc09-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5bc09-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="5bc09-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5bc09-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5bc09-124">Schema Name</span></span>  <br/> |<span data-ttu-id="5bc09-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="5bc09-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="5bc09-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5bc09-126">Validation File</span></span>  <br/> |<span data-ttu-id="5bc09-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5bc09-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5bc09-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5bc09-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="5bc09-129">False</span><span class="sxs-lookup"><span data-stu-id="5bc09-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5bc09-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="5bc09-130">See also</span></span>



- [<span data-ttu-id="5bc09-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="5bc09-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

