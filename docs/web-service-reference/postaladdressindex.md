---
title: PostalAddressIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PostalAddressIndex
api_type:
- schema
ms.assetid: 170fec26-5cb7-4578-ac09-140da9a6c84e
description: PostalAddressIndex 要素は、物理アドレスの表示の種類を表します。
ms.openlocfilehash: b99e7f2f9bbeeb7cdeaed7258e4d7c33bfc446d3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832852"
---
# <a name="postaladdressindex"></a><span data-ttu-id="b06d2-103">PostalAddressIndex</span><span class="sxs-lookup"><span data-stu-id="b06d2-103">PostalAddressIndex</span></span>

<span data-ttu-id="b06d2-104">**PostalAddressIndex**要素は、物理アドレスの表示の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="b06d2-104">The **PostalAddressIndex** element represents the display types for physical addresses.</span></span> 
  
```xml
<PostalAddressIndex/>
```

 <span data-ttu-id="b06d2-105">**PhysicalAddressIndexType**</span><span class="sxs-lookup"><span data-stu-id="b06d2-105">**PhysicalAddressIndexType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b06d2-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b06d2-106">Attributes and elements</span></span>

<span data-ttu-id="b06d2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b06d2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b06d2-108">属性</span><span class="sxs-lookup"><span data-stu-id="b06d2-108">Attributes</span></span>

<span data-ttu-id="b06d2-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b06d2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b06d2-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b06d2-110">Child elements</span></span>

<span data-ttu-id="b06d2-111">なし。</span><span class="sxs-lookup"><span data-stu-id="b06d2-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b06d2-112">親要素</span><span class="sxs-lookup"><span data-stu-id="b06d2-112">Parent elements</span></span>

|<span data-ttu-id="b06d2-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="b06d2-113">**Element**</span></span>|<span data-ttu-id="b06d2-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="b06d2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b06d2-115">Contact</span><span class="sxs-lookup"><span data-stu-id="b06d2-115">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="b06d2-116">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="b06d2-116">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b06d2-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b06d2-117">Text value</span></span>

<span data-ttu-id="b06d2-118">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="b06d2-118">A text value is required.</span></span> <span data-ttu-id="b06d2-119">この要素の使用可能なテキスト値は、次のように。</span><span class="sxs-lookup"><span data-stu-id="b06d2-119">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="b06d2-120">なし</span><span class="sxs-lookup"><span data-stu-id="b06d2-120">None</span></span>
    
- <span data-ttu-id="b06d2-121">Business</span><span class="sxs-lookup"><span data-stu-id="b06d2-121">Business</span></span>
    
- <span data-ttu-id="b06d2-122">Home</span><span class="sxs-lookup"><span data-stu-id="b06d2-122">Home</span></span>
    
- <span data-ttu-id="b06d2-123">Other</span><span class="sxs-lookup"><span data-stu-id="b06d2-123">Other</span></span>
    
## <a name="remarks"></a><span data-ttu-id="b06d2-124">備考</span><span class="sxs-lookup"><span data-stu-id="b06d2-124">Remarks</span></span>

<span data-ttu-id="b06d2-125">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="b06d2-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b06d2-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="b06d2-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b06d2-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="b06d2-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b06d2-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b06d2-128">Schema name</span></span>  <br/> |<span data-ttu-id="b06d2-129">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="b06d2-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="b06d2-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b06d2-130">Validation file</span></span>  <br/> |<span data-ttu-id="b06d2-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b06d2-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b06d2-132">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b06d2-132">Can be empty</span></span>  <br/> |<span data-ttu-id="b06d2-133">False</span><span class="sxs-lookup"><span data-stu-id="b06d2-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b06d2-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="b06d2-134">See also</span></span>



 <span data-ttu-id="b06d2-135">**PostalAddressIndex**</span><span class="sxs-lookup"><span data-stu-id="b06d2-135">**PostalAddressIndex**</span></span>


- [<span data-ttu-id="b06d2-136">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="b06d2-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="b06d2-137">連絡先 (Exchange Web サービス) を作成します。</span><span class="sxs-lookup"><span data-stu-id="b06d2-137">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[<span data-ttu-id="b06d2-138">連絡先を更新</span><span class="sxs-lookup"><span data-stu-id="b06d2-138">Updating Contacts</span></span>](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[<span data-ttu-id="b06d2-139">連絡先を削除します。</span><span class="sxs-lookup"><span data-stu-id="b06d2-139">Deleting Contacts</span></span>](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

