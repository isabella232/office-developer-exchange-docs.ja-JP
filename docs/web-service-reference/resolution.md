---
title: 解決方法
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
description: Resolution 要素には、1つの解決済みエンティティが含まれています。
ms.openlocfilehash: 63c80f3c8d7dabf7e6dc1494df04c0be821b28bf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468286"
---
# <a name="resolution"></a><span data-ttu-id="b92bc-103">解決方法</span><span class="sxs-lookup"><span data-stu-id="b92bc-103">Resolution</span></span>

<span data-ttu-id="b92bc-104">**Resolution**要素には、1つの解決済みエンティティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="b92bc-104">The **Resolution** element contains a single resolved entity.</span></span> 
  
[<span data-ttu-id="b92bc-105">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="b92bc-105">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
  
[<span data-ttu-id="b92bc-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b92bc-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="b92bc-107">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b92bc-107">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
  
[<span data-ttu-id="b92bc-108">解像度セット</span><span class="sxs-lookup"><span data-stu-id="b92bc-108">ResolutionSet</span></span>](resolutionset.md)
  
[<span data-ttu-id="b92bc-109">Resolution</span><span class="sxs-lookup"><span data-stu-id="b92bc-109">Resolution</span></span>](resolution.md)
  
```xml
<Resolution>
   <Mailbox/>
   <Contact/>
</Resolution>
```

 <span data-ttu-id="b92bc-110">**解像度の種類**</span><span class="sxs-lookup"><span data-stu-id="b92bc-110">**ResolutionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b92bc-111">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b92bc-111">Attributes and elements</span></span>

<span data-ttu-id="b92bc-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b92bc-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b92bc-113">属性</span><span class="sxs-lookup"><span data-stu-id="b92bc-113">Attributes</span></span>

<span data-ttu-id="b92bc-114">なし。</span><span class="sxs-lookup"><span data-stu-id="b92bc-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b92bc-115">子要素</span><span class="sxs-lookup"><span data-stu-id="b92bc-115">Child elements</span></span>

|<span data-ttu-id="b92bc-116">**Element**</span><span class="sxs-lookup"><span data-stu-id="b92bc-116">**Element**</span></span>|<span data-ttu-id="b92bc-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="b92bc-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b92bc-118">メールボックス</span><span class="sxs-lookup"><span data-stu-id="b92bc-118">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="b92bc-119">メールが有効な Active Directory ディレクトリサービスオブジェクトを識別します。</span><span class="sxs-lookup"><span data-stu-id="b92bc-119">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
|[<span data-ttu-id="b92bc-120">連絡先</span><span class="sxs-lookup"><span data-stu-id="b92bc-120">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="b92bc-121">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="b92bc-121">Represents an Exchange contact item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b92bc-122">親要素</span><span class="sxs-lookup"><span data-stu-id="b92bc-122">Parent elements</span></span>

|<span data-ttu-id="b92bc-123">**要素**</span><span class="sxs-lookup"><span data-stu-id="b92bc-123">**Element**</span></span>|<span data-ttu-id="b92bc-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="b92bc-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b92bc-125">解像度セット</span><span class="sxs-lookup"><span data-stu-id="b92bc-125">ResolutionSet</span></span>](resolutionset.md) <br/> |<span data-ttu-id="b92bc-126">あいまいな名前の解決方法の配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="b92bc-126">Contains an array of resolutions for an ambiguous name.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b92bc-127">注釈</span><span class="sxs-lookup"><span data-stu-id="b92bc-127">Remarks</span></span>

<span data-ttu-id="b92bc-128">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="b92bc-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b92bc-129">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b92bc-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b92bc-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="b92bc-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b92bc-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b92bc-131">Schema name</span></span>  <br/> |<span data-ttu-id="b92bc-132">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="b92bc-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="b92bc-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b92bc-133">Validation file</span></span>  <br/> |<span data-ttu-id="b92bc-134">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="b92bc-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b92bc-135">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b92bc-135">Can be empty</span></span>  <br/> |<span data-ttu-id="b92bc-136">正しくない</span><span class="sxs-lookup"><span data-stu-id="b92bc-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b92bc-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="b92bc-137">See also</span></span>



[<span data-ttu-id="b92bc-138">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="b92bc-138">ResolveNames</span></span>](resolvenames.md)
  
[<span data-ttu-id="b92bc-139">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="b92bc-139">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
  
[<span data-ttu-id="b92bc-140">ResolveNames 操作</span><span class="sxs-lookup"><span data-stu-id="b92bc-140">ResolveNames operation</span></span>](resolvenames-operation.md)

