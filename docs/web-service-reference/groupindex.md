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
description: GroupIndex 要素は、FindItem 操作呼び出しで現在のアイテムグループのアイテムをグループ化するために使用されるプロパティの値を表します。
ms.openlocfilehash: 05f303be92885a15dddf85c85251af04910d835c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530269"
---
# <a name="groupindex"></a><span data-ttu-id="06a4e-103">GroupIndex</span><span class="sxs-lookup"><span data-stu-id="06a4e-103">GroupIndex</span></span>

<span data-ttu-id="06a4e-104">**Groupindex**要素は、 [FindItem 操作](finditem-operation.md)呼び出しで現在のアイテムグループのアイテムをグループ化するために使用されるプロパティの値を表します。</span><span class="sxs-lookup"><span data-stu-id="06a4e-104">The **GroupIndex** element represents the property value that is used to group items for the current group of items in a [FindItem operation](finditem-operation.md) call.</span></span> 
  
[<span data-ttu-id="06a4e-105">FindItemResponse</span><span class="sxs-lookup"><span data-stu-id="06a4e-105">FindItemResponse</span></span>](finditemresponse.md)
  
[<span data-ttu-id="06a4e-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="06a4e-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="06a4e-107">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="06a4e-107">FindItemResponseMessage</span></span>](finditemresponsemessage.md)
  
[<span data-ttu-id="06a4e-108">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="06a4e-108">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md)
  
[<span data-ttu-id="06a4e-109">Groups</span><span class="sxs-lookup"><span data-stu-id="06a4e-109">Groups</span></span>](groups.md)
  
[<span data-ttu-id="06a4e-110">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="06a4e-110">GroupedItems</span></span>](groupeditems.md)
  
[<span data-ttu-id="06a4e-111">GroupIndex</span><span class="sxs-lookup"><span data-stu-id="06a4e-111">GroupIndex</span></span>](groupindex.md)
  
```xml
<GroupIndex/>
```

 <span data-ttu-id="06a4e-112">**string**</span><span class="sxs-lookup"><span data-stu-id="06a4e-112">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="06a4e-113">属性と要素</span><span class="sxs-lookup"><span data-stu-id="06a4e-113">Attributes and elements</span></span>

<span data-ttu-id="06a4e-114">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="06a4e-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="06a4e-115">属性</span><span class="sxs-lookup"><span data-stu-id="06a4e-115">Attributes</span></span>

<span data-ttu-id="06a4e-116">なし。</span><span class="sxs-lookup"><span data-stu-id="06a4e-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="06a4e-117">子要素</span><span class="sxs-lookup"><span data-stu-id="06a4e-117">Child elements</span></span>

<span data-ttu-id="06a4e-118">なし。</span><span class="sxs-lookup"><span data-stu-id="06a4e-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="06a4e-119">親要素</span><span class="sxs-lookup"><span data-stu-id="06a4e-119">Parent elements</span></span>

|<span data-ttu-id="06a4e-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="06a4e-120">**Element**</span></span>|<span data-ttu-id="06a4e-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="06a4e-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="06a4e-122">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="06a4e-122">GroupedItems</span></span>](groupeditems.md) <br/> |<span data-ttu-id="06a4e-123">グループ化された[FindItem 操作](finditem-operation.md)呼び出しの結果であるアイテムのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="06a4e-123">Represents a collection of items that are the result of a grouped [FindItem operation](finditem-operation.md) call.</span></span>  <br/> <span data-ttu-id="06a4e-124">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="06a4e-124">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItemResponse/ResponseMessages/FindItemResponseMessage/RootFolder/Groups/GroupedItems[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="06a4e-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="06a4e-125">Text value</span></span>

<span data-ttu-id="06a4e-126">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="06a4e-126">A text value is required.</span></span> <span data-ttu-id="06a4e-127">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="06a4e-127">This property is read-only.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="06a4e-128">注釈</span><span class="sxs-lookup"><span data-stu-id="06a4e-128">Remarks</span></span>

<span data-ttu-id="06a4e-129">この要素は、 [FindItem 操作](finditem-operation.md)応答でのみ発生します。</span><span class="sxs-lookup"><span data-stu-id="06a4e-129">This element only occurs in a [FindItem operation](finditem-operation.md) response.</span></span> 
  
<span data-ttu-id="06a4e-130">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="06a4e-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="06a4e-131">要素の情報</span><span class="sxs-lookup"><span data-stu-id="06a4e-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="06a4e-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="06a4e-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="06a4e-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="06a4e-133">Schema name</span></span>  <br/> |<span data-ttu-id="06a4e-134">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="06a4e-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="06a4e-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="06a4e-135">Validation file</span></span>  <br/> |<span data-ttu-id="06a4e-136">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="06a4e-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="06a4e-137">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="06a4e-137">Can be empty</span></span>  <br/> |<span data-ttu-id="06a4e-138">正しくない</span><span class="sxs-lookup"><span data-stu-id="06a4e-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="06a4e-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="06a4e-139">See also</span></span>



[<span data-ttu-id="06a4e-140">FindItem 操作</span><span class="sxs-lookup"><span data-stu-id="06a4e-140">FindItem operation</span></span>](finditem-operation.md)


[<span data-ttu-id="06a4e-141">アイテムの検索</span><span class="sxs-lookup"><span data-stu-id="06a4e-141">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

