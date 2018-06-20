---
title: '[開始日'
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cbb1320c-479e-4bd3-a462-4ab14c24b1c5
description: 開始要素は、メッセージが送信された日付を指定します。
ms.openlocfilehash: edc3f8ada87c64ccc3eeeb8a7467e7e050a30ce1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760613"
---
# <a name="fromdate"></a><span data-ttu-id="530ab-103">[開始日</span><span class="sxs-lookup"><span data-stu-id="530ab-103">FromDate</span></span>

<span data-ttu-id="530ab-104">**開始**要素は、メッセージが送信された日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="530ab-104">The **FromDate** element specifies the date that the message was sent.</span></span> 
  
```XML
<FromDate></FromDate>
```

 <span data-ttu-id="530ab-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="530ab-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="530ab-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="530ab-106">Attributes and elements</span></span>

<span data-ttu-id="530ab-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="530ab-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="530ab-108">属性</span><span class="sxs-lookup"><span data-stu-id="530ab-108">Attributes</span></span>

<span data-ttu-id="530ab-109">なし。</span><span class="sxs-lookup"><span data-stu-id="530ab-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="530ab-110">子要素</span><span class="sxs-lookup"><span data-stu-id="530ab-110">Child elements</span></span>

<span data-ttu-id="530ab-111">なし。</span><span class="sxs-lookup"><span data-stu-id="530ab-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="530ab-112">親要素</span><span class="sxs-lookup"><span data-stu-id="530ab-112">Parent elements</span></span>

|<span data-ttu-id="530ab-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="530ab-113">**Element**</span></span>|<span data-ttu-id="530ab-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="530ab-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="530ab-115">FindMailboxStatisticsByKeywords</span><span class="sxs-lookup"><span data-stu-id="530ab-115">FindMailboxStatisticsByKeywords</span></span>](findmailboxstatisticsbykeywords.md) <br/> |<span data-ttu-id="530ab-116">キーワードでメールボックスの統計情報を検索するための要求を指定します。</span><span class="sxs-lookup"><span data-stu-id="530ab-116">Specifies a request to search for mailbox statistics by keyword.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="530ab-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="530ab-117">Text value</span></span>

<span data-ttu-id="530ab-118">**開始**要素のテキスト値は、メッセージが送信されたときの日時です。</span><span class="sxs-lookup"><span data-stu-id="530ab-118">The text value of the **FromDate** element is the date and time that a message was sent.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="530ab-119">備考</span><span class="sxs-lookup"><span data-stu-id="530ab-119">Remarks</span></span>

<span data-ttu-id="530ab-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="530ab-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="530ab-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="530ab-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="530ab-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="530ab-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="530ab-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="530ab-123">Schema Name</span></span>  <br/> |<span data-ttu-id="530ab-124">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="530ab-124">Message schema</span></span>  <br/> |
|<span data-ttu-id="530ab-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="530ab-125">Validation File</span></span>  <br/> |<span data-ttu-id="530ab-126">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="530ab-126">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="530ab-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="530ab-127">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="530ab-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="530ab-128">See also</span></span>



- [<span data-ttu-id="530ab-129">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="530ab-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

