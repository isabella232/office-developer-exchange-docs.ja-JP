---
title: GroupType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c31552f-22b8-4bf0-8cac-046fd92ac0d4
description: GroupType 要素では、インスタント メッセージング (IM) のグループのグループ クラスを指定します。
ms.openlocfilehash: 330a1567ce85877ba73c6205898ea66b59585e16
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831800"
---
# <a name="grouptype"></a><span data-ttu-id="44ac3-103">GroupType</span><span class="sxs-lookup"><span data-stu-id="44ac3-103">GroupType</span></span>

<span data-ttu-id="44ac3-104">**GroupType**要素では、インスタント メッセージング (IM) のグループのグループ クラスを指定します。</span><span class="sxs-lookup"><span data-stu-id="44ac3-104">The **GroupType** element specifies the group class of an instant messaging (IM) group.</span></span> 
  
```XML
<GroupType></GroupType>
```

 <span data-ttu-id="44ac3-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="44ac3-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="44ac3-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="44ac3-106">Attributes and elements</span></span>

<span data-ttu-id="44ac3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="44ac3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="44ac3-108">属性</span><span class="sxs-lookup"><span data-stu-id="44ac3-108">Attributes</span></span>

<span data-ttu-id="44ac3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="44ac3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="44ac3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="44ac3-110">Child elements</span></span>

<span data-ttu-id="44ac3-111">なし。</span><span class="sxs-lookup"><span data-stu-id="44ac3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="44ac3-112">親要素</span><span class="sxs-lookup"><span data-stu-id="44ac3-112">Parent elements</span></span>

|<span data-ttu-id="44ac3-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="44ac3-113">**Element**</span></span>|<span data-ttu-id="44ac3-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="44ac3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="44ac3-115">ImGroup</span><span class="sxs-lookup"><span data-stu-id="44ac3-115">ImGroup</span></span>](imgroup.md) <br/> |<span data-ttu-id="44ac3-116">インスタント メッセージングのグループを表します。</span><span class="sxs-lookup"><span data-stu-id="44ac3-116">Represents an instant messaging group.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="44ac3-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="44ac3-117">Text value</span></span>

<span data-ttu-id="44ac3-118">**GroupType**要素のテキスト値は、グループの種類を指定する文字列値です。</span><span class="sxs-lookup"><span data-stu-id="44ac3-118">The text value of the **GroupType** element is a string value that specifies type of the group.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="44ac3-119">備考</span><span class="sxs-lookup"><span data-stu-id="44ac3-119">Remarks</span></span>

<span data-ttu-id="44ac3-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="44ac3-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="44ac3-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="44ac3-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="44ac3-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="44ac3-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="44ac3-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="44ac3-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="44ac3-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="44ac3-124">Schema Name</span></span>  <br/> |<span data-ttu-id="44ac3-125">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="44ac3-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="44ac3-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="44ac3-126">Validation File</span></span>  <br/> |<span data-ttu-id="44ac3-127">types.xsd</span><span class="sxs-lookup"><span data-stu-id="44ac3-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="44ac3-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="44ac3-128">Can Be Empty</span></span>  <br/> |<span data-ttu-id="44ac3-129">False</span><span class="sxs-lookup"><span data-stu-id="44ac3-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="44ac3-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="44ac3-130">See also</span></span>



- [<span data-ttu-id="44ac3-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="44ac3-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

