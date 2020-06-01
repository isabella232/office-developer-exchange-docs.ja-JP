---
title: GetNonIndexableItemStatistics
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dd16d1fb-d82d-42e5-b64a-bc6c19c48fa8
description: GetNonIndexableItemStatistics 要素は、インデックス付けされていないアイテムの統計情報を取得するための要求を指定します。
ms.openlocfilehash: 4b605379f20f5558566f1cfbad9ef1aa33b6fce6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44452791"
---
# <a name="getnonindexableitemstatistics"></a><span data-ttu-id="93c5d-103">GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="93c5d-103">GetNonIndexableItemStatistics</span></span>

<span data-ttu-id="93c5d-104">**Getnonindexableitemstatistics**要素は、インデックス付けされていないアイテムの統計情報を取得するための要求を指定します。</span><span class="sxs-lookup"><span data-stu-id="93c5d-104">The **GetNonIndexableItemStatistics** element specifies a request to retrieve nonindexable item statistics.</span></span> 
  
```XML
<GetNonIndexableItemStatistics>
    <Mailboxes/>
</GetNonIndexableItemStatistics>
```

 <span data-ttu-id="93c5d-105">**GetNonIndexableItemStatisticsType**</span><span class="sxs-lookup"><span data-stu-id="93c5d-105">**GetNonIndexableItemStatisticsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="93c5d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="93c5d-106">Attributes and elements</span></span>

<span data-ttu-id="93c5d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="93c5d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="93c5d-108">属性</span><span class="sxs-lookup"><span data-stu-id="93c5d-108">Attributes</span></span>

<span data-ttu-id="93c5d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="93c5d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="93c5d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="93c5d-110">Child elements</span></span>

|<span data-ttu-id="93c5d-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="93c5d-111">**Element**</span></span>|<span data-ttu-id="93c5d-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="93c5d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93c5d-113">メールボックス (NonEmptyArrayOfLegacyDNsType)</span><span class="sxs-lookup"><span data-stu-id="93c5d-113">Mailboxes (NonEmptyArrayOfLegacyDNsType)</span></span>](mailboxes-nonemptyarrayoflegacydnstype.md) <br/> |<span data-ttu-id="93c5d-114">**メールボックス**要素の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="93c5d-114">Specifies an array of **Mailbox** elements.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="93c5d-115">親要素</span><span class="sxs-lookup"><span data-stu-id="93c5d-115">Parent elements</span></span>

<span data-ttu-id="93c5d-116">なし。</span><span class="sxs-lookup"><span data-stu-id="93c5d-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="93c5d-117">注釈</span><span class="sxs-lookup"><span data-stu-id="93c5d-117">Remarks</span></span>

<span data-ttu-id="93c5d-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="93c5d-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="93c5d-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="93c5d-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="93c5d-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="93c5d-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="93c5d-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="93c5d-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="93c5d-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="93c5d-122">Schema Name</span></span>  <br/> |<span data-ttu-id="93c5d-123">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="93c5d-123">Message schema</span></span>  <br/> |
|<span data-ttu-id="93c5d-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="93c5d-124">Validation File</span></span>  <br/> |<span data-ttu-id="93c5d-125">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="93c5d-125">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="93c5d-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="93c5d-126">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="93c5d-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="93c5d-127">See also</span></span>



- [<span data-ttu-id="93c5d-128">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="93c5d-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

