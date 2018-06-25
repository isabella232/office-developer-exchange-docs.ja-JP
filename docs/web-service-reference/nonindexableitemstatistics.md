---
title: NonIndexableItemStatistics
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 12f2934a-008c-4236-b8b3-7c7b6b5707e2
description: NonIndexableItemStatistics 要素には、インデックス付けされない項目の統計情報の配列が含まれています。
ms.openlocfilehash: 1414053b6d39f4cd08ccfd1a11faaf1b13c2052b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832544"
---
# <a name="nonindexableitemstatistics"></a><span data-ttu-id="26bf5-103">NonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="26bf5-103">NonIndexableItemStatistics</span></span>

<span data-ttu-id="26bf5-104">**NonIndexableItemStatistics**要素には、インデックス付けされない項目の統計情報の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="26bf5-104">The **NonIndexableItemStatistics** element contains an array of statistics for items that could not be indexed.</span></span> 
  
```XML
<NonIndexableItemStatistics>
   <NonIndexableItemStatistic/>
</NonIndexableItemStatistics>
```

 <span data-ttu-id="26bf5-105">**ArrayOfNonIndexableItemStatisticsType**</span><span class="sxs-lookup"><span data-stu-id="26bf5-105">**ArrayOfNonIndexableItemStatisticsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="26bf5-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="26bf5-106">Attributes and elements</span></span>

<span data-ttu-id="26bf5-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="26bf5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="26bf5-108">属性</span><span class="sxs-lookup"><span data-stu-id="26bf5-108">Attributes</span></span>

<span data-ttu-id="26bf5-109">なし。</span><span class="sxs-lookup"><span data-stu-id="26bf5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="26bf5-110">子要素</span><span class="sxs-lookup"><span data-stu-id="26bf5-110">Child elements</span></span>

[<span data-ttu-id="26bf5-111">NonIndexableItemStatistic</span><span class="sxs-lookup"><span data-stu-id="26bf5-111">NonIndexableItemStatistic</span></span>](nonindexableitemstatistic.md)
  
### <a name="parent-elements"></a><span data-ttu-id="26bf5-112">親要素</span><span class="sxs-lookup"><span data-stu-id="26bf5-112">Parent elements</span></span>

<span data-ttu-id="26bf5-113">[GetNonIndexableItemStatisticsResponse](getnonindexableitemstatisticsresponse.md) 、 [GetNonIndexableItemStatisticsResponseMessage](getnonindexableitemstatisticsresponsemessage.md)</span><span class="sxs-lookup"><span data-stu-id="26bf5-113">[GetNonIndexableItemStatisticsResponse](getnonindexableitemstatisticsresponse.md) , [GetNonIndexableItemStatisticsResponseMessage](getnonindexableitemstatisticsresponsemessage.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="26bf5-114">備考</span><span class="sxs-lookup"><span data-stu-id="26bf5-114">Remarks</span></span>

<span data-ttu-id="26bf5-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="26bf5-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="26bf5-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="26bf5-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="26bf5-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="26bf5-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="26bf5-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="26bf5-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="26bf5-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="26bf5-119">Schema name</span></span>  <br/> |<span data-ttu-id="26bf5-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="26bf5-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="26bf5-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="26bf5-121">Validation file</span></span>  <br/> |<span data-ttu-id="26bf5-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="26bf5-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="26bf5-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="26bf5-123">Can be empty</span></span>  <br/> |<span data-ttu-id="26bf5-124">False</span><span class="sxs-lookup"><span data-stu-id="26bf5-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="26bf5-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="26bf5-125">See also</span></span>



[<span data-ttu-id="26bf5-126">GetNonIndexableItemStatistics 操作</span><span class="sxs-lookup"><span data-stu-id="26bf5-126">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)


- [<span data-ttu-id="26bf5-127">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="26bf5-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

