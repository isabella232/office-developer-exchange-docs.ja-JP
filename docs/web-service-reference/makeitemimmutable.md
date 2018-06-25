---
title: MakeItemImmutable
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: de1d2a60-aeeb-4625-8b11-23c42e1e7bae
description: MakeItemImmutable 要素は、読み取り専用で、項目を行う必要があるかどうかを示すブール値を指定します。
ms.openlocfilehash: 63c05fd3572c7b4ab93fe098d9165a117849ef02
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832337"
---
# <a name="makeitemimmutable"></a><span data-ttu-id="bfaca-103">MakeItemImmutable</span><span class="sxs-lookup"><span data-stu-id="bfaca-103">MakeItemImmutable</span></span>

<span data-ttu-id="bfaca-104">**MakeItemImmutable**要素は、読み取り専用で、項目を行う必要があるかどうかを示すブール値を指定します。</span><span class="sxs-lookup"><span data-stu-id="bfaca-104">The **MakeItemImmutable** element specifies a Boolean value that indicates whether an item should be made read-only.</span></span> 
  
```XML
<MakeItemImmutable>true | false</MakeItemImmutable>
```

 <span data-ttu-id="bfaca-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="bfaca-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bfaca-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="bfaca-106">Attributes and elements</span></span>

<span data-ttu-id="bfaca-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="bfaca-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bfaca-108">属性</span><span class="sxs-lookup"><span data-stu-id="bfaca-108">Attributes</span></span>

<span data-ttu-id="bfaca-109">なし。</span><span class="sxs-lookup"><span data-stu-id="bfaca-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bfaca-110">子要素</span><span class="sxs-lookup"><span data-stu-id="bfaca-110">Child elements</span></span>

<span data-ttu-id="bfaca-111">なし。</span><span class="sxs-lookup"><span data-stu-id="bfaca-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bfaca-112">親要素</span><span class="sxs-lookup"><span data-stu-id="bfaca-112">Parent elements</span></span>

[<span data-ttu-id="bfaca-113">UpdateItemInRecoverableItems</span><span class="sxs-lookup"><span data-stu-id="bfaca-113">UpdateItemInRecoverableItems</span></span>](updateiteminrecoverableitems.md)
  
## <a name="text-value"></a><span data-ttu-id="bfaca-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="bfaca-114">Text value</span></span>

<span data-ttu-id="bfaca-115">の**場合は true** 、 **MakeItemImmutable**要素のテキスト値は、項目読み取り専用にすることを示します。</span><span class="sxs-lookup"><span data-stu-id="bfaca-115">A text value of **true** for the **MakeItemImmutable** element indicates that the item should be made read-only.</span></span> <span data-ttu-id="bfaca-116">**False**の値は、項目が読み取り/書き込みアクセスを許可していることを示します。</span><span class="sxs-lookup"><span data-stu-id="bfaca-116">A value of **false** indicates that the item allows read-write access.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="bfaca-117">備考</span><span class="sxs-lookup"><span data-stu-id="bfaca-117">Remarks</span></span>

<span data-ttu-id="bfaca-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="bfaca-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="bfaca-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="bfaca-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bfaca-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="bfaca-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bfaca-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="bfaca-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bfaca-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="bfaca-122">Schema name</span></span>  <br/> |<span data-ttu-id="bfaca-123">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="bfaca-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bfaca-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="bfaca-124">Validation file</span></span>  <br/> |<span data-ttu-id="bfaca-125">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="bfaca-125">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bfaca-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="bfaca-126">Can be empty</span></span>  <br/> ||
   

