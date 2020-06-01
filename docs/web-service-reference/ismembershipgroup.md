---
title: Isメンバーシップグループ
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0dc3e285-8f49-48ad-b844-37041c0d782b
description: Isメンバーシップグループ要素は、エンティティが配布グループまたはメールボックスであるかどうかを示すブール値を指定します。
ms.openlocfilehash: ed79961c6d13ab226c0b489103ef3d2c4a08668d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459287"
---
# <a name="ismembershipgroup"></a><span data-ttu-id="e7f59-103">Isメンバーシップグループ</span><span class="sxs-lookup"><span data-stu-id="e7f59-103">IsMembershipGroup</span></span>

<span data-ttu-id="e7f59-104">**Isメンバーシップグループ**要素は、エンティティが配布グループまたはメールボックスであるかどうかを示すブール値を指定します。</span><span class="sxs-lookup"><span data-stu-id="e7f59-104">The **IsMembershipGroup** element specifies a Boolean value that indicates whether the entity is a distribution group or a mailbox.</span></span> 
  
```XML
<IsMembershipGroup>true | false</IsMembershipGroup>
```

 <span data-ttu-id="e7f59-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="e7f59-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e7f59-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e7f59-106">Attributes and elements</span></span>

<span data-ttu-id="e7f59-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e7f59-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e7f59-108">属性</span><span class="sxs-lookup"><span data-stu-id="e7f59-108">Attributes</span></span>

<span data-ttu-id="e7f59-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e7f59-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e7f59-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e7f59-110">Child elements</span></span>

<span data-ttu-id="e7f59-111">なし。</span><span class="sxs-lookup"><span data-stu-id="e7f59-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e7f59-112">親要素</span><span class="sxs-lookup"><span data-stu-id="e7f59-112">Parent elements</span></span>

|<span data-ttu-id="e7f59-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="e7f59-113">**Element**</span></span>|<span data-ttu-id="e7f59-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="e7f59-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e7f59-115">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="e7f59-115">SearchableMailbox</span></span>](searchablemailbox.md) <br/> |<span data-ttu-id="e7f59-116">**Getsearchablemailboxes**要求から返されるメールボックスを指定します。</span><span class="sxs-lookup"><span data-stu-id="e7f59-116">Specifies a mailbox returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e7f59-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e7f59-117">Text value</span></span>

<span data-ttu-id="e7f59-118">**Isメンバーシップグループ**要素のテキスト値が**true**である場合は、エンティティが配布グループまたはメールボックスであることを示します。</span><span class="sxs-lookup"><span data-stu-id="e7f59-118">A text value of **true** for the **IsMembershipGroup** element indicates that the entity is a distribution group or a mailbox.</span></span> <span data-ttu-id="e7f59-119">値が false の場合、エンティティが配布グループまたはメールボックスではないことを示します。</span><span class="sxs-lookup"><span data-stu-id="e7f59-119">A value of false indicates that the entity is not a distribution group or a mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e7f59-120">注釈</span><span class="sxs-lookup"><span data-stu-id="e7f59-120">Remarks</span></span>

<span data-ttu-id="e7f59-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e7f59-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e7f59-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e7f59-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e7f59-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e7f59-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e7f59-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="e7f59-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e7f59-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e7f59-125">Schema Name</span></span>  <br/> |<span data-ttu-id="e7f59-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="e7f59-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="e7f59-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e7f59-127">Validation File</span></span>  <br/> |<span data-ttu-id="e7f59-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="e7f59-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="e7f59-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e7f59-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e7f59-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="e7f59-130">See also</span></span>



- [<span data-ttu-id="e7f59-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="e7f59-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

