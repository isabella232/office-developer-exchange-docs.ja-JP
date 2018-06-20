---
title: GetNonIndexableItemStatistics
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dd16d1fb-d82d-42e5-b64a-bc6c19c48fa8
description: GetNonIndexableItemStatistics 要素は、nonindexable の項目の統計情報を取得する要求を指定します。
ms.openlocfilehash: 4e6f9a0ba94e9946a3910661810bc2c9e748ba9f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760798"
---
# <a name="getnonindexableitemstatistics"></a><span data-ttu-id="fdf7e-103">GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="fdf7e-103">GetNonIndexableItemStatistics</span></span>

<span data-ttu-id="fdf7e-104">**GetNonIndexableItemStatistics**要素は、nonindexable の項目の統計情報を取得する要求を指定します。</span><span class="sxs-lookup"><span data-stu-id="fdf7e-104">The **GetNonIndexableItemStatistics** element specifies a request to retrieve nonindexable item statistics.</span></span> 
  
```XML
<GetNonIndexableItemStatistics>
    <Mailboxes/>
</GetNonIndexableItemStatistics>
```

 <span data-ttu-id="fdf7e-105">**GetNonIndexableItemStatisticsType**</span><span class="sxs-lookup"><span data-stu-id="fdf7e-105">**GetNonIndexableItemStatisticsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fdf7e-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="fdf7e-106">Attributes and elements</span></span>

<span data-ttu-id="fdf7e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fdf7e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fdf7e-108">属性</span><span class="sxs-lookup"><span data-stu-id="fdf7e-108">Attributes</span></span>

<span data-ttu-id="fdf7e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="fdf7e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fdf7e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="fdf7e-110">Child elements</span></span>

|<span data-ttu-id="fdf7e-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="fdf7e-111">**Element**</span></span>|<span data-ttu-id="fdf7e-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="fdf7e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fdf7e-113">メールボックス (NonEmptyArrayOfLegacyDNsType)</span><span class="sxs-lookup"><span data-stu-id="fdf7e-113">Mailboxes (NonEmptyArrayOfLegacyDNsType)</span></span>](mailboxes-nonemptyarrayoflegacydnstype.md) <br/> |<span data-ttu-id="fdf7e-114">**メールボックス**の要素の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="fdf7e-114">Specifies an array of **Mailbox** elements.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fdf7e-115">親要素</span><span class="sxs-lookup"><span data-stu-id="fdf7e-115">Parent elements</span></span>

<span data-ttu-id="fdf7e-116">なし。</span><span class="sxs-lookup"><span data-stu-id="fdf7e-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fdf7e-117">備考</span><span class="sxs-lookup"><span data-stu-id="fdf7e-117">Remarks</span></span>

<span data-ttu-id="fdf7e-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="fdf7e-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="fdf7e-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="fdf7e-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fdf7e-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="fdf7e-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fdf7e-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="fdf7e-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fdf7e-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fdf7e-122">Schema Name</span></span>  <br/> |<span data-ttu-id="fdf7e-123">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="fdf7e-123">Message schema</span></span>  <br/> |
|<span data-ttu-id="fdf7e-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fdf7e-124">Validation File</span></span>  <br/> |<span data-ttu-id="fdf7e-125">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fdf7e-125">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fdf7e-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="fdf7e-126">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="fdf7e-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="fdf7e-127">See also</span></span>



- [<span data-ttu-id="fdf7e-128">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="fdf7e-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

