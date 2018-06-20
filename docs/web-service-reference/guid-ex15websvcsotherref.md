---
title: GUID
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 49dcf69f-bf8d-4be6-a24c-03bbd13f4fe5
description: Guid 要素では、メールボックスのグローバルに一意の識別子を指定します。
ms.openlocfilehash: 35307a706523fc5c2916767c7508dec07deb8d09
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831799"
---
# <a name="guid"></a><span data-ttu-id="3ede8-103">GUID</span><span class="sxs-lookup"><span data-stu-id="3ede8-103">Guid</span></span>

<span data-ttu-id="3ede8-104">**Guid**要素では、メールボックスのグローバルに一意の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="3ede8-104">The **Guid** element specifies the globally unique identifier of the mailbox.</span></span> 
  
```XML
<Guid></Guid>
```

 <span data-ttu-id="3ede8-105">**GuidType**</span><span class="sxs-lookup"><span data-stu-id="3ede8-105">**GuidType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3ede8-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="3ede8-106">Attributes and elements</span></span>

<span data-ttu-id="3ede8-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3ede8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3ede8-108">属性</span><span class="sxs-lookup"><span data-stu-id="3ede8-108">Attributes</span></span>

<span data-ttu-id="3ede8-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3ede8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3ede8-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3ede8-110">Child elements</span></span>

<span data-ttu-id="3ede8-111">なし。</span><span class="sxs-lookup"><span data-stu-id="3ede8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3ede8-112">親要素</span><span class="sxs-lookup"><span data-stu-id="3ede8-112">Parent elements</span></span>

|<span data-ttu-id="3ede8-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="3ede8-113">**Element**</span></span>|<span data-ttu-id="3ede8-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="3ede8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3ede8-115">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="3ede8-115">SearchableMailbox</span></span>](searchablemailbox.md) <br/> |<span data-ttu-id="3ede8-116">メールボックスは、 **GetSearchableMailboxes**要求から返されるかを指定します。</span><span class="sxs-lookup"><span data-stu-id="3ede8-116">Specifies a mailbox returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3ede8-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3ede8-117">Text value</span></span>

<span data-ttu-id="3ede8-118">**Guid**要素のテキスト値は、メールボックスを一意に識別する GUID 値です。</span><span class="sxs-lookup"><span data-stu-id="3ede8-118">The text value of the **Guid** element is a GUID value that uniquely identifies a mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3ede8-119">備考</span><span class="sxs-lookup"><span data-stu-id="3ede8-119">Remarks</span></span>

<span data-ttu-id="3ede8-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="3ede8-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3ede8-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="3ede8-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3ede8-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="3ede8-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3ede8-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="3ede8-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3ede8-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3ede8-124">Schema Name</span></span>  <br/> |<span data-ttu-id="3ede8-125">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="3ede8-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="3ede8-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3ede8-126">Validation File</span></span>  <br/> |<span data-ttu-id="3ede8-127">types.xsd</span><span class="sxs-lookup"><span data-stu-id="3ede8-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="3ede8-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="3ede8-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="3ede8-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="3ede8-129">See also</span></span>



- [<span data-ttu-id="3ede8-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="3ede8-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

