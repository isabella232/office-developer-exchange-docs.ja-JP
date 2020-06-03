---
title: Guid
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 49dcf69f-bf8d-4be6-a24c-03bbd13f4fe5
description: Guid 要素は、メールボックスのグローバル一意識別子を指定します。
ms.openlocfilehash: 4db66b5ae2c67f64f75c69a3d77cfa2b587775be
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530776"
---
# <a name="guid"></a><span data-ttu-id="00b32-103">Guid</span><span class="sxs-lookup"><span data-stu-id="00b32-103">Guid</span></span>

<span data-ttu-id="00b32-104">**Guid**要素は、メールボックスのグローバル一意識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="00b32-104">The **Guid** element specifies the globally unique identifier of the mailbox.</span></span> 
  
```XML
<Guid></Guid>
```

 <span data-ttu-id="00b32-105">**GuidType**</span><span class="sxs-lookup"><span data-stu-id="00b32-105">**GuidType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="00b32-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="00b32-106">Attributes and elements</span></span>

<span data-ttu-id="00b32-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="00b32-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="00b32-108">属性</span><span class="sxs-lookup"><span data-stu-id="00b32-108">Attributes</span></span>

<span data-ttu-id="00b32-109">なし。</span><span class="sxs-lookup"><span data-stu-id="00b32-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="00b32-110">子要素</span><span class="sxs-lookup"><span data-stu-id="00b32-110">Child elements</span></span>

<span data-ttu-id="00b32-111">なし。</span><span class="sxs-lookup"><span data-stu-id="00b32-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="00b32-112">親要素</span><span class="sxs-lookup"><span data-stu-id="00b32-112">Parent elements</span></span>

|<span data-ttu-id="00b32-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="00b32-113">**Element**</span></span>|<span data-ttu-id="00b32-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="00b32-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00b32-115">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="00b32-115">SearchableMailbox</span></span>](searchablemailbox.md) <br/> |<span data-ttu-id="00b32-116">**Getsearchablemailboxes**要求から返されるメールボックスを指定します。</span><span class="sxs-lookup"><span data-stu-id="00b32-116">Specifies a mailbox returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="00b32-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="00b32-117">Text value</span></span>

<span data-ttu-id="00b32-118">**Guid**要素のテキスト値は、メールボックスを一意に識別する guid 値です。</span><span class="sxs-lookup"><span data-stu-id="00b32-118">The text value of the **Guid** element is a GUID value that uniquely identifies a mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="00b32-119">注釈</span><span class="sxs-lookup"><span data-stu-id="00b32-119">Remarks</span></span>

<span data-ttu-id="00b32-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="00b32-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="00b32-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="00b32-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="00b32-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="00b32-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="00b32-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="00b32-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="00b32-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="00b32-124">Schema Name</span></span>  <br/> |<span data-ttu-id="00b32-125">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="00b32-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="00b32-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="00b32-126">Validation File</span></span>  <br/> |<span data-ttu-id="00b32-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="00b32-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="00b32-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="00b32-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="00b32-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="00b32-129">See also</span></span>



- [<span data-ttu-id="00b32-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="00b32-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

