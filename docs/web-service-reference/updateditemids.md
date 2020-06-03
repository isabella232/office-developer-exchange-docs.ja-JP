---
title: UpdatedItemIds
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9199aeb2-abdf-40c5-8743-40b61853c951
description: UpdatedItemIds 要素は、更新された事前通知アイテムの識別子を指定します。
ms.openlocfilehash: 4a87bf50f90e80c0c887ee3a66b9f201ea1c8440
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465037"
---
# <a name="updateditemids"></a><span data-ttu-id="d87fc-103">UpdatedItemIds</span><span class="sxs-lookup"><span data-stu-id="d87fc-103">UpdatedItemIds</span></span>

<span data-ttu-id="d87fc-104">**Updateditemids**要素は、更新された事前通知アイテムの識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="d87fc-104">The **UpdatedItemIds** element specifies the identifiers of updated reminder items.</span></span> 
  
```XML
<UpdatedItemIds>
   <ItemId></ItemId>
</UpdatedItemIds>

```

 <span data-ttu-id="d87fc-105">**非 Emptyarrayofitemidstype**</span><span class="sxs-lookup"><span data-stu-id="d87fc-105">**NonEmptyArrayOfItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d87fc-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d87fc-106">Attributes and elements</span></span>

<span data-ttu-id="d87fc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d87fc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d87fc-108">属性</span><span class="sxs-lookup"><span data-stu-id="d87fc-108">Attributes</span></span>

<span data-ttu-id="d87fc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d87fc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d87fc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d87fc-110">Child elements</span></span>

[<span data-ttu-id="d87fc-111">ItemId</span><span class="sxs-lookup"><span data-stu-id="d87fc-111">ItemId</span></span>](itemid.md)
  
### <a name="parent-elements"></a><span data-ttu-id="d87fc-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d87fc-112">Parent elements</span></span>

[<span data-ttu-id="d87fc-113">PerformReminderActionResponse</span><span class="sxs-lookup"><span data-stu-id="d87fc-113">PerformReminderActionResponse</span></span>](performreminderactionresponse.md)
  
## <a name="remarks"></a><span data-ttu-id="d87fc-114">注釈</span><span class="sxs-lookup"><span data-stu-id="d87fc-114">Remarks</span></span>

<span data-ttu-id="d87fc-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d87fc-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d87fc-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d87fc-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="d87fc-117">[PerformReminderAction](performreminderaction-operation.md)操作が正常に完了しなかった場合、またはサーバーで変更が行われなかった場合は、 **Updateditemids**要素が空の値として返されます。</span><span class="sxs-lookup"><span data-stu-id="d87fc-117">If the [PerformReminderAction](performreminderaction-operation.md) operation did not complete successfully, or no changes were made on the server, the **UpdatedItemIds** element is returned as an empty value.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="d87fc-118">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d87fc-118">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d87fc-119">Namespace</span><span class="sxs-lookup"><span data-stu-id="d87fc-119">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d87fc-120">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d87fc-120">Schema Name</span></span>  <br/> |<span data-ttu-id="d87fc-121">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="d87fc-121">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d87fc-122">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d87fc-122">Validation File</span></span>  <br/> |<span data-ttu-id="d87fc-123">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="d87fc-123">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d87fc-124">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d87fc-124">Can be Empty</span></span>  <br/> |<span data-ttu-id="d87fc-125">正しい</span><span class="sxs-lookup"><span data-stu-id="d87fc-125">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d87fc-126">関連項目</span><span class="sxs-lookup"><span data-stu-id="d87fc-126">See also</span></span>



[<span data-ttu-id="d87fc-127">PerformReminderActionResponse</span><span class="sxs-lookup"><span data-stu-id="d87fc-127">PerformReminderActionResponse</span></span>](performreminderactionresponse.md)


- [<span data-ttu-id="d87fc-128">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d87fc-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

