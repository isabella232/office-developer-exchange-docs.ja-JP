---
title: NonIndexableItemStatistics
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 12f2934a-008c-4236-b8b3-7c7b6b5707e2
description: NonIndexableItemStatistics 要素には、インデックスを作成できなかったアイテムの統計の配列が含まれています。
ms.openlocfilehash: 5a11bd4d7ef0c574f26580613063a885530176f9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466732"
---
# <a name="nonindexableitemstatistics"></a><span data-ttu-id="b368c-103">NonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="b368c-103">NonIndexableItemStatistics</span></span>

<span data-ttu-id="b368c-104">**Nonindexableitemstatistics**要素には、インデックスを作成できなかったアイテムの統計の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b368c-104">The **NonIndexableItemStatistics** element contains an array of statistics for items that could not be indexed.</span></span> 
  
```XML
<NonIndexableItemStatistics>
   <NonIndexableItemStatistic/>
</NonIndexableItemStatistics>
```

 <span data-ttu-id="b368c-105">**ArrayOfNonIndexableItemStatisticsType**</span><span class="sxs-lookup"><span data-stu-id="b368c-105">**ArrayOfNonIndexableItemStatisticsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b368c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b368c-106">Attributes and elements</span></span>

<span data-ttu-id="b368c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b368c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b368c-108">属性</span><span class="sxs-lookup"><span data-stu-id="b368c-108">Attributes</span></span>

<span data-ttu-id="b368c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b368c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b368c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b368c-110">Child elements</span></span>

[<span data-ttu-id="b368c-111">NonIndexableItemStatistic</span><span class="sxs-lookup"><span data-stu-id="b368c-111">NonIndexableItemStatistic</span></span>](nonindexableitemstatistic.md)
  
### <a name="parent-elements"></a><span data-ttu-id="b368c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="b368c-112">Parent elements</span></span>

<span data-ttu-id="b368c-113">[GetNonIndexableItemStatisticsResponse](getnonindexableitemstatisticsresponse.md) 、 [GetNonIndexableItemStatisticsResponseMessage](getnonindexableitemstatisticsresponsemessage.md)</span><span class="sxs-lookup"><span data-stu-id="b368c-113">[GetNonIndexableItemStatisticsResponse](getnonindexableitemstatisticsresponse.md) , [GetNonIndexableItemStatisticsResponseMessage](getnonindexableitemstatisticsresponsemessage.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b368c-114">注釈</span><span class="sxs-lookup"><span data-stu-id="b368c-114">Remarks</span></span>

<span data-ttu-id="b368c-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b368c-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b368c-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b368c-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b368c-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b368c-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b368c-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="b368c-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b368c-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b368c-119">Schema name</span></span>  <br/> |<span data-ttu-id="b368c-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="b368c-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b368c-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b368c-121">Validation file</span></span>  <br/> |<span data-ttu-id="b368c-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="b368c-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b368c-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b368c-123">Can be empty</span></span>  <br/> |<span data-ttu-id="b368c-124">正しくない</span><span class="sxs-lookup"><span data-stu-id="b368c-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b368c-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="b368c-125">See also</span></span>



[<span data-ttu-id="b368c-126">GetNonIndexableItemStatistics 操作</span><span class="sxs-lookup"><span data-stu-id="b368c-126">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)


- [<span data-ttu-id="b368c-127">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="b368c-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

