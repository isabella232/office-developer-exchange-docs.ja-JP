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
description: UmEnabled 要素は、ユニファイドメッセージングがアカウントに対して有効になっているかどうかを示します。
ms.openlocfilehash: 7ba7be69868cb439177702f74ff4a2f12875b7ff
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468356"
---
# <a name="umenabled"></a><span data-ttu-id="c5441-103">UmEnabled</span><span class="sxs-lookup"><span data-stu-id="c5441-103">UmEnabled</span></span>

<span data-ttu-id="c5441-104">**Umenabled**要素は、ユニファイドメッセージングがアカウントに対して有効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c5441-104">The **UmEnabled** element indicates whether Unified Messaging is enabled for an account.</span></span> 
  
```XML
<UmEnabled>true | false</UmEnabled>
```

 <span data-ttu-id="c5441-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="c5441-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c5441-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c5441-106">Attributes and elements</span></span>

<span data-ttu-id="c5441-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c5441-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c5441-108">属性</span><span class="sxs-lookup"><span data-stu-id="c5441-108">Attributes</span></span>

<span data-ttu-id="c5441-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c5441-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c5441-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c5441-110">Child elements</span></span>

<span data-ttu-id="c5441-111">なし。</span><span class="sxs-lookup"><span data-stu-id="c5441-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c5441-112">親要素</span><span class="sxs-lookup"><span data-stu-id="c5441-112">Parent elements</span></span>

|<span data-ttu-id="c5441-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="c5441-113">**Element**</span></span>|<span data-ttu-id="c5441-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="c5441-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c5441-115">UnifiedMessagingConfiguration</span><span class="sxs-lookup"><span data-stu-id="c5441-115">UnifiedMessagingConfiguration</span></span>](unifiedmessagingconfiguration.md) <br/> |<span data-ttu-id="c5441-116">ユニファイドメッセージングサービスのサービス構成情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c5441-116">Contains service configuration information for the Unified Messaging service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c5441-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c5441-117">Text value</span></span>

<span data-ttu-id="c5441-118">アカウントに対してユニファイドメッセージングが有効になっている場合、 **Umenabled**要素のテキスト値は**true**になります。それ以外の場合、値は**false**になります。</span><span class="sxs-lookup"><span data-stu-id="c5441-118">The text value of the **UmEnabled** element is **true** if Unified Messaging is enabled for the account; otherwise, the value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c5441-119">注釈</span><span class="sxs-lookup"><span data-stu-id="c5441-119">Remarks</span></span>

<span data-ttu-id="c5441-120">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="c5441-120">This element is required.</span></span>
  
<span data-ttu-id="c5441-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="c5441-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c5441-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c5441-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c5441-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="c5441-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c5441-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c5441-124">Schema Name</span></span>  <br/> |<span data-ttu-id="c5441-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="c5441-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="c5441-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c5441-126">Validation File</span></span>  <br/> |<span data-ttu-id="c5441-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="c5441-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c5441-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c5441-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="c5441-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="c5441-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c5441-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="c5441-130">See also</span></span>



- [<span data-ttu-id="c5441-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="c5441-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

