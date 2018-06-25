---
title: IsEncrypted
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsEncrypted
api_type:
- schema
ms.assetid: 68a30e92-c2b1-4af5-bb16-ba38afb80c43
description: 暗号化されたチャレンジの要素は、受信メッセージが S/MIME 暗号化を適用する場合の条件または例外の順序である必要があるかどうかを示します。
ms.openlocfilehash: 582a1f197d4ee6b60af91b1a178d79163b50052c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832003"
---
# <a name="isencrypted"></a><span data-ttu-id="e51ba-103">IsEncrypted</span><span class="sxs-lookup"><span data-stu-id="e51ba-103">IsEncrypted</span></span>

<span data-ttu-id="e51ba-104">**暗号化されたチャレンジ**の要素は、受信メッセージが S/MIME 暗号化を適用する場合の条件または例外の順序である必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e51ba-104">The **IsEncrypted** element indicates whether incoming messages must be S/MIME encrypted in order for the condition or exception to apply.</span></span> 
  
```XML
<IsEncrypted>true | false</IsEncrypted>
```

 <span data-ttu-id="e51ba-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="e51ba-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e51ba-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e51ba-106">Attributes and elements</span></span>

<span data-ttu-id="e51ba-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e51ba-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e51ba-108">属性</span><span class="sxs-lookup"><span data-stu-id="e51ba-108">Attributes</span></span>

<span data-ttu-id="e51ba-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e51ba-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e51ba-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e51ba-110">Child elements</span></span>

<span data-ttu-id="e51ba-111">なし。</span><span class="sxs-lookup"><span data-stu-id="e51ba-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e51ba-112">親要素</span><span class="sxs-lookup"><span data-stu-id="e51ba-112">Parent elements</span></span>

|<span data-ttu-id="e51ba-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="e51ba-113">**Element**</span></span>|<span data-ttu-id="e51ba-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="e51ba-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e51ba-115">条件</span><span class="sxs-lookup"><span data-stu-id="e51ba-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="e51ba-116">条件を表しますが、満たされるとときに、ルールのルールの処理をトリガーします。</span><span class="sxs-lookup"><span data-stu-id="e51ba-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="e51ba-117">Exceptions</span><span class="sxs-lookup"><span data-stu-id="e51ba-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="e51ba-118">受信トレイ ルールの使用可能なルールの例外条件をすべてを表します。</span><span class="sxs-lookup"><span data-stu-id="e51ba-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e51ba-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e51ba-119">Text value</span></span>

<span data-ttu-id="e51ba-120">**True**の場合、テキスト値は、メッセージに S/MIME 暗号化を適用する場合の条件または例外の順序で必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="e51ba-120">A text value of **true** indicates that the message must be S/MIME encrypted in order for the condition or exception to apply.</span></span> <span data-ttu-id="e51ba-121">**False**の値を適用する場合の条件または例外の順序で有効にするメッセージがないことを示します。</span><span class="sxs-lookup"><span data-stu-id="e51ba-121">A value of **false** indicates that the message does not have to be S/MIME in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e51ba-122">備考</span><span class="sxs-lookup"><span data-stu-id="e51ba-122">Remarks</span></span>

<span data-ttu-id="e51ba-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e51ba-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e51ba-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="e51ba-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e51ba-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="e51ba-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e51ba-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e51ba-126">Schema Name</span></span>  <br/> |<span data-ttu-id="e51ba-127">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="e51ba-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e51ba-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e51ba-128">Validation File</span></span>  <br/> |<span data-ttu-id="e51ba-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e51ba-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e51ba-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e51ba-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="e51ba-131">True</span><span class="sxs-lookup"><span data-stu-id="e51ba-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e51ba-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="e51ba-132">See also</span></span>



- [<span data-ttu-id="e51ba-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="e51ba-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

