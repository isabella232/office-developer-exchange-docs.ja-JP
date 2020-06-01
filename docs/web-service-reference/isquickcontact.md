---
title: IsQuickContact
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1c9542d6-ef72-4743-828a-bb671e783836
description: IsQuickContact 要素は、基になる連絡先がクイック連絡先であるかどうかを示すブール値を指定します。
ms.openlocfilehash: a8944be111a8dcbe914601ffc4e31794422d58aa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44441577"
---
# <a name="isquickcontact"></a><span data-ttu-id="b6d3f-103">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="b6d3f-103">IsQuickContact</span></span>

<span data-ttu-id="b6d3f-104">**Isquickcontact**要素は、基になる連絡先がクイック連絡先であるかどうかを示すブール値を指定します。</span><span class="sxs-lookup"><span data-stu-id="b6d3f-104">The **IsQuickContact** element specifies a Boolean value that indicates whether the underlying contact is a quick contact.</span></span> 
  
```XML
<IsQuickContact>true | false</IsQuickContact>
```

 <span data-ttu-id="b6d3f-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="b6d3f-105">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b6d3f-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b6d3f-106">Attributes and elements</span></span>

<span data-ttu-id="b6d3f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b6d3f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b6d3f-108">属性</span><span class="sxs-lookup"><span data-stu-id="b6d3f-108">Attributes</span></span>

<span data-ttu-id="b6d3f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b6d3f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b6d3f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b6d3f-110">Child elements</span></span>

<span data-ttu-id="b6d3f-111">なし。</span><span class="sxs-lookup"><span data-stu-id="b6d3f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b6d3f-112">親要素</span><span class="sxs-lookup"><span data-stu-id="b6d3f-112">Parent elements</span></span>

|<span data-ttu-id="b6d3f-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="b6d3f-113">**Element**</span></span>|<span data-ttu-id="b6d3f-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="b6d3f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b6d3f-115">属性 (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="b6d3f-115">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md) <br/> |<span data-ttu-id="b6d3f-116">**Persona**要素の属性の配列のインスタンスを指定します。</span><span class="sxs-lookup"><span data-stu-id="b6d3f-116">Specifies an instance in an array of attributes for a **Persona** element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b6d3f-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b6d3f-117">Text value</span></span>

<span data-ttu-id="b6d3f-118">**Isquickcontact**要素のテキスト値が**true の場合**は、連絡先がクイック連絡先であることを示します。</span><span class="sxs-lookup"><span data-stu-id="b6d3f-118">A text value of **true** for the **IsQuickContact** element indicates that the contact is a quick contact.</span></span> <span data-ttu-id="b6d3f-119">値が**false**の場合、連絡先がクイック連絡先ではないことを示します。</span><span class="sxs-lookup"><span data-stu-id="b6d3f-119">A value of **false** indicates that the contact is not a quick contact.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b6d3f-120">注釈</span><span class="sxs-lookup"><span data-stu-id="b6d3f-120">Remarks</span></span>

<span data-ttu-id="b6d3f-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b6d3f-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b6d3f-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b6d3f-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b6d3f-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b6d3f-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b6d3f-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="b6d3f-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b6d3f-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b6d3f-125">Schema Name</span></span>  <br/> |<span data-ttu-id="b6d3f-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="b6d3f-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="b6d3f-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b6d3f-127">Validation File</span></span>  <br/> |<span data-ttu-id="b6d3f-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="b6d3f-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="b6d3f-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b6d3f-129">Can Be Empty</span></span>  <br/> |<span data-ttu-id="b6d3f-130">false</span><span class="sxs-lookup"><span data-stu-id="b6d3f-130">false</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b6d3f-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="b6d3f-131">See also</span></span>



- [<span data-ttu-id="b6d3f-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="b6d3f-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

