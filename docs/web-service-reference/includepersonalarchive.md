---
title: Includeパーソナルアーカイブ
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b373bb1a-6b1d-4959-98a1-4c4ea62973bc
description: Includeな Archive 要素は、検索に個人用アーカイブを含めるかどうかを指定します。
ms.openlocfilehash: a25dd45bc0717af8f949d14b88793af3821ca69f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458251"
---
# <a name="includepersonalarchive"></a><span data-ttu-id="b66c3-103">Includeパーソナルアーカイブ</span><span class="sxs-lookup"><span data-stu-id="b66c3-103">IncludePersonalArchive</span></span>

<span data-ttu-id="b66c3-104">**Includeな archive**要素は、検索に個人用アーカイブを含めるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="b66c3-104">The **IncludePersonalArchive** element specifies whether to include the personal archive in the search.</span></span> 
  
```XML
<IncludePersonalArchive>true | false</IncludePersonalArchive>
```

 <span data-ttu-id="b66c3-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="b66c3-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b66c3-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b66c3-106">Attributes and elements</span></span>

<span data-ttu-id="b66c3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b66c3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b66c3-108">属性</span><span class="sxs-lookup"><span data-stu-id="b66c3-108">Attributes</span></span>

<span data-ttu-id="b66c3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b66c3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b66c3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b66c3-110">Child elements</span></span>

<span data-ttu-id="b66c3-111">なし。</span><span class="sxs-lookup"><span data-stu-id="b66c3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b66c3-112">親要素</span><span class="sxs-lookup"><span data-stu-id="b66c3-112">Parent elements</span></span>

|<span data-ttu-id="b66c3-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="b66c3-113">**Element**</span></span>|<span data-ttu-id="b66c3-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="b66c3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b66c3-115">FindMailboxStatisticsByKeywords</span><span class="sxs-lookup"><span data-stu-id="b66c3-115">FindMailboxStatisticsByKeywords</span></span>](findmailboxstatisticsbykeywords.md) <br/> |<span data-ttu-id="b66c3-116">キーワードでメールボックス統計情報を検索する要求を指定します。</span><span class="sxs-lookup"><span data-stu-id="b66c3-116">Specifies a request to search for mailbox statistics by keyword.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b66c3-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b66c3-117">Text value</span></span>

<span data-ttu-id="b66c3-118">**Includeパーソナルアーカイブ**要素のテキスト値が**true の場合**は、個人用アーカイブが検索に含まれていることを示します。</span><span class="sxs-lookup"><span data-stu-id="b66c3-118">A text value of **true** for the **IncludePersonalArchive** element indicates that the personal archive is included in the search.</span></span> <span data-ttu-id="b66c3-119">値が**false**の場合は、個人用アーカイブが検索に含まれていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="b66c3-119">A value of **false** indicates that the personal archive is not included in the search.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b66c3-120">注釈</span><span class="sxs-lookup"><span data-stu-id="b66c3-120">Remarks</span></span>

<span data-ttu-id="b66c3-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b66c3-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b66c3-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b66c3-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b66c3-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="b66c3-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b66c3-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b66c3-124">Schema Name</span></span>  <br/> |<span data-ttu-id="b66c3-125">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="b66c3-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="b66c3-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b66c3-126">Validation File</span></span>  <br/> |<span data-ttu-id="b66c3-127">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="b66c3-127">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b66c3-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b66c3-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="b66c3-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="b66c3-129">See also</span></span>



- [<span data-ttu-id="b66c3-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="b66c3-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

