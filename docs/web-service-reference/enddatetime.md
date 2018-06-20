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
description: EndDateTime 要素は、ルールや検索の終了日時を指定します。
ms.openlocfilehash: ad596c6441e7bdb10b4e886a8d0f3ba183c43c3e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760293"
---
# <a name="enddatetime"></a><span data-ttu-id="4eeb3-103">EndDateTime</span><span class="sxs-lookup"><span data-stu-id="4eeb3-103">EndDateTime</span></span>

<span data-ttu-id="4eeb3-104">**EndDateTime**要素は、ルールや検索の終了日時を指定します。</span><span class="sxs-lookup"><span data-stu-id="4eeb3-104">The **EndDateTime** element specifies the end date and time for a rule or a search.</span></span> 
  
```XML
<EndDateTime/>
```

 <span data-ttu-id="4eeb3-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="4eeb3-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4eeb3-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4eeb3-106">Attributes and elements</span></span>

<span data-ttu-id="4eeb3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4eeb3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4eeb3-108">属性</span><span class="sxs-lookup"><span data-stu-id="4eeb3-108">Attributes</span></span>

<span data-ttu-id="4eeb3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4eeb3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4eeb3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4eeb3-110">Child elements</span></span>

<span data-ttu-id="4eeb3-111">なし。</span><span class="sxs-lookup"><span data-stu-id="4eeb3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4eeb3-112">親要素</span><span class="sxs-lookup"><span data-stu-id="4eeb3-112">Parent elements</span></span>

|<span data-ttu-id="4eeb3-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="4eeb3-113">**Element**</span></span>|<span data-ttu-id="4eeb3-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="4eeb3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4eeb3-115">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="4eeb3-115">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="4eeb3-116">検索するメッセージの種類の条件が含まれています。</span><span class="sxs-lookup"><span data-stu-id="4eeb3-116">Contains criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="4eeb3-117">WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="4eeb3-117">WithinDateRange</span></span>](withindaterange.md) <br/> |<span data-ttu-id="4eeb3-118">受信したメッセージが適用の条件または例外のために到着した日付の範囲を指定します。</span><span class="sxs-lookup"><span data-stu-id="4eeb3-118">Specifies the date range within which incoming messages have to have been received in order for the condition or exception to apply.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4eeb3-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="4eeb3-119">Text value</span></span>

<span data-ttu-id="4eeb3-120">日付と時刻を表すテキスト値は、この要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="4eeb3-120">A text value that represents a date/time is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4eeb3-121">備考</span><span class="sxs-lookup"><span data-stu-id="4eeb3-121">Remarks</span></span>

<span data-ttu-id="4eeb3-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="4eeb3-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4eeb3-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="4eeb3-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4eeb3-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="4eeb3-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4eeb3-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4eeb3-125">Schema Name</span></span>  <br/> |<span data-ttu-id="4eeb3-126">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="4eeb3-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4eeb3-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4eeb3-127">Validation File</span></span>  <br/> |<span data-ttu-id="4eeb3-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4eeb3-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4eeb3-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4eeb3-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="4eeb3-130">False</span><span class="sxs-lookup"><span data-stu-id="4eeb3-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4eeb3-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="4eeb3-131">See also</span></span>



- [<span data-ttu-id="4eeb3-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="4eeb3-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

