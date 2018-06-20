---
title: OldItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OldItemId
api_type:
- schema
ms.assetid: fb57deee-9cc3-4730-9805-ff34f39e3ab7
description: OldItemId 要素には、コピーまたは移動された項目の一意の識別子が含まれています。
ms.openlocfilehash: ced7fc6891e0d1fde42a8cb9cad4f4e55493b5d1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832648"
---
# <a name="olditemid"></a><span data-ttu-id="3e558-103">OldItemId</span><span class="sxs-lookup"><span data-stu-id="3e558-103">OldItemId</span></span>

<span data-ttu-id="3e558-104">**OldItemId**要素には、コピーまたは移動された項目の一意の識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3e558-104">The **OldItemId** element contains the unique identifier of the item that was copied or moved.</span></span> 
  
```xml
<OldItemId Id="" ChangeKey=""/>
```

 <span data-ttu-id="3e558-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="3e558-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3e558-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="3e558-106">Attributes and elements</span></span>

<span data-ttu-id="3e558-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3e558-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3e558-108">属性</span><span class="sxs-lookup"><span data-stu-id="3e558-108">Attributes</span></span>

|<span data-ttu-id="3e558-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="3e558-109">**Attribute**</span></span>|<span data-ttu-id="3e558-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="3e558-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3e558-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="3e558-111">**Id**</span></span> <br/> |<span data-ttu-id="3e558-112">Exchange ストア内の項目を識別する文字列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3e558-112">Contains a string that identifies an item in the Exchange store.</span></span> <span data-ttu-id="3e558-113">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="3e558-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="3e558-114">**変更キー**</span><span class="sxs-lookup"><span data-stu-id="3e558-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="3e558-115">Id 属性によって識別される項目のバージョンを識別する文字列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3e558-115">Contains a string that identifies a version of an item that is identified by the Id attribute.</span></span> <span data-ttu-id="3e558-116">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="3e558-116">This attribute is optional.</span></span> <span data-ttu-id="3e558-117">アイテムの正しいバージョンを使用するかどうかを確認するには、この属性を使用します。</span><span class="sxs-lookup"><span data-stu-id="3e558-117">Use this attribute to make sure that the correct version of an item is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="3e558-118">子要素</span><span class="sxs-lookup"><span data-stu-id="3e558-118">Child elements</span></span>

<span data-ttu-id="3e558-119">なし。</span><span class="sxs-lookup"><span data-stu-id="3e558-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3e558-120">親要素</span><span class="sxs-lookup"><span data-stu-id="3e558-120">Parent elements</span></span>

|<span data-ttu-id="3e558-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="3e558-121">**Element**</span></span>|<span data-ttu-id="3e558-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="3e558-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3e558-123">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="3e558-123">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="3e558-124">アイテムまたはフォルダーのコピー先のイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="3e558-124">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="3e558-125">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="3e558-125">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="3e558-126">アイテムまたはフォルダーが 1 つの親フォルダー間で移動して別の親フォルダー イベントを表します。</span><span class="sxs-lookup"><span data-stu-id="3e558-126">Represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3e558-127">備考</span><span class="sxs-lookup"><span data-stu-id="3e558-127">Remarks</span></span>

<span data-ttu-id="3e558-128">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="3e558-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3e558-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="3e558-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3e558-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="3e558-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3e558-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3e558-131">Schema Name</span></span>  <br/> |<span data-ttu-id="3e558-132">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="3e558-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="3e558-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3e558-133">Validation File</span></span>  <br/> |<span data-ttu-id="3e558-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3e558-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3e558-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3e558-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="3e558-136">False</span><span class="sxs-lookup"><span data-stu-id="3e558-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3e558-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="3e558-137">See also</span></span>



[<span data-ttu-id="3e558-138">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="3e558-138">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="3e558-139">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="3e558-139">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="3e558-140">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="3e558-140">Unsubscribe operation</span></span>](unsubscribe-operation.md)


- [<span data-ttu-id="3e558-141">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="3e558-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

