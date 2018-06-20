---
title: 解決策
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Resolution
api_type:
- schema
ms.assetid: 573bed4b-d7b1-4baf-b16f-0795cdebf1a7
description: 解像度の要素には、1 つの解決されたエンティティが含まれています。
ms.openlocfilehash: d65f6401e54a4397cad1bfcc85384f644fbae405
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833156"
---
# <a name="resolution"></a><span data-ttu-id="c34af-103">解決策</span><span class="sxs-lookup"><span data-stu-id="c34af-103">Resolution</span></span>

<span data-ttu-id="c34af-104">**解像度**の要素には、1 つの解決されたエンティティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="c34af-104">The **Resolution** element contains a single resolved entity.</span></span> 
  
[<span data-ttu-id="c34af-105">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="c34af-105">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
  
[<span data-ttu-id="c34af-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c34af-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="c34af-107">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c34af-107">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
  
[<span data-ttu-id="c34af-108">ResolutionSet</span><span class="sxs-lookup"><span data-stu-id="c34af-108">ResolutionSet</span></span>](resolutionset.md)
  
[<span data-ttu-id="c34af-109">解決策</span><span class="sxs-lookup"><span data-stu-id="c34af-109">Resolution</span></span>](resolution.md)
  
```xml
<Resolution>
   <Mailbox/>
   <Contact/>
</Resolution>
```

 <span data-ttu-id="c34af-110">**ResolutionType**</span><span class="sxs-lookup"><span data-stu-id="c34af-110">**ResolutionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c34af-111">属性および要素</span><span class="sxs-lookup"><span data-stu-id="c34af-111">Attributes and elements</span></span>

<span data-ttu-id="c34af-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c34af-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c34af-113">属性</span><span class="sxs-lookup"><span data-stu-id="c34af-113">Attributes</span></span>

<span data-ttu-id="c34af-114">なし。</span><span class="sxs-lookup"><span data-stu-id="c34af-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c34af-115">子要素</span><span class="sxs-lookup"><span data-stu-id="c34af-115">Child elements</span></span>

|<span data-ttu-id="c34af-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="c34af-116">**Element**</span></span>|<span data-ttu-id="c34af-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="c34af-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c34af-118">メールボックス</span><span class="sxs-lookup"><span data-stu-id="c34af-118">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="c34af-119">メールが有効な Active Directory ディレクトリ サービス オブジェクトを識別します。</span><span class="sxs-lookup"><span data-stu-id="c34af-119">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
|[<span data-ttu-id="c34af-120">Contact</span><span class="sxs-lookup"><span data-stu-id="c34af-120">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="c34af-121">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="c34af-121">Represents an Exchange contact item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c34af-122">親要素</span><span class="sxs-lookup"><span data-stu-id="c34af-122">Parent elements</span></span>

|<span data-ttu-id="c34af-123">**要素**</span><span class="sxs-lookup"><span data-stu-id="c34af-123">**Element**</span></span>|<span data-ttu-id="c34af-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="c34af-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c34af-125">ResolutionSet</span><span class="sxs-lookup"><span data-stu-id="c34af-125">ResolutionSet</span></span>](resolutionset.md) <br/> |<span data-ttu-id="c34af-126">あいまいな名前の解決策の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c34af-126">Contains an array of resolutions for an ambiguous name.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c34af-127">備考</span><span class="sxs-lookup"><span data-stu-id="c34af-127">Remarks</span></span>

<span data-ttu-id="c34af-128">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="c34af-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c34af-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="c34af-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c34af-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="c34af-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c34af-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c34af-131">Schema name</span></span>  <br/> |<span data-ttu-id="c34af-132">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="c34af-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="c34af-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c34af-133">Validation file</span></span>  <br/> |<span data-ttu-id="c34af-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c34af-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c34af-135">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c34af-135">Can be empty</span></span>  <br/> |<span data-ttu-id="c34af-136">False</span><span class="sxs-lookup"><span data-stu-id="c34af-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c34af-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="c34af-137">See also</span></span>



[<span data-ttu-id="c34af-138">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="c34af-138">ResolveNames</span></span>](resolvenames.md)
  
[<span data-ttu-id="c34af-139">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="c34af-139">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
  
[<span data-ttu-id="c34af-140">ResolveNames 操作</span><span class="sxs-lookup"><span data-stu-id="c34af-140">ResolveNames operation</span></span>](resolvenames-operation.md)

