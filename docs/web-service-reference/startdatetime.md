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
description: させる要素は、ルールや検索の開始日時を指定します。
ms.openlocfilehash: 4bc32ed5626d692fc73dfa8bd7c46923aba72f9e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833552"
---
# <a name="startdatetime"></a><span data-ttu-id="0415e-103">StartDateTime</span><span class="sxs-lookup"><span data-stu-id="0415e-103">StartDateTime</span></span>

<span data-ttu-id="0415e-104">**させる**要素は、ルールや検索の開始日時を指定します。</span><span class="sxs-lookup"><span data-stu-id="0415e-104">The **StartDateTime** element specifies the start date and time for a rule or a search.</span></span> 
  
```XML
<StartDate/>
```

<span data-ttu-id="0415e-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="0415e-105">**dateTime**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="0415e-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="0415e-106">Attributes and elements</span></span>

<span data-ttu-id="0415e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0415e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0415e-108">属性</span><span class="sxs-lookup"><span data-stu-id="0415e-108">Attributes</span></span>

<span data-ttu-id="0415e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="0415e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0415e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="0415e-110">Child elements</span></span>

<span data-ttu-id="0415e-111">なし。</span><span class="sxs-lookup"><span data-stu-id="0415e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0415e-112">親要素</span><span class="sxs-lookup"><span data-stu-id="0415e-112">Parent elements</span></span>

|<span data-ttu-id="0415e-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="0415e-113">**Element**</span></span>|<span data-ttu-id="0415e-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="0415e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0415e-115">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="0415e-115">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="0415e-116">検索するメッセージの種類の条件を指定します。</span><span class="sxs-lookup"><span data-stu-id="0415e-116">Specifies criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="0415e-117">WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="0415e-117">WithinDateRange</span></span>](withindaterange.md) <br/> |<span data-ttu-id="0415e-118">受信したメッセージが適用の条件または例外のために到着した日付の範囲を指定します。</span><span class="sxs-lookup"><span data-stu-id="0415e-118">Specifies the date range within which incoming messages have to have been received in order for the condition or exception to apply.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0415e-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="0415e-119">Text value</span></span>

 <span data-ttu-id="0415e-120">日付と時刻を表すテキスト値は、この要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="0415e-120">A text value that represents a date/time is required if this element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="0415e-121">備考</span><span class="sxs-lookup"><span data-stu-id="0415e-121">Remarks</span></span>

<span data-ttu-id="0415e-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="0415e-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0415e-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="0415e-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0415e-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="0415e-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0415e-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0415e-125">Schema Name</span></span>  <br/> |<span data-ttu-id="0415e-126">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="0415e-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0415e-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0415e-127">Validation File</span></span>  <br/> |<span data-ttu-id="0415e-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0415e-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0415e-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0415e-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="0415e-130">False</span><span class="sxs-lookup"><span data-stu-id="0415e-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0415e-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="0415e-131">See also</span></span>

- [<span data-ttu-id="0415e-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="0415e-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

