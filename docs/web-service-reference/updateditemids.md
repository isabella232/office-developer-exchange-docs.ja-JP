---
title: UpdatedItemIds
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9199aeb2-abdf-40c5-8743-40b61853c951
description: UpdatedItemIds 要素は、更新されたアイテムの識別子を指定します。
ms.openlocfilehash: b95ebb20823706e68b1fd66dc64f756808bb7375
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839835"
---
# <a name="updateditemids"></a><span data-ttu-id="243ca-103">UpdatedItemIds</span><span class="sxs-lookup"><span data-stu-id="243ca-103">UpdatedItemIds</span></span>

<span data-ttu-id="243ca-104">**UpdatedItemIds**要素は、更新されたアイテムの識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="243ca-104">The **UpdatedItemIds** element specifies the identifiers of updated reminder items.</span></span> 
  
```XML
<UpdatedItemIds>
   <ItemId></ItemId>
</UpdatedItemIds>

```

 <span data-ttu-id="243ca-105">**NonEmptyArrayOfItemIdsType**</span><span class="sxs-lookup"><span data-stu-id="243ca-105">**NonEmptyArrayOfItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="243ca-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="243ca-106">Attributes and elements</span></span>

<span data-ttu-id="243ca-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="243ca-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="243ca-108">属性</span><span class="sxs-lookup"><span data-stu-id="243ca-108">Attributes</span></span>

<span data-ttu-id="243ca-109">なし。</span><span class="sxs-lookup"><span data-stu-id="243ca-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="243ca-110">子要素</span><span class="sxs-lookup"><span data-stu-id="243ca-110">Child elements</span></span>

[<span data-ttu-id="243ca-111">ItemId</span><span class="sxs-lookup"><span data-stu-id="243ca-111">ItemId</span></span>](itemid.md)
  
### <a name="parent-elements"></a><span data-ttu-id="243ca-112">親要素</span><span class="sxs-lookup"><span data-stu-id="243ca-112">Parent elements</span></span>

[<span data-ttu-id="243ca-113">PerformReminderActionResponse</span><span class="sxs-lookup"><span data-stu-id="243ca-113">PerformReminderActionResponse</span></span>](performreminderactionresponse.md)
  
## <a name="remarks"></a><span data-ttu-id="243ca-114">備考</span><span class="sxs-lookup"><span data-stu-id="243ca-114">Remarks</span></span>

<span data-ttu-id="243ca-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="243ca-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="243ca-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="243ca-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="243ca-117">[PerformReminderAction](performreminderaction-operation.md)操作が正常に完了しませんでした、またはサーバー上で変更されていない、 **UpdatedItemIds**の要素が空の値として返されます。</span><span class="sxs-lookup"><span data-stu-id="243ca-117">If the [PerformReminderAction](performreminderaction-operation.md) operation did not complete successfully, or no changes were made on the server, the **UpdatedItemIds** element is returned as an empty value.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="243ca-118">要素情報</span><span class="sxs-lookup"><span data-stu-id="243ca-118">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="243ca-119">名前空間</span><span class="sxs-lookup"><span data-stu-id="243ca-119">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="243ca-120">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="243ca-120">Schema Name</span></span>  <br/> |<span data-ttu-id="243ca-121">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="243ca-121">Messages schema</span></span>  <br/> |
|<span data-ttu-id="243ca-122">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="243ca-122">Validation File</span></span>  <br/> |<span data-ttu-id="243ca-123">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="243ca-123">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="243ca-124">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="243ca-124">Can be Empty</span></span>  <br/> |<span data-ttu-id="243ca-125">True</span><span class="sxs-lookup"><span data-stu-id="243ca-125">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="243ca-126">関連項目</span><span class="sxs-lookup"><span data-stu-id="243ca-126">See also</span></span>



[<span data-ttu-id="243ca-127">PerformReminderActionResponse</span><span class="sxs-lookup"><span data-stu-id="243ca-127">PerformReminderActionResponse</span></span>](performreminderactionresponse.md)


- [<span data-ttu-id="243ca-128">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="243ca-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

