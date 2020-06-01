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
description: ExecutedSearchScope 要素には、検索結果を取得するために実行された検索のスコープが含まれています。
ms.openlocfilehash: 828fe3800b8c13a0e18c0daba6cdeab140a1c394
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456970"
---
# <a name="executedsearchscope"></a><span data-ttu-id="c4724-103">ExecutedSearchScope</span><span class="sxs-lookup"><span data-stu-id="c4724-103">ExecutedSearchScope</span></span>

<span data-ttu-id="c4724-104">**Executedsearchscope**要素には、検索結果を取得するために実行された検索のスコープが含まれています。</span><span class="sxs-lookup"><span data-stu-id="c4724-104">The **ExecutedSearchScope** element contains the scope of the search that was performed to get the search results.</span></span> 
  
```xml
<ExecutedSearchScope/>
```

 <span data-ttu-id="c4724-105">**String**</span><span class="sxs-lookup"><span data-stu-id="c4724-105">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c4724-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c4724-106">Attributes and elements</span></span>

<span data-ttu-id="c4724-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c4724-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c4724-108">属性</span><span class="sxs-lookup"><span data-stu-id="c4724-108">Attributes</span></span>

<span data-ttu-id="c4724-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c4724-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c4724-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c4724-110">Child elements</span></span>

<span data-ttu-id="c4724-111">なし。</span><span class="sxs-lookup"><span data-stu-id="c4724-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c4724-112">親要素</span><span class="sxs-lookup"><span data-stu-id="c4724-112">Parent elements</span></span>

|<span data-ttu-id="c4724-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="c4724-113">**Element**</span></span>|<span data-ttu-id="c4724-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="c4724-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c4724-115">FindMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="c4724-115">FindMessageTrackingReportResponse</span></span>](findmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="c4724-116">単一の[Findmessagetrackingreport 操作](findmessagetrackingreport-operation.md)要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="c4724-116">Contains the status and result of a single [FindMessageTrackingReport operation](findmessagetrackingreport-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c4724-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c4724-117">Text value</span></span>

<span data-ttu-id="c4724-118">テキスト値はオプションです。</span><span class="sxs-lookup"><span data-stu-id="c4724-118">The text value is optional.</span></span> <span data-ttu-id="c4724-119">この情報は、クライアントアプリケーションが検索結果をより効果的にキャッシュするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="c4724-119">This information is used by the client application to cache the results more effectively.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c4724-120">注釈</span><span class="sxs-lookup"><span data-stu-id="c4724-120">Remarks</span></span>

<span data-ttu-id="c4724-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="c4724-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c4724-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c4724-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c4724-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="c4724-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c4724-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c4724-124">Schema Name</span></span>  <br/> |<span data-ttu-id="c4724-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="c4724-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="c4724-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c4724-126">Validation File</span></span>  <br/> |<span data-ttu-id="c4724-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="c4724-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c4724-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c4724-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="c4724-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="c4724-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c4724-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="c4724-130">See also</span></span>



[<span data-ttu-id="c4724-131">FindMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="c4724-131">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)


- [<span data-ttu-id="c4724-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="c4724-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

