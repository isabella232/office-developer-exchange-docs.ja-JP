---
title: MessageTrackingSearchResults
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MessageTrackingSearchResults
api_type:
- schema
ms.assetid: 6bf36f37-c2b3-40c1-a4df-31573ed8642a
description: MessageTrackingSearchResults 要素には、検索条件に一致するレコードの一覧が含まれています。
ms.openlocfilehash: 866cc8d4e9afa8347eb7bd0d9e9acaddc616c396
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832454"
---
# <a name="messagetrackingsearchresults"></a><span data-ttu-id="dae13-103">MessageTrackingSearchResults</span><span class="sxs-lookup"><span data-stu-id="dae13-103">MessageTrackingSearchResults</span></span>

<span data-ttu-id="dae13-104">**MessageTrackingSearchResults**要素には、検索条件に一致するレコードの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="dae13-104">The **MessageTrackingSearchResults** element contains a list of records that match the search criteria.</span></span> 
  
```XML
<MessageTrackingSearchResults>
   <MessageTrackingSearchResult/>
</MessageTrackingSearchResults>
```

 <span data-ttu-id="dae13-105">**ArrayOfFindMessageTrackingSearchResultType**</span><span class="sxs-lookup"><span data-stu-id="dae13-105">**ArrayOfFindMessageTrackingSearchResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dae13-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="dae13-106">Attributes and elements</span></span>

<span data-ttu-id="dae13-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="dae13-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dae13-108">属性</span><span class="sxs-lookup"><span data-stu-id="dae13-108">Attributes</span></span>

<span data-ttu-id="dae13-109">なし。</span><span class="sxs-lookup"><span data-stu-id="dae13-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dae13-110">子要素</span><span class="sxs-lookup"><span data-stu-id="dae13-110">Child elements</span></span>

|<span data-ttu-id="dae13-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="dae13-111">**Element**</span></span>|<span data-ttu-id="dae13-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="dae13-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dae13-113">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="dae13-113">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="dae13-114">[FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md)要素の 1 つのメッセージの結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="dae13-114">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dae13-115">親要素</span><span class="sxs-lookup"><span data-stu-id="dae13-115">Parent elements</span></span>

|<span data-ttu-id="dae13-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="dae13-116">**Element**</span></span>|<span data-ttu-id="dae13-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="dae13-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dae13-118">FindMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="dae13-118">FindMessageTrackingReportResponse</span></span>](findmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="dae13-119">状態および 1 つの結果が含まれています[FindMessageTrackingReport の操作](findmessagetrackingreport-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="dae13-119">Contains the status and result of a single [FindMessageTrackingReport operation](findmessagetrackingreport-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dae13-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="dae13-120">Text value</span></span>

<span data-ttu-id="dae13-121">なし。</span><span class="sxs-lookup"><span data-stu-id="dae13-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="dae13-122">備考</span><span class="sxs-lookup"><span data-stu-id="dae13-122">Remarks</span></span>

<span data-ttu-id="dae13-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="dae13-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dae13-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="dae13-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dae13-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="dae13-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="dae13-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="dae13-126">Schema Name</span></span>  <br/> |<span data-ttu-id="dae13-127">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="dae13-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="dae13-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="dae13-128">Validation File</span></span>  <br/> |<span data-ttu-id="dae13-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="dae13-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dae13-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="dae13-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="dae13-131">False</span><span class="sxs-lookup"><span data-stu-id="dae13-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dae13-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="dae13-132">See also</span></span>



- [<span data-ttu-id="dae13-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="dae13-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

