---
title: InvalidRecipient (メール ヒント)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InvalidRecipient
api_type:
- schema
ms.assetid: 48959a99-bb0d-4004-963e-5a5baaa96476
description: InvalidRecipient 要素は、受信者が有効ではないかどうかを示します。
ms.openlocfilehash: addb86ece2be3091ac55a52ee2f16f5c5f72ae41
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831958"
---
# <a name="invalidrecipient-mailtips"></a><span data-ttu-id="19e67-103">InvalidRecipient (メール ヒント)</span><span class="sxs-lookup"><span data-stu-id="19e67-103">InvalidRecipient (MailTips)</span></span>

<span data-ttu-id="19e67-104">**InvalidRecipient**要素は、受信者が有効ではないかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="19e67-104">The **InvalidRecipient** element indicates whether the recipient is invalid.</span></span> 
  
```XML
<InvalidRecipient>true | false</InvalidRecipient>
```

 <span data-ttu-id="19e67-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="19e67-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="19e67-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="19e67-106">Attributes and elements</span></span>

<span data-ttu-id="19e67-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="19e67-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="19e67-108">属性</span><span class="sxs-lookup"><span data-stu-id="19e67-108">Attributes</span></span>

<span data-ttu-id="19e67-109">なし。</span><span class="sxs-lookup"><span data-stu-id="19e67-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="19e67-110">子要素</span><span class="sxs-lookup"><span data-stu-id="19e67-110">Child elements</span></span>

<span data-ttu-id="19e67-111">なし。</span><span class="sxs-lookup"><span data-stu-id="19e67-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="19e67-112">親要素</span><span class="sxs-lookup"><span data-stu-id="19e67-112">Parent elements</span></span>

|<span data-ttu-id="19e67-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="19e67-113">**Element**</span></span>|<span data-ttu-id="19e67-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="19e67-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="19e67-115">メール ヒント</span><span class="sxs-lookup"><span data-stu-id="19e67-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="19e67-116">さまざまな種類のメール ヒントの値を表します。</span><span class="sxs-lookup"><span data-stu-id="19e67-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="19e67-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="19e67-117">Text value</span></span>

<span data-ttu-id="19e67-118">**受信者が有効ではない場合は、この要素のテキスト値は**</span><span class="sxs-lookup"><span data-stu-id="19e67-118">The text value of this element is **true** if the recipient is invalid.</span></span> <span data-ttu-id="19e67-119">受信者が無効な場合に、値は**false です**。</span><span class="sxs-lookup"><span data-stu-id="19e67-119">The value is **false** if the recipient is not invalid.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="19e67-120">備考</span><span class="sxs-lookup"><span data-stu-id="19e67-120">Remarks</span></span>

<span data-ttu-id="19e67-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="19e67-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="19e67-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="19e67-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="19e67-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="19e67-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="19e67-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="19e67-124">Schema Name</span></span>  <br/> |<span data-ttu-id="19e67-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="19e67-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="19e67-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="19e67-126">Validation File</span></span>  <br/> |<span data-ttu-id="19e67-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="19e67-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="19e67-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="19e67-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="19e67-129">False</span><span class="sxs-lookup"><span data-stu-id="19e67-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="19e67-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="19e67-130">See also</span></span>



- [<span data-ttu-id="19e67-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="19e67-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

