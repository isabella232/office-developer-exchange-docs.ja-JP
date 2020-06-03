---
title: SearchArchiveOnly
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cce5344c-b622-44d4-bc14-a0de346c9335
description: SearchArchiveOnly 要素は、インデックス付けされていないアイテムに対してアーカイブメールボックスのみを検索するかどうかを示します。
ms.openlocfilehash: 9014044ed06c697cc43dd62103d7a1a907bda5a8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460499"
---
# <a name="searcharchiveonly"></a><span data-ttu-id="27ce7-103">SearchArchiveOnly</span><span class="sxs-lookup"><span data-stu-id="27ce7-103">SearchArchiveOnly</span></span>

<span data-ttu-id="27ce7-104">**SearchArchiveOnly**要素は、インデックス付けされていないアイテムに対してアーカイブメールボックスのみを検索するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="27ce7-104">The **SearchArchiveOnly** element indicates whether only the archive mailbox is searched for non-indexable items.</span></span> 
  
```xml
<SearchArchiveOnly>true | false</SearchArchiveOnly>
```

 <span data-ttu-id="27ce7-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="27ce7-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="27ce7-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="27ce7-106">Attributes and elements</span></span>

<span data-ttu-id="27ce7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="27ce7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="27ce7-108">属性</span><span class="sxs-lookup"><span data-stu-id="27ce7-108">Attributes</span></span>

<span data-ttu-id="27ce7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="27ce7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="27ce7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="27ce7-110">Child elements</span></span>

<span data-ttu-id="27ce7-111">なし。</span><span class="sxs-lookup"><span data-stu-id="27ce7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="27ce7-112">親要素</span><span class="sxs-lookup"><span data-stu-id="27ce7-112">Parent elements</span></span>

<span data-ttu-id="27ce7-113">[Getnonindexableitemstatistics](getnonindexableitemstatistics.md) │ [getnonindexableitemstatistics](getnonindexableitemdetails.md)</span><span class="sxs-lookup"><span data-stu-id="27ce7-113">[GetNonIndexableItemStatistics](getnonindexableitemstatistics.md) │ [GetNonIndexableItemDetails](getnonindexableitemdetails.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="27ce7-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="27ce7-114">Text value</span></span>

<span data-ttu-id="27ce7-115">**SearchArchiveOnly**要素のテキスト値が**true**の場合、インデックス付けされていないアイテムの検索はアーカイブメールボックスでのみ実行されることを示します。</span><span class="sxs-lookup"><span data-stu-id="27ce7-115">A text value of **true** for the **SearchArchiveOnly** element indicates that non-indexable item search is only performed on the archive mailbox.</span></span> <span data-ttu-id="27ce7-116">テキスト値が**false**の場合は、検索がプライマリメールボックスとアーカイブメールボックスに対して実行されることを示します。</span><span class="sxs-lookup"><span data-stu-id="27ce7-116">A text value of **false** indicates that the search is performed against the primary mailbox and archive mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="27ce7-117">注釈</span><span class="sxs-lookup"><span data-stu-id="27ce7-117">Remarks</span></span>

<span data-ttu-id="27ce7-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="27ce7-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="27ce7-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="27ce7-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="27ce7-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="27ce7-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="27ce7-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="27ce7-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="27ce7-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="27ce7-122">Schema name</span></span>  <br/> |<span data-ttu-id="27ce7-123">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="27ce7-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="27ce7-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="27ce7-124">Validation file</span></span>  <br/> |<span data-ttu-id="27ce7-125">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="27ce7-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="27ce7-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="27ce7-126">Can be empty</span></span>  <br/> ||
   

