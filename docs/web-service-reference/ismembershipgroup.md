---
title: IsMembershipGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0dc3e285-8f49-48ad-b844-37041c0d782b
description: IsMembershipGroup 要素は、エンティティが、メールボックスまたは配布グループかどうかを示すブール値を指定します。
ms.openlocfilehash: 03ab0dc75d2c798b7f2afeef85aa45f0349be70a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832050"
---
# <a name="ismembershipgroup"></a><span data-ttu-id="a3c18-103">IsMembershipGroup</span><span class="sxs-lookup"><span data-stu-id="a3c18-103">IsMembershipGroup</span></span>

<span data-ttu-id="a3c18-104">**IsMembershipGroup**要素は、エンティティが、メールボックスまたは配布グループかどうかを示すブール値を指定します。</span><span class="sxs-lookup"><span data-stu-id="a3c18-104">The **IsMembershipGroup** element specifies a Boolean value that indicates whether the entity is a distribution group or a mailbox.</span></span> 
  
```XML
<IsMembershipGroup>true | false</IsMembershipGroup>
```

 <span data-ttu-id="a3c18-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="a3c18-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a3c18-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a3c18-106">Attributes and elements</span></span>

<span data-ttu-id="a3c18-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a3c18-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a3c18-108">属性</span><span class="sxs-lookup"><span data-stu-id="a3c18-108">Attributes</span></span>

<span data-ttu-id="a3c18-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a3c18-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a3c18-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a3c18-110">Child elements</span></span>

<span data-ttu-id="a3c18-111">なし。</span><span class="sxs-lookup"><span data-stu-id="a3c18-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a3c18-112">親要素</span><span class="sxs-lookup"><span data-stu-id="a3c18-112">Parent elements</span></span>

|<span data-ttu-id="a3c18-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="a3c18-113">**Element**</span></span>|<span data-ttu-id="a3c18-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="a3c18-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a3c18-115">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="a3c18-115">SearchableMailbox</span></span>](searchablemailbox.md) <br/> |<span data-ttu-id="a3c18-116">メールボックスは、 **GetSearchableMailboxes**要求から返されるかを指定します。</span><span class="sxs-lookup"><span data-stu-id="a3c18-116">Specifies a mailbox returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a3c18-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a3c18-117">Text value</span></span>

<span data-ttu-id="a3c18-118">の**場合は true** 、 **IsMembershipGroup**要素のテキスト値は、エンティティがメールボックスまたは配布グループであることを示します。</span><span class="sxs-lookup"><span data-stu-id="a3c18-118">A text value of **true** for the **IsMembershipGroup** element indicates that the entity is a distribution group or a mailbox.</span></span> <span data-ttu-id="a3c18-119">False の値は、エンティティが、メールボックスまたは配布グループではないことを示します。</span><span class="sxs-lookup"><span data-stu-id="a3c18-119">A value of false indicates that the entity is not a distribution group or a mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a3c18-120">備考</span><span class="sxs-lookup"><span data-stu-id="a3c18-120">Remarks</span></span>

<span data-ttu-id="a3c18-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="a3c18-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a3c18-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a3c18-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a3c18-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="a3c18-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a3c18-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="a3c18-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a3c18-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a3c18-125">Schema Name</span></span>  <br/> |<span data-ttu-id="a3c18-126">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="a3c18-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="a3c18-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a3c18-127">Validation File</span></span>  <br/> |<span data-ttu-id="a3c18-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="a3c18-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="a3c18-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a3c18-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="a3c18-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="a3c18-130">See also</span></span>



- [<span data-ttu-id="a3c18-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="a3c18-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

