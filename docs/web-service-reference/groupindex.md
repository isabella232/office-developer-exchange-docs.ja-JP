---
title: GroupIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupIndex
api_type:
- schema
ms.assetid: 7a596ff7-6cc3-4626-a52c-538a92202337
description: GroupIndex 要素は、FindItem 操作の呼び出し内の項目の現在のグループのアイテムをグループ化するために使用されるプロパティ値を表します。
ms.openlocfilehash: 8b23f5142a15c099c30209ea48cd04f4af4e8c6a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831762"
---
# <a name="groupindex"></a><span data-ttu-id="1c05f-103">GroupIndex</span><span class="sxs-lookup"><span data-stu-id="1c05f-103">GroupIndex</span></span>

<span data-ttu-id="1c05f-104">**GroupIndex**要素は、 [FindItem 操作](finditem-operation.md)の呼び出し内の項目の現在のグループのアイテムをグループ化するために使用されるプロパティ値を表します。</span><span class="sxs-lookup"><span data-stu-id="1c05f-104">The **GroupIndex** element represents the property value that is used to group items for the current group of items in a [FindItem operation](finditem-operation.md) call.</span></span> 
  
[<span data-ttu-id="1c05f-105">FindItemResponse</span><span class="sxs-lookup"><span data-stu-id="1c05f-105">FindItemResponse</span></span>](finditemresponse.md)
  
[<span data-ttu-id="1c05f-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="1c05f-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="1c05f-107">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="1c05f-107">FindItemResponseMessage</span></span>](finditemresponsemessage.md)
  
[<span data-ttu-id="1c05f-108">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="1c05f-108">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md)
  
[<span data-ttu-id="1c05f-109">グループ</span><span class="sxs-lookup"><span data-stu-id="1c05f-109">Groups</span></span>](groups.md)
  
[<span data-ttu-id="1c05f-110">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="1c05f-110">GroupedItems</span></span>](groupeditems.md)
  
[<span data-ttu-id="1c05f-111">GroupIndex</span><span class="sxs-lookup"><span data-stu-id="1c05f-111">GroupIndex</span></span>](groupindex.md)
  
```xml
<GroupIndex/>
```

 <span data-ttu-id="1c05f-112">**string**</span><span class="sxs-lookup"><span data-stu-id="1c05f-112">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1c05f-113">属性および要素</span><span class="sxs-lookup"><span data-stu-id="1c05f-113">Attributes and elements</span></span>

<span data-ttu-id="1c05f-114">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1c05f-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1c05f-115">属性</span><span class="sxs-lookup"><span data-stu-id="1c05f-115">Attributes</span></span>

<span data-ttu-id="1c05f-116">なし。</span><span class="sxs-lookup"><span data-stu-id="1c05f-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1c05f-117">子要素</span><span class="sxs-lookup"><span data-stu-id="1c05f-117">Child elements</span></span>

<span data-ttu-id="1c05f-118">なし。</span><span class="sxs-lookup"><span data-stu-id="1c05f-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1c05f-119">親要素</span><span class="sxs-lookup"><span data-stu-id="1c05f-119">Parent elements</span></span>

|<span data-ttu-id="1c05f-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="1c05f-120">**Element**</span></span>|<span data-ttu-id="1c05f-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="1c05f-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1c05f-122">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="1c05f-122">GroupedItems</span></span>](groupeditems.md) <br/> |<span data-ttu-id="1c05f-123">グループ化された[FindItem 操作](finditem-operation.md)の結果であるアイテムのコレクションを呼び出します。</span><span class="sxs-lookup"><span data-stu-id="1c05f-123">Represents a collection of items that are the result of a grouped [FindItem operation](finditem-operation.md) call.</span></span>  <br/> <span data-ttu-id="1c05f-124">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="1c05f-124">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItemResponse/ResponseMessages/FindItemResponseMessage/RootFolder/Groups/GroupedItems[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1c05f-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1c05f-125">Text value</span></span>

<span data-ttu-id="1c05f-126">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="1c05f-126">A text value is required.</span></span> <span data-ttu-id="1c05f-127">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="1c05f-127">This property is read-only.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1c05f-128">備考</span><span class="sxs-lookup"><span data-stu-id="1c05f-128">Remarks</span></span>

<span data-ttu-id="1c05f-129">[FindItem 操作](finditem-operation.md)の応答にこの要素にのみ発生します。</span><span class="sxs-lookup"><span data-stu-id="1c05f-129">This element only occurs in a [FindItem operation](finditem-operation.md) response.</span></span> 
  
<span data-ttu-id="1c05f-130">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="1c05f-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1c05f-131">要素情報</span><span class="sxs-lookup"><span data-stu-id="1c05f-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1c05f-132">名前空間</span><span class="sxs-lookup"><span data-stu-id="1c05f-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1c05f-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1c05f-133">Schema name</span></span>  <br/> |<span data-ttu-id="1c05f-134">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="1c05f-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="1c05f-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1c05f-135">Validation file</span></span>  <br/> |<span data-ttu-id="1c05f-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1c05f-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1c05f-137">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="1c05f-137">Can be empty</span></span>  <br/> |<span data-ttu-id="1c05f-138">False</span><span class="sxs-lookup"><span data-stu-id="1c05f-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1c05f-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="1c05f-139">See also</span></span>



<span data-ttu-id="1c05f-140">
  [FindItem 操作](finditem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="1c05f-140">[FindItem operation](finditem-operation.md)</span></span>


[<span data-ttu-id="1c05f-141">項目を検索します。</span><span class="sxs-lookup"><span data-stu-id="1c05f-141">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

