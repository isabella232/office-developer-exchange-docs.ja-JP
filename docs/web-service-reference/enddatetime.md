---
title: EndDateTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EndDateTime
api_type:
- schema
ms.assetid: 54d14e47-a8f7-400b-a859-c7ea7ce4c6a4
description: EndDateTime 要素は、ルールまたは検索の終了日時を指定します。
ms.openlocfilehash: 9556e4c1ef405ae66a71d19d99d9a71a61f54efc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460135"
---
# <a name="enddatetime"></a><span data-ttu-id="69fcb-103">EndDateTime</span><span class="sxs-lookup"><span data-stu-id="69fcb-103">EndDateTime</span></span>

<span data-ttu-id="69fcb-104">**Enddatetime**要素は、ルールまたは検索の終了日時を指定します。</span><span class="sxs-lookup"><span data-stu-id="69fcb-104">The **EndDateTime** element specifies the end date and time for a rule or a search.</span></span> 
  
```XML
<EndDateTime/>
```

 <span data-ttu-id="69fcb-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="69fcb-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="69fcb-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="69fcb-106">Attributes and elements</span></span>

<span data-ttu-id="69fcb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="69fcb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="69fcb-108">属性</span><span class="sxs-lookup"><span data-stu-id="69fcb-108">Attributes</span></span>

<span data-ttu-id="69fcb-109">なし。</span><span class="sxs-lookup"><span data-stu-id="69fcb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="69fcb-110">子要素</span><span class="sxs-lookup"><span data-stu-id="69fcb-110">Child elements</span></span>

<span data-ttu-id="69fcb-111">なし。</span><span class="sxs-lookup"><span data-stu-id="69fcb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="69fcb-112">親要素</span><span class="sxs-lookup"><span data-stu-id="69fcb-112">Parent elements</span></span>

|<span data-ttu-id="69fcb-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="69fcb-113">**Element**</span></span>|<span data-ttu-id="69fcb-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="69fcb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="69fcb-115">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="69fcb-115">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="69fcb-116">検索するメッセージの種類に関する条件を含みます。</span><span class="sxs-lookup"><span data-stu-id="69fcb-116">Contains criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="69fcb-117">WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="69fcb-117">WithinDateRange</span></span>](withindaterange.md) <br/> |<span data-ttu-id="69fcb-118">条件または例外を適用するために、受信メッセージが受信される必要がある日付範囲を指定します。</span><span class="sxs-lookup"><span data-stu-id="69fcb-118">Specifies the date range within which incoming messages have to have been received in order for the condition or exception to apply.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="69fcb-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="69fcb-119">Text value</span></span>

<span data-ttu-id="69fcb-120">この要素を使用する場合は、日付/時刻を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="69fcb-120">A text value that represents a date/time is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="69fcb-121">注釈</span><span class="sxs-lookup"><span data-stu-id="69fcb-121">Remarks</span></span>

<span data-ttu-id="69fcb-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="69fcb-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="69fcb-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="69fcb-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="69fcb-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="69fcb-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="69fcb-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="69fcb-125">Schema Name</span></span>  <br/> |<span data-ttu-id="69fcb-126">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="69fcb-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="69fcb-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="69fcb-127">Validation File</span></span>  <br/> |<span data-ttu-id="69fcb-128">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="69fcb-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="69fcb-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="69fcb-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="69fcb-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="69fcb-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="69fcb-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="69fcb-131">See also</span></span>



- [<span data-ttu-id="69fcb-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="69fcb-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

