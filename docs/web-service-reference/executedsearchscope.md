---
title: ExecutedSearchScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExecutedSearchScope
api_type:
- schema
ms.assetid: 2de5f0ad-43f2-4d38-b520-06540066564e
description: ExecutedSearchScope 要素には、検索結果を得るために実行された検索の範囲が含まれています。
ms.openlocfilehash: ece9fdfc156cedad2a9fa181897145ae4eea20a0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760367"
---
# <a name="executedsearchscope"></a><span data-ttu-id="65165-103">ExecutedSearchScope</span><span class="sxs-lookup"><span data-stu-id="65165-103">ExecutedSearchScope</span></span>

<span data-ttu-id="65165-104">**ExecutedSearchScope**要素には、検索結果を得るために実行された検索の範囲が含まれています。</span><span class="sxs-lookup"><span data-stu-id="65165-104">The **ExecutedSearchScope** element contains the scope of the search that was performed to get the search results.</span></span> 
  
```xml
<ExecutedSearchScope/>
```

 <span data-ttu-id="65165-105">**文字列型 (String)**</span><span class="sxs-lookup"><span data-stu-id="65165-105">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="65165-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="65165-106">Attributes and elements</span></span>

<span data-ttu-id="65165-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="65165-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="65165-108">属性</span><span class="sxs-lookup"><span data-stu-id="65165-108">Attributes</span></span>

<span data-ttu-id="65165-109">なし。</span><span class="sxs-lookup"><span data-stu-id="65165-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="65165-110">子要素</span><span class="sxs-lookup"><span data-stu-id="65165-110">Child elements</span></span>

<span data-ttu-id="65165-111">なし。</span><span class="sxs-lookup"><span data-stu-id="65165-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="65165-112">親要素</span><span class="sxs-lookup"><span data-stu-id="65165-112">Parent elements</span></span>

|<span data-ttu-id="65165-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="65165-113">**Element**</span></span>|<span data-ttu-id="65165-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="65165-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="65165-115">FindMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="65165-115">FindMessageTrackingReportResponse</span></span>](findmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="65165-116">状態および 1 つの結果が含まれています[FindMessageTrackingReport の操作](findmessagetrackingreport-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="65165-116">Contains the status and result of a single [FindMessageTrackingReport operation](findmessagetrackingreport-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="65165-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="65165-117">Text value</span></span>

<span data-ttu-id="65165-118">テキスト値は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="65165-118">The text value is optional.</span></span> <span data-ttu-id="65165-119">この情報より効果的に結果をキャッシュするのには、クライアント アプリケーションによって使用されます。</span><span class="sxs-lookup"><span data-stu-id="65165-119">This information is used by the client application to cache the results more effectively.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="65165-120">備考</span><span class="sxs-lookup"><span data-stu-id="65165-120">Remarks</span></span>

<span data-ttu-id="65165-121">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="65165-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="65165-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="65165-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="65165-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="65165-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="65165-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="65165-124">Schema Name</span></span>  <br/> |<span data-ttu-id="65165-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="65165-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="65165-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="65165-126">Validation File</span></span>  <br/> |<span data-ttu-id="65165-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="65165-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="65165-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="65165-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="65165-129">False</span><span class="sxs-lookup"><span data-stu-id="65165-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="65165-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="65165-130">See also</span></span>



[<span data-ttu-id="65165-131">FindMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="65165-131">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)


- [<span data-ttu-id="65165-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="65165-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

