---
title: IsNDR
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsNDR
api_type:
- schema
ms.assetid: 194f5836-7793-463a-a090-4386d1c2487a
description: IsNDR 要素は、受信メッセージが配信不能レポート (Ndr) をする必要があるかどうかを示しますを適用する場合の条件または例外の順序で。
ms.openlocfilehash: 651590d055a0532c904dbf6c481dca2f899d673f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832056"
---
# <a name="isndr"></a><span data-ttu-id="9eb60-103">IsNDR</span><span class="sxs-lookup"><span data-stu-id="9eb60-103">IsNDR</span></span>

<span data-ttu-id="9eb60-104">**IsNDR**要素は、受信メッセージが配信不能レポート (Ndr) をする必要があるかどうかを示しますを適用する場合の条件または例外の順序で。</span><span class="sxs-lookup"><span data-stu-id="9eb60-104">The **IsNDR** element indicates whether incoming messages must be non-delivery reports (NDRs) in order for the condition or exception to apply.</span></span> 
  
```XML
<IsNDR>true | false</IsNDR>
```

 <span data-ttu-id="9eb60-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="9eb60-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9eb60-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9eb60-106">Attributes and elements</span></span>

<span data-ttu-id="9eb60-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9eb60-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9eb60-108">属性</span><span class="sxs-lookup"><span data-stu-id="9eb60-108">Attributes</span></span>

<span data-ttu-id="9eb60-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9eb60-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9eb60-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9eb60-110">Child elements</span></span>

<span data-ttu-id="9eb60-111">なし。</span><span class="sxs-lookup"><span data-stu-id="9eb60-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9eb60-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9eb60-112">Parent elements</span></span>

|<span data-ttu-id="9eb60-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="9eb60-113">**Element**</span></span>|<span data-ttu-id="9eb60-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="9eb60-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9eb60-115">条件</span><span class="sxs-lookup"><span data-stu-id="9eb60-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="9eb60-116">条件を表しますが、満たされるとときに、ルールのルールの処理をトリガーします。</span><span class="sxs-lookup"><span data-stu-id="9eb60-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="9eb60-117">Exceptions</span><span class="sxs-lookup"><span data-stu-id="9eb60-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="9eb60-118">受信トレイ ルールの使用可能なルールの例外条件をすべてを表します。</span><span class="sxs-lookup"><span data-stu-id="9eb60-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9eb60-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9eb60-119">Text value</span></span>

<span data-ttu-id="9eb60-120">**True**の場合、テキスト値は、メッセージは NDR を適用する場合の条件または例外の順序のである必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="9eb60-120">A text value of **true** indicates that the message must be an NDR in order for the condition or exception to apply.</span></span> <span data-ttu-id="9eb60-121">**False**の値は、メッセージが NDR を適用する場合の条件または例外の順にする必要がありますできないことを示します。</span><span class="sxs-lookup"><span data-stu-id="9eb60-121">A value of **false** indicates that the message must not be an NDR in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="9eb60-122">備考</span><span class="sxs-lookup"><span data-stu-id="9eb60-122">Remarks</span></span>

<span data-ttu-id="9eb60-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9eb60-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9eb60-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="9eb60-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9eb60-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="9eb60-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9eb60-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9eb60-126">Schema Name</span></span>  <br/> |<span data-ttu-id="9eb60-127">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="9eb60-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9eb60-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9eb60-128">Validation File</span></span>  <br/> |<span data-ttu-id="9eb60-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9eb60-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9eb60-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9eb60-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="9eb60-131">True</span><span class="sxs-lookup"><span data-stu-id="9eb60-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9eb60-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="9eb60-132">See also</span></span>



- [<span data-ttu-id="9eb60-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="9eb60-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

