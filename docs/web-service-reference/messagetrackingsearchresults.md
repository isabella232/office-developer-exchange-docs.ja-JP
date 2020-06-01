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
ms.openlocfilehash: 1e03cb135b7b2a125da1e29f7293d233f4e20ddb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468678"
---
# <a name="messagetrackingsearchresults"></a><span data-ttu-id="01c85-103">MessageTrackingSearchResults</span><span class="sxs-lookup"><span data-stu-id="01c85-103">MessageTrackingSearchResults</span></span>

<span data-ttu-id="01c85-104">**Messagetrackingsearchresults**要素には、検索条件に一致するレコードの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="01c85-104">The **MessageTrackingSearchResults** element contains a list of records that match the search criteria.</span></span> 
  
```XML
<MessageTrackingSearchResults>
   <MessageTrackingSearchResult/>
</MessageTrackingSearchResults>
```

 <span data-ttu-id="01c85-105">**ArrayOfFindMessageTrackingSearchResultType**</span><span class="sxs-lookup"><span data-stu-id="01c85-105">**ArrayOfFindMessageTrackingSearchResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="01c85-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="01c85-106">Attributes and elements</span></span>

<span data-ttu-id="01c85-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="01c85-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="01c85-108">属性</span><span class="sxs-lookup"><span data-stu-id="01c85-108">Attributes</span></span>

<span data-ttu-id="01c85-109">なし。</span><span class="sxs-lookup"><span data-stu-id="01c85-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="01c85-110">子要素</span><span class="sxs-lookup"><span data-stu-id="01c85-110">Child elements</span></span>

|<span data-ttu-id="01c85-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="01c85-111">**Element**</span></span>|<span data-ttu-id="01c85-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="01c85-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="01c85-113">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="01c85-113">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="01c85-114">[Findmessagetrackingreportresponse](findmessagetrackingreportresponse.md)要素の単一メッセージ結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="01c85-114">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="01c85-115">親要素</span><span class="sxs-lookup"><span data-stu-id="01c85-115">Parent elements</span></span>

|<span data-ttu-id="01c85-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="01c85-116">**Element**</span></span>|<span data-ttu-id="01c85-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="01c85-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="01c85-118">FindMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="01c85-118">FindMessageTrackingReportResponse</span></span>](findmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="01c85-119">単一の[Findmessagetrackingreport 操作](findmessagetrackingreport-operation.md)要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="01c85-119">Contains the status and result of a single [FindMessageTrackingReport operation](findmessagetrackingreport-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="01c85-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="01c85-120">Text value</span></span>

<span data-ttu-id="01c85-121">なし。</span><span class="sxs-lookup"><span data-stu-id="01c85-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="01c85-122">注釈</span><span class="sxs-lookup"><span data-stu-id="01c85-122">Remarks</span></span>

<span data-ttu-id="01c85-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="01c85-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="01c85-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="01c85-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="01c85-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="01c85-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="01c85-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="01c85-126">Schema Name</span></span>  <br/> |<span data-ttu-id="01c85-127">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="01c85-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="01c85-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="01c85-128">Validation File</span></span>  <br/> |<span data-ttu-id="01c85-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="01c85-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="01c85-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="01c85-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="01c85-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="01c85-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="01c85-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="01c85-132">See also</span></span>



- [<span data-ttu-id="01c85-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="01c85-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

