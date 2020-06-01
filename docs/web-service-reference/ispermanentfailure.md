---
title: IsPermanentFailure
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 18dc3a97-cc0a-4092-934e-a6e86f52e668
description: IsPermanentFailure 要素は、アイテムに対する以前のインデックス作成の試行が失敗したかどうかを示します。
ms.openlocfilehash: 48a13eebfa16c538c1b10d92f080d51f1b318d12
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460394"
---
# <a name="ispermanentfailure"></a><span data-ttu-id="7f459-103">IsPermanentFailure</span><span class="sxs-lookup"><span data-stu-id="7f459-103">IsPermanentFailure</span></span>

<span data-ttu-id="7f459-104">**IsPermanentFailure**要素は、アイテムに対する以前のインデックス作成の試行が失敗したかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7f459-104">The **IsPermanentFailure** element indicates whether a previous attempt to index the item was unsuccessful.</span></span> 
  
```XML
<IsPermanentFailure>true | false</IsPermanentFailure>
```

 <span data-ttu-id="7f459-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="7f459-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7f459-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7f459-106">Attributes and elements</span></span>

<span data-ttu-id="7f459-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7f459-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7f459-108">属性</span><span class="sxs-lookup"><span data-stu-id="7f459-108">Attributes</span></span>

<span data-ttu-id="7f459-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7f459-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7f459-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7f459-110">Child elements</span></span>

<span data-ttu-id="7f459-111">なし。</span><span class="sxs-lookup"><span data-stu-id="7f459-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7f459-112">親要素</span><span class="sxs-lookup"><span data-stu-id="7f459-112">Parent elements</span></span>

[<span data-ttu-id="7f459-113">NonIndexableItemDetail</span><span class="sxs-lookup"><span data-stu-id="7f459-113">NonIndexableItemDetail</span></span>](nonindexableitemdetail.md)
  
## <a name="text-value"></a><span data-ttu-id="7f459-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7f459-114">Text value</span></span>

<span data-ttu-id="7f459-115">**IsPermanentFailure**要素のテキスト値が**true**になっている場合、メールボックスアイテムの以前のインデックス作成の試行が失敗したことを示します。</span><span class="sxs-lookup"><span data-stu-id="7f459-115">A text value of **true** for the **IsPermanentFailure** element indicates that a previous attempt to index the mailbox item was unsuccessful.</span></span> <span data-ttu-id="7f459-116">値が**false**の場合、メールボックスアイテムの以前のインデックス作成が成功したことを示します。</span><span class="sxs-lookup"><span data-stu-id="7f459-116">A value of **false** indicates that a previous attempt to index the mailbox item was successful.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="7f459-117">注釈</span><span class="sxs-lookup"><span data-stu-id="7f459-117">Remarks</span></span>

<span data-ttu-id="7f459-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="7f459-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7f459-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7f459-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7f459-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7f459-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7f459-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="7f459-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7f459-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7f459-122">Schema name</span></span>  <br/> |<span data-ttu-id="7f459-123">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="7f459-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="7f459-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7f459-124">Validation file</span></span>  <br/> |<span data-ttu-id="7f459-125">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="7f459-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7f459-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="7f459-126">Can be empty</span></span>  <br/> |<span data-ttu-id="7f459-127">false</span><span class="sxs-lookup"><span data-stu-id="7f459-127">false</span></span>  <br/> |
   

