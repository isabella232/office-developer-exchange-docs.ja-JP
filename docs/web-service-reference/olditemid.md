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
description: OldItemId 要素には、コピーまたは移動されたアイテムの一意の識別子が含まれています。
ms.openlocfilehash: 9fab14478ffbb2dd8ad013d59520af943584f2eb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467467"
---
# <a name="olditemid"></a><span data-ttu-id="544cf-103">OldItemId</span><span class="sxs-lookup"><span data-stu-id="544cf-103">OldItemId</span></span>

<span data-ttu-id="544cf-104">**Olditemid**要素には、コピーまたは移動されたアイテムの一意の識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="544cf-104">The **OldItemId** element contains the unique identifier of the item that was copied or moved.</span></span> 
  
```xml
<OldItemId Id="" ChangeKey=""/>
```

 <span data-ttu-id="544cf-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="544cf-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="544cf-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="544cf-106">Attributes and elements</span></span>

<span data-ttu-id="544cf-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="544cf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="544cf-108">属性</span><span class="sxs-lookup"><span data-stu-id="544cf-108">Attributes</span></span>

|<span data-ttu-id="544cf-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="544cf-109">**Attribute**</span></span>|<span data-ttu-id="544cf-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="544cf-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="544cf-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="544cf-111">**Id**</span></span> <br/> |<span data-ttu-id="544cf-112">Exchange ストア内のアイテムを識別する文字列を格納します。</span><span class="sxs-lookup"><span data-stu-id="544cf-112">Contains a string that identifies an item in the Exchange store.</span></span> <span data-ttu-id="544cf-113">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="544cf-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="544cf-114">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="544cf-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="544cf-115">Id 属性によって識別されるアイテムのバージョンを識別する文字列を格納します。</span><span class="sxs-lookup"><span data-stu-id="544cf-115">Contains a string that identifies a version of an item that is identified by the Id attribute.</span></span> <span data-ttu-id="544cf-116">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="544cf-116">This attribute is optional.</span></span> <span data-ttu-id="544cf-117">この属性を使用して、アイテムの正しいバージョンが使用されるようにします。</span><span class="sxs-lookup"><span data-stu-id="544cf-117">Use this attribute to make sure that the correct version of an item is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="544cf-118">子要素</span><span class="sxs-lookup"><span data-stu-id="544cf-118">Child elements</span></span>

<span data-ttu-id="544cf-119">なし。</span><span class="sxs-lookup"><span data-stu-id="544cf-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="544cf-120">親要素</span><span class="sxs-lookup"><span data-stu-id="544cf-120">Parent elements</span></span>

|<span data-ttu-id="544cf-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="544cf-121">**Element**</span></span>|<span data-ttu-id="544cf-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="544cf-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="544cf-123">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="544cf-123">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="544cf-124">アイテムまたはフォルダーがコピーされるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="544cf-124">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="544cf-125">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="544cf-125">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="544cf-126">ある親フォルダーから別の親フォルダーにアイテムまたはフォルダーを移動するイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="544cf-126">Represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="544cf-127">注釈</span><span class="sxs-lookup"><span data-stu-id="544cf-127">Remarks</span></span>

<span data-ttu-id="544cf-128">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="544cf-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="544cf-129">要素の情報</span><span class="sxs-lookup"><span data-stu-id="544cf-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="544cf-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="544cf-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="544cf-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="544cf-131">Schema Name</span></span>  <br/> |<span data-ttu-id="544cf-132">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="544cf-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="544cf-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="544cf-133">Validation File</span></span>  <br/> |<span data-ttu-id="544cf-134">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="544cf-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="544cf-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="544cf-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="544cf-136">正しくない</span><span class="sxs-lookup"><span data-stu-id="544cf-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="544cf-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="544cf-137">See also</span></span>



[<span data-ttu-id="544cf-138">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="544cf-138">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="544cf-139">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="544cf-139">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="544cf-140">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="544cf-140">Unsubscribe operation</span></span>](unsubscribe-operation.md)


- [<span data-ttu-id="544cf-141">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="544cf-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

