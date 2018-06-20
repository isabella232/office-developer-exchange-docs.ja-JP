---
title: PostalCode
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PostalCode
api_type:
- schema
ms.assetid: 35935ca3-60d5-47f0-b16d-69ab2b8fdd49
description: '[郵便番号] 要素は、連絡先アイテムの郵便番号コードを表します。'
ms.openlocfilehash: 853c65e0ac2fe182b1d188996948eaab6a1b7165
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832857"
---
# <a name="postalcode"></a><span data-ttu-id="83fed-103">PostalCode</span><span class="sxs-lookup"><span data-stu-id="83fed-103">PostalCode</span></span>

<span data-ttu-id="83fed-104">**[郵便番号]** 要素は、連絡先アイテムの郵便番号コードを表します。</span><span class="sxs-lookup"><span data-stu-id="83fed-104">The **PostalCode** element represents the postal code for a contact item.</span></span> 
  
```xml
<PostalCode/>
```

 <span data-ttu-id="83fed-105">**string**</span><span class="sxs-lookup"><span data-stu-id="83fed-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="83fed-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="83fed-106">Attributes and elements</span></span>

<span data-ttu-id="83fed-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="83fed-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="83fed-108">属性</span><span class="sxs-lookup"><span data-stu-id="83fed-108">Attributes</span></span>

<span data-ttu-id="83fed-109">なし。</span><span class="sxs-lookup"><span data-stu-id="83fed-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="83fed-110">子要素</span><span class="sxs-lookup"><span data-stu-id="83fed-110">Child elements</span></span>

<span data-ttu-id="83fed-111">なし。</span><span class="sxs-lookup"><span data-stu-id="83fed-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="83fed-112">親要素</span><span class="sxs-lookup"><span data-stu-id="83fed-112">Parent elements</span></span>

|<span data-ttu-id="83fed-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="83fed-113">**Element**</span></span>|<span data-ttu-id="83fed-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="83fed-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="83fed-115">エントリ (PhysicalAddress)</span><span class="sxs-lookup"><span data-stu-id="83fed-115">Entry (PhysicalAddress)</span></span>](entry-physicaladdress.md) <br/> |<span data-ttu-id="83fed-116">連絡先アイテムの 1 つの物理アドレスをについて説明します。</span><span class="sxs-lookup"><span data-stu-id="83fed-116">Describes a single physical address for a contact item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="83fed-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="83fed-117">Text value</span></span>

<span data-ttu-id="83fed-118">テキスト値は、連絡先の郵便番号コードを表す文字列値です。</span><span class="sxs-lookup"><span data-stu-id="83fed-118">The text value is a string value that represents the postal code of a contact.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="83fed-119">備考</span><span class="sxs-lookup"><span data-stu-id="83fed-119">Remarks</span></span>

<span data-ttu-id="83fed-120">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="83fed-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="83fed-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="83fed-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="83fed-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="83fed-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="83fed-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="83fed-123">Schema name</span></span>  <br/> |<span data-ttu-id="83fed-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="83fed-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="83fed-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="83fed-125">Validation file</span></span>  <br/> |<span data-ttu-id="83fed-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="83fed-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="83fed-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="83fed-127">Can be empty</span></span>  <br/> |<span data-ttu-id="83fed-128">False</span><span class="sxs-lookup"><span data-stu-id="83fed-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="83fed-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="83fed-129">See also</span></span>



- [<span data-ttu-id="83fed-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="83fed-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

