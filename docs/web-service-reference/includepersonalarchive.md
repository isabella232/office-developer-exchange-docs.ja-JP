---
title: IncludePersonalArchive
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b373bb1a-6b1d-4959-98a1-4c4ea62973bc
description: IncludePersonalArchive 要素では、個人用アーカイブを検索に含めるかどうかを指定します。
ms.openlocfilehash: ba2dcaae3befd3595815c7281858e4fa8a738e0a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831905"
---
# <a name="includepersonalarchive"></a><span data-ttu-id="439d0-103">IncludePersonalArchive</span><span class="sxs-lookup"><span data-stu-id="439d0-103">IncludePersonalArchive</span></span>

<span data-ttu-id="439d0-104">**IncludePersonalArchive**要素では、個人用アーカイブを検索に含めるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="439d0-104">The **IncludePersonalArchive** element specifies whether to include the personal archive in the search.</span></span> 
  
```XML
<IncludePersonalArchive>true | false</IncludePersonalArchive>
```

 <span data-ttu-id="439d0-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="439d0-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="439d0-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="439d0-106">Attributes and elements</span></span>

<span data-ttu-id="439d0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="439d0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="439d0-108">属性</span><span class="sxs-lookup"><span data-stu-id="439d0-108">Attributes</span></span>

<span data-ttu-id="439d0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="439d0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="439d0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="439d0-110">Child elements</span></span>

<span data-ttu-id="439d0-111">なし。</span><span class="sxs-lookup"><span data-stu-id="439d0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="439d0-112">親要素</span><span class="sxs-lookup"><span data-stu-id="439d0-112">Parent elements</span></span>

|<span data-ttu-id="439d0-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="439d0-113">**Element**</span></span>|<span data-ttu-id="439d0-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="439d0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="439d0-115">FindMailboxStatisticsByKeywords</span><span class="sxs-lookup"><span data-stu-id="439d0-115">FindMailboxStatisticsByKeywords</span></span>](findmailboxstatisticsbykeywords.md) <br/> |<span data-ttu-id="439d0-116">キーワードでメールボックスの統計情報を検索するための要求を指定します。</span><span class="sxs-lookup"><span data-stu-id="439d0-116">Specifies a request to search for mailbox statistics by keyword.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="439d0-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="439d0-117">Text value</span></span>

<span data-ttu-id="439d0-118">の**場合は true** 、 **IncludePersonalArchive**要素のテキスト値では、個人用アーカイブが検索対象に含まれていることを示します。</span><span class="sxs-lookup"><span data-stu-id="439d0-118">A text value of **true** for the **IncludePersonalArchive** element indicates that the personal archive is included in the search.</span></span> <span data-ttu-id="439d0-119">**False**の値は、個人用アーカイブが検索対象に含まれていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="439d0-119">A value of **false** indicates that the personal archive is not included in the search.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="439d0-120">備考</span><span class="sxs-lookup"><span data-stu-id="439d0-120">Remarks</span></span>

<span data-ttu-id="439d0-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="439d0-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="439d0-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="439d0-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="439d0-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="439d0-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="439d0-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="439d0-124">Schema Name</span></span>  <br/> |<span data-ttu-id="439d0-125">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="439d0-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="439d0-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="439d0-126">Validation File</span></span>  <br/> |<span data-ttu-id="439d0-127">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="439d0-127">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="439d0-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="439d0-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="439d0-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="439d0-129">See also</span></span>



- [<span data-ttu-id="439d0-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="439d0-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

