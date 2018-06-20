---
title: IsQuickContact
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1c9542d6-ef72-4743-828a-bb671e783836
description: IsQuickContact 要素は、基になっている取引先担当者が取引先担当者を簡易であるかどうかを示すブール値を指定します。
ms.openlocfilehash: 979dbd3c0358eacd443eed79b258f7dd6bb9bc7d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832092"
---
# <a name="isquickcontact"></a><span data-ttu-id="b3216-103">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="b3216-103">IsQuickContact</span></span>

<span data-ttu-id="b3216-104">**IsQuickContact**要素は、基になっている取引先担当者が取引先担当者を簡易であるかどうかを示すブール値を指定します。</span><span class="sxs-lookup"><span data-stu-id="b3216-104">The **IsQuickContact** element specifies a Boolean value that indicates whether the underlying contact is a quick contact.</span></span> 
  
```XML
<IsQuickContact>true | false</IsQuickContact>
```

 <span data-ttu-id="b3216-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="b3216-105">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b3216-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b3216-106">Attributes and elements</span></span>

<span data-ttu-id="b3216-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b3216-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b3216-108">属性</span><span class="sxs-lookup"><span data-stu-id="b3216-108">Attributes</span></span>

<span data-ttu-id="b3216-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b3216-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b3216-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b3216-110">Child elements</span></span>

<span data-ttu-id="b3216-111">なし。</span><span class="sxs-lookup"><span data-stu-id="b3216-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b3216-112">親要素</span><span class="sxs-lookup"><span data-stu-id="b3216-112">Parent elements</span></span>

|<span data-ttu-id="b3216-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="b3216-113">**Element**</span></span>|<span data-ttu-id="b3216-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="b3216-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b3216-115">属性 (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="b3216-115">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md) <br/> |<span data-ttu-id="b3216-116">**ペルソナ**の要素の属性の配列のインスタンスを指定します。</span><span class="sxs-lookup"><span data-stu-id="b3216-116">Specifies an instance in an array of attributes for a **Persona** element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b3216-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b3216-117">Text value</span></span>

<span data-ttu-id="b3216-118">の**場合は true** 、 **IsQuickContact**要素のテキスト値は、連絡先がクイック連絡先であることを示します。</span><span class="sxs-lookup"><span data-stu-id="b3216-118">A text value of **true** for the **IsQuickContact** element indicates that the contact is a quick contact.</span></span> <span data-ttu-id="b3216-119">**False**の値は、連絡先がクイック連絡先ではないことを示します。</span><span class="sxs-lookup"><span data-stu-id="b3216-119">A value of **false** indicates that the contact is not a quick contact.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b3216-120">備考</span><span class="sxs-lookup"><span data-stu-id="b3216-120">Remarks</span></span>

<span data-ttu-id="b3216-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b3216-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b3216-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b3216-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b3216-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="b3216-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b3216-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="b3216-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b3216-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b3216-125">Schema Name</span></span>  <br/> |<span data-ttu-id="b3216-126">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="b3216-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="b3216-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b3216-127">Validation File</span></span>  <br/> |<span data-ttu-id="b3216-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="b3216-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="b3216-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b3216-129">Can Be Empty</span></span>  <br/> |<span data-ttu-id="b3216-130">false</span><span class="sxs-lookup"><span data-stu-id="b3216-130">false</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b3216-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="b3216-131">See also</span></span>



- [<span data-ttu-id="b3216-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="b3216-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

