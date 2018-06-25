---
title: IncludeUnsearchableItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9a9bd2dc-f5b9-4b82-a6a0-f643d2951080
description: IncludeUnsearchableItems 要素を検索できない項目を含めるかどうかを指定します。
ms.openlocfilehash: 4c6b9b3752330bf914c9901d2e8f69e93546fec6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831907"
---
# <a name="includeunsearchableitems"></a><span data-ttu-id="8ef58-103">IncludeUnsearchableItems</span><span class="sxs-lookup"><span data-stu-id="8ef58-103">IncludeUnsearchableItems</span></span>

<span data-ttu-id="8ef58-104">**IncludeUnsearchableItems**要素を検索できない項目を含めるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8ef58-104">The **IncludeUnsearchableItems** element specifies whether to include items that cannot be searched.</span></span> 
  
```XML
<IncludeUnsearchableItems>true | false</IncludeUnsearchableItems>
```

 <span data-ttu-id="8ef58-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="8ef58-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8ef58-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8ef58-106">Attributes and elements</span></span>

<span data-ttu-id="8ef58-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8ef58-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8ef58-108">属性</span><span class="sxs-lookup"><span data-stu-id="8ef58-108">Attributes</span></span>

<span data-ttu-id="8ef58-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8ef58-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8ef58-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8ef58-110">Child elements</span></span>

<span data-ttu-id="8ef58-111">なし。</span><span class="sxs-lookup"><span data-stu-id="8ef58-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8ef58-112">親要素</span><span class="sxs-lookup"><span data-stu-id="8ef58-112">Parent elements</span></span>

|<span data-ttu-id="8ef58-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="8ef58-113">**Element**</span></span>|<span data-ttu-id="8ef58-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="8ef58-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8ef58-115">FindMailboxStatisticsByKeywords</span><span class="sxs-lookup"><span data-stu-id="8ef58-115">FindMailboxStatisticsByKeywords</span></span>](findmailboxstatisticsbykeywords.md) <br/> |<span data-ttu-id="8ef58-116">キーワードでメールボックスの統計情報を検索するための要求を指定します。</span><span class="sxs-lookup"><span data-stu-id="8ef58-116">Specifies a request to search for mailbox statistics by keyword.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8ef58-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8ef58-117">Text value</span></span>

<span data-ttu-id="8ef58-118">の**場合は true** 、 **IncludeUnsearchableItems**要素のテキスト値は、統計情報が検索可能ではない項目に含まれていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="8ef58-118">A text value of **true** for the **IncludeUnsearchableItems** element indicates that statistics are not included for items that are not searchable.</span></span> <span data-ttu-id="8ef58-119">**False**の値は、統計情報は、検索可能ではない項目に含まれていることを示します。</span><span class="sxs-lookup"><span data-stu-id="8ef58-119">A value of **false** indicates that statistics are included for items that are not searchable.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="8ef58-120">備考</span><span class="sxs-lookup"><span data-stu-id="8ef58-120">Remarks</span></span>

<span data-ttu-id="8ef58-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="8ef58-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8ef58-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="8ef58-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8ef58-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="8ef58-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8ef58-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="8ef58-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8ef58-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8ef58-125">Schema Name</span></span>  <br/> |<span data-ttu-id="8ef58-126">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="8ef58-126">Message schema</span></span>  <br/> |
|<span data-ttu-id="8ef58-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8ef58-127">Validation File</span></span>  <br/> |<span data-ttu-id="8ef58-128">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8ef58-128">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8ef58-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="8ef58-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="8ef58-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="8ef58-130">See also</span></span>



- [<span data-ttu-id="8ef58-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="8ef58-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

