---
title: UmEnabled
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UmEnabled
api_type:
- schema
ms.assetid: 87382d9b-0c02-49ec-85dc-3f5918df3195
description: UmEnabled 要素は、アカウントのユニファイド メッセージングが有効になっているかどうかを示します。
ms.openlocfilehash: 8324e02136adc6704bc0badb77131e9671ee569f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839769"
---
# <a name="umenabled"></a><span data-ttu-id="2fec2-103">UmEnabled</span><span class="sxs-lookup"><span data-stu-id="2fec2-103">UmEnabled</span></span>

<span data-ttu-id="2fec2-104">**UmEnabled**要素は、アカウントのユニファイド メッセージングが有効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2fec2-104">The **UmEnabled** element indicates whether Unified Messaging is enabled for an account.</span></span> 
  
```XML
<UmEnabled>true | false</UmEnabled>
```

 <span data-ttu-id="2fec2-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="2fec2-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2fec2-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2fec2-106">Attributes and elements</span></span>

<span data-ttu-id="2fec2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2fec2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2fec2-108">属性</span><span class="sxs-lookup"><span data-stu-id="2fec2-108">Attributes</span></span>

<span data-ttu-id="2fec2-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2fec2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2fec2-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2fec2-110">Child elements</span></span>

<span data-ttu-id="2fec2-111">なし。</span><span class="sxs-lookup"><span data-stu-id="2fec2-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2fec2-112">親要素</span><span class="sxs-lookup"><span data-stu-id="2fec2-112">Parent elements</span></span>

|<span data-ttu-id="2fec2-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="2fec2-113">**Element**</span></span>|<span data-ttu-id="2fec2-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="2fec2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2fec2-115">UnifiedMessagingConfiguration</span><span class="sxs-lookup"><span data-stu-id="2fec2-115">UnifiedMessagingConfiguration</span></span>](unifiedmessagingconfiguration.md) <br/> |<span data-ttu-id="2fec2-116">ユニファイド メッセージング サービスのサービスの構成情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2fec2-116">Contains service configuration information for the Unified Messaging service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2fec2-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="2fec2-117">Text value</span></span>

<span data-ttu-id="2fec2-118">**UmEnabled**要素のテキスト値は、アカウントのユニファイド メッセージングが有効になっている場合**は true。** それ以外の場合、値が**false**にします。</span><span class="sxs-lookup"><span data-stu-id="2fec2-118">The text value of the **UmEnabled** element is **true** if Unified Messaging is enabled for the account; otherwise, the value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2fec2-119">備考</span><span class="sxs-lookup"><span data-stu-id="2fec2-119">Remarks</span></span>

<span data-ttu-id="2fec2-120">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="2fec2-120">This element is required.</span></span>
  
<span data-ttu-id="2fec2-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2fec2-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2fec2-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="2fec2-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2fec2-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="2fec2-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2fec2-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2fec2-124">Schema Name</span></span>  <br/> |<span data-ttu-id="2fec2-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="2fec2-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="2fec2-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2fec2-126">Validation File</span></span>  <br/> |<span data-ttu-id="2fec2-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2fec2-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2fec2-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="2fec2-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="2fec2-129">False</span><span class="sxs-lookup"><span data-stu-id="2fec2-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2fec2-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="2fec2-130">See also</span></span>



- [<span data-ttu-id="2fec2-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="2fec2-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

