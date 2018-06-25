---
title: IsPermanentFailure
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 18dc3a97-cc0a-4092-934e-a6e86f52e668
description: IsPermanentFailure 要素は、項目のインデックスを作成する前の試みに成功したかどうかを示します。
ms.openlocfilehash: 39592c15394a57e1c6aa1183ed0ccedeb085e6ea
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832085"
---
# <a name="ispermanentfailure"></a><span data-ttu-id="5b6a3-103">IsPermanentFailure</span><span class="sxs-lookup"><span data-stu-id="5b6a3-103">IsPermanentFailure</span></span>

<span data-ttu-id="5b6a3-104">**IsPermanentFailure**要素は、項目のインデックスを作成する前の試みに成功したかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5b6a3-104">The **IsPermanentFailure** element indicates whether a previous attempt to index the item was unsuccessful.</span></span> 
  
```XML
<IsPermanentFailure>true | false</IsPermanentFailure>
```

 <span data-ttu-id="5b6a3-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="5b6a3-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5b6a3-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5b6a3-106">Attributes and elements</span></span>

<span data-ttu-id="5b6a3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5b6a3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5b6a3-108">属性</span><span class="sxs-lookup"><span data-stu-id="5b6a3-108">Attributes</span></span>

<span data-ttu-id="5b6a3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5b6a3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5b6a3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5b6a3-110">Child elements</span></span>

<span data-ttu-id="5b6a3-111">なし。</span><span class="sxs-lookup"><span data-stu-id="5b6a3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5b6a3-112">親要素</span><span class="sxs-lookup"><span data-stu-id="5b6a3-112">Parent elements</span></span>

[<span data-ttu-id="5b6a3-113">NonIndexableItemDetail</span><span class="sxs-lookup"><span data-stu-id="5b6a3-113">NonIndexableItemDetail</span></span>](nonindexableitemdetail.md)
  
## <a name="text-value"></a><span data-ttu-id="5b6a3-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="5b6a3-114">Text value</span></span>

<span data-ttu-id="5b6a3-115">の**場合は true** 、 **IsPermanentFailure**要素のテキスト値は、メールボックスのアイテムのインデックスを作成する前の試みが失敗したことを示します。</span><span class="sxs-lookup"><span data-stu-id="5b6a3-115">A text value of **true** for the **IsPermanentFailure** element indicates that a previous attempt to index the mailbox item was unsuccessful.</span></span> <span data-ttu-id="5b6a3-116">**False**の値は、メールボックスのアイテムのインデックスを作成する前の試みが成功したことを示します。</span><span class="sxs-lookup"><span data-stu-id="5b6a3-116">A value of **false** indicates that a previous attempt to index the mailbox item was successful.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="5b6a3-117">備考</span><span class="sxs-lookup"><span data-stu-id="5b6a3-117">Remarks</span></span>

<span data-ttu-id="5b6a3-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="5b6a3-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="5b6a3-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="5b6a3-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5b6a3-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="5b6a3-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5b6a3-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="5b6a3-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5b6a3-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5b6a3-122">Schema name</span></span>  <br/> |<span data-ttu-id="5b6a3-123">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="5b6a3-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="5b6a3-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5b6a3-124">Validation file</span></span>  <br/> |<span data-ttu-id="5b6a3-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5b6a3-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5b6a3-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="5b6a3-126">Can be empty</span></span>  <br/> |<span data-ttu-id="5b6a3-127">false</span><span class="sxs-lookup"><span data-stu-id="5b6a3-127">false</span></span>  <br/> |
   

