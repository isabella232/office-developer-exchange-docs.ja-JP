---
title: StartDateTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StartDateTime
api_type:
- schema
ms.assetid: 6fd41b7b-6c83-43b6-8b16-0bdb3d173d73
description: StartDateTime 要素は、ルールまたは検索の開始日時を指定します。
ms.openlocfilehash: 28b78fad87abb1148cfe49fee4f9bb98f822eae5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462844"
---
# <a name="startdatetime"></a><span data-ttu-id="479f1-103">StartDateTime</span><span class="sxs-lookup"><span data-stu-id="479f1-103">StartDateTime</span></span>

<span data-ttu-id="479f1-104">**StartDateTime**要素は、ルールまたは検索の開始日時を指定します。</span><span class="sxs-lookup"><span data-stu-id="479f1-104">The **StartDateTime** element specifies the start date and time for a rule or a search.</span></span> 
  
```XML
<StartDate/>
```

<span data-ttu-id="479f1-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="479f1-105">**dateTime**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="479f1-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="479f1-106">Attributes and elements</span></span>

<span data-ttu-id="479f1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="479f1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="479f1-108">属性</span><span class="sxs-lookup"><span data-stu-id="479f1-108">Attributes</span></span>

<span data-ttu-id="479f1-109">なし。</span><span class="sxs-lookup"><span data-stu-id="479f1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="479f1-110">子要素</span><span class="sxs-lookup"><span data-stu-id="479f1-110">Child elements</span></span>

<span data-ttu-id="479f1-111">なし。</span><span class="sxs-lookup"><span data-stu-id="479f1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="479f1-112">親要素</span><span class="sxs-lookup"><span data-stu-id="479f1-112">Parent elements</span></span>

|<span data-ttu-id="479f1-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="479f1-113">**Element**</span></span>|<span data-ttu-id="479f1-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="479f1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="479f1-115">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="479f1-115">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="479f1-116">検索するメッセージの種類の条件を指定します。</span><span class="sxs-lookup"><span data-stu-id="479f1-116">Specifies criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="479f1-117">WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="479f1-117">WithinDateRange</span></span>](withindaterange.md) <br/> |<span data-ttu-id="479f1-118">条件または例外を適用するために、受信メッセージが受信される必要がある日付範囲を指定します。</span><span class="sxs-lookup"><span data-stu-id="479f1-118">Specifies the date range within which incoming messages have to have been received in order for the condition or exception to apply.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="479f1-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="479f1-119">Text value</span></span>

 <span data-ttu-id="479f1-120">この要素を使用する場合は、日付/時刻を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="479f1-120">A text value that represents a date/time is required if this element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="479f1-121">注釈</span><span class="sxs-lookup"><span data-stu-id="479f1-121">Remarks</span></span>

<span data-ttu-id="479f1-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="479f1-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="479f1-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="479f1-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="479f1-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="479f1-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="479f1-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="479f1-125">Schema Name</span></span>  <br/> |<span data-ttu-id="479f1-126">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="479f1-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="479f1-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="479f1-127">Validation File</span></span>  <br/> |<span data-ttu-id="479f1-128">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="479f1-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="479f1-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="479f1-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="479f1-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="479f1-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="479f1-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="479f1-131">See also</span></span>

- [<span data-ttu-id="479f1-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="479f1-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

