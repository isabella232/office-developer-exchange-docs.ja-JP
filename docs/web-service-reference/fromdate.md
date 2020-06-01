---
title: FromDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cbb1320c-479e-4bd3-a462-4ab14c24b1c5
description: FromDate 要素は、メッセージが送信された日付を指定します。
ms.openlocfilehash: c08873a11915f4e82ad5b6f62423d0abdb9a429b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463063"
---
# <a name="fromdate"></a><span data-ttu-id="5b1e6-103">FromDate</span><span class="sxs-lookup"><span data-stu-id="5b1e6-103">FromDate</span></span>

<span data-ttu-id="5b1e6-104">**FromDate**要素は、メッセージが送信された日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="5b1e6-104">The **FromDate** element specifies the date that the message was sent.</span></span> 
  
```XML
<FromDate></FromDate>
```

 <span data-ttu-id="5b1e6-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="5b1e6-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5b1e6-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="5b1e6-106">Attributes and elements</span></span>

<span data-ttu-id="5b1e6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5b1e6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5b1e6-108">属性</span><span class="sxs-lookup"><span data-stu-id="5b1e6-108">Attributes</span></span>

<span data-ttu-id="5b1e6-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5b1e6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5b1e6-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5b1e6-110">Child elements</span></span>

<span data-ttu-id="5b1e6-111">なし。</span><span class="sxs-lookup"><span data-stu-id="5b1e6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5b1e6-112">親要素</span><span class="sxs-lookup"><span data-stu-id="5b1e6-112">Parent elements</span></span>

|<span data-ttu-id="5b1e6-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="5b1e6-113">**Element**</span></span>|<span data-ttu-id="5b1e6-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="5b1e6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5b1e6-115">FindMailboxStatisticsByKeywords</span><span class="sxs-lookup"><span data-stu-id="5b1e6-115">FindMailboxStatisticsByKeywords</span></span>](findmailboxstatisticsbykeywords.md) <br/> |<span data-ttu-id="5b1e6-116">キーワードでメールボックス統計情報を検索する要求を指定します。</span><span class="sxs-lookup"><span data-stu-id="5b1e6-116">Specifies a request to search for mailbox statistics by keyword.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5b1e6-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="5b1e6-117">Text value</span></span>

<span data-ttu-id="5b1e6-118">**FromDate**要素のテキスト値は、メッセージが送信された日付と時刻です。</span><span class="sxs-lookup"><span data-stu-id="5b1e6-118">The text value of the **FromDate** element is the date and time that a message was sent.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="5b1e6-119">注釈</span><span class="sxs-lookup"><span data-stu-id="5b1e6-119">Remarks</span></span>

<span data-ttu-id="5b1e6-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="5b1e6-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5b1e6-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="5b1e6-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5b1e6-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="5b1e6-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5b1e6-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5b1e6-123">Schema Name</span></span>  <br/> |<span data-ttu-id="5b1e6-124">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="5b1e6-124">Message schema</span></span>  <br/> |
|<span data-ttu-id="5b1e6-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5b1e6-125">Validation File</span></span>  <br/> |<span data-ttu-id="5b1e6-126">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="5b1e6-126">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5b1e6-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="5b1e6-127">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="5b1e6-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="5b1e6-128">See also</span></span>



- [<span data-ttu-id="5b1e6-129">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="5b1e6-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

