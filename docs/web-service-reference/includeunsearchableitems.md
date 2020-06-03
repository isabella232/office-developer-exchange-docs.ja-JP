---
title: Include非 Searchableitems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9a9bd2dc-f5b9-4b82-a6a0-f643d2951080
description: IncludeUnsearchableItems 要素は、検索できないアイテムを含めるかどうかを指定します。
ms.openlocfilehash: 19fe450f5b1647be2df75138dbe67dd9e1c05c21
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465703"
---
# <a name="includeunsearchableitems"></a><span data-ttu-id="1bc6d-103">Include非 Searchableitems</span><span class="sxs-lookup"><span data-stu-id="1bc6d-103">IncludeUnsearchableItems</span></span>

<span data-ttu-id="1bc6d-104">**Includeunsearchableitems**要素は、検索できないアイテムを含めるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="1bc6d-104">The **IncludeUnsearchableItems** element specifies whether to include items that cannot be searched.</span></span> 
  
```XML
<IncludeUnsearchableItems>true | false</IncludeUnsearchableItems>
```

 <span data-ttu-id="1bc6d-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="1bc6d-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1bc6d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1bc6d-106">Attributes and elements</span></span>

<span data-ttu-id="1bc6d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1bc6d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1bc6d-108">属性</span><span class="sxs-lookup"><span data-stu-id="1bc6d-108">Attributes</span></span>

<span data-ttu-id="1bc6d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1bc6d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1bc6d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1bc6d-110">Child elements</span></span>

<span data-ttu-id="1bc6d-111">なし。</span><span class="sxs-lookup"><span data-stu-id="1bc6d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1bc6d-112">親要素</span><span class="sxs-lookup"><span data-stu-id="1bc6d-112">Parent elements</span></span>

|<span data-ttu-id="1bc6d-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="1bc6d-113">**Element**</span></span>|<span data-ttu-id="1bc6d-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="1bc6d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1bc6d-115">FindMailboxStatisticsByKeywords</span><span class="sxs-lookup"><span data-stu-id="1bc6d-115">FindMailboxStatisticsByKeywords</span></span>](findmailboxstatisticsbykeywords.md) <br/> |<span data-ttu-id="1bc6d-116">キーワードでメールボックス統計情報を検索する要求を指定します。</span><span class="sxs-lookup"><span data-stu-id="1bc6d-116">Specifies a request to search for mailbox statistics by keyword.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1bc6d-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1bc6d-117">Text value</span></span>

<span data-ttu-id="1bc6d-118">**Include非**検索可能な items 要素のテキスト値が**true の場合**は、検索できないアイテムの統計が含まれていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="1bc6d-118">A text value of **true** for the **IncludeUnsearchableItems** element indicates that statistics are not included for items that are not searchable.</span></span> <span data-ttu-id="1bc6d-119">値が**false**の場合、検索できないアイテムの統計が含まれていることを示します。</span><span class="sxs-lookup"><span data-stu-id="1bc6d-119">A value of **false** indicates that statistics are included for items that are not searchable.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="1bc6d-120">注釈</span><span class="sxs-lookup"><span data-stu-id="1bc6d-120">Remarks</span></span>

<span data-ttu-id="1bc6d-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="1bc6d-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1bc6d-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="1bc6d-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1bc6d-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1bc6d-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1bc6d-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="1bc6d-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1bc6d-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1bc6d-125">Schema Name</span></span>  <br/> |<span data-ttu-id="1bc6d-126">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="1bc6d-126">Message schema</span></span>  <br/> |
|<span data-ttu-id="1bc6d-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1bc6d-127">Validation File</span></span>  <br/> |<span data-ttu-id="1bc6d-128">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="1bc6d-128">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1bc6d-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="1bc6d-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="1bc6d-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="1bc6d-130">See also</span></span>



- [<span data-ttu-id="1bc6d-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="1bc6d-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

