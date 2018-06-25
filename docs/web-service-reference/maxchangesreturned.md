---
title: MaxChangesReturned
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MaxChangesReturned
api_type:
- schema
ms.assetid: f471db84-a666-4dfa-9993-8ca9113a0384
description: MaxChangesReturned 要素では、同期の応答で返すことができる変更の最大数について説明します。
ms.openlocfilehash: c3719b12b7e3e2f83a9454c7b68432b375d78614
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832395"
---
# <a name="maxchangesreturned"></a><span data-ttu-id="0af01-103">MaxChangesReturned</span><span class="sxs-lookup"><span data-stu-id="0af01-103">MaxChangesReturned</span></span>

<span data-ttu-id="0af01-104">**MaxChangesReturned**要素では、同期の応答で返すことができる変更の最大数について説明します。</span><span class="sxs-lookup"><span data-stu-id="0af01-104">The **MaxChangesReturned** element describes the maximum number of changes that can be returned in a synchronization response.</span></span> 
  
[<span data-ttu-id="0af01-105">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="0af01-105">SyncFolderItems</span></span>](syncfolderitems.md)
  
[<span data-ttu-id="0af01-106">MaxChangesReturned</span><span class="sxs-lookup"><span data-stu-id="0af01-106">MaxChangesReturned</span></span>](maxchangesreturned.md)
  
```xml
<MaxChangesReturned/>
```

 <span data-ttu-id="0af01-107">**int**</span><span class="sxs-lookup"><span data-stu-id="0af01-107">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0af01-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="0af01-108">Attributes and elements</span></span>

<span data-ttu-id="0af01-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0af01-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0af01-110">属性</span><span class="sxs-lookup"><span data-stu-id="0af01-110">Attributes</span></span>

<span data-ttu-id="0af01-111">なし。</span><span class="sxs-lookup"><span data-stu-id="0af01-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0af01-112">子要素</span><span class="sxs-lookup"><span data-stu-id="0af01-112">Child elements</span></span>

<span data-ttu-id="0af01-113">なし。</span><span class="sxs-lookup"><span data-stu-id="0af01-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0af01-114">親要素</span><span class="sxs-lookup"><span data-stu-id="0af01-114">Parent elements</span></span>

|<span data-ttu-id="0af01-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="0af01-115">**Element**</span></span>|<span data-ttu-id="0af01-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="0af01-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0af01-117">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="0af01-117">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="0af01-118">Exchange ストア フォルダー内のアイテムを同期するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="0af01-118">Defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0af01-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="0af01-119">Text value</span></span>

<span data-ttu-id="0af01-120">テキスト値は、1 つの同期呼び出しで返される項目の最大数を示す整数を表します。</span><span class="sxs-lookup"><span data-stu-id="0af01-120">The text value represents an integer that describes the maximum number of items that are returned in a single synchronization call.</span></span> <span data-ttu-id="0af01-121">値は 1 から 512、包括的にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="0af01-121">The value must be between 1 and 512, inclusive.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0af01-122">備考</span><span class="sxs-lookup"><span data-stu-id="0af01-122">Remarks</span></span>

<span data-ttu-id="0af01-123">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="0af01-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0af01-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="0af01-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0af01-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="0af01-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0af01-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0af01-126">Schema name</span></span>  <br/> |<span data-ttu-id="0af01-127">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="0af01-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="0af01-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0af01-128">Validation file</span></span>  <br/> |<span data-ttu-id="0af01-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0af01-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0af01-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="0af01-130">Can be empty</span></span>  <br/> |<span data-ttu-id="0af01-131">False</span><span class="sxs-lookup"><span data-stu-id="0af01-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0af01-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="0af01-132">See also</span></span>



[<span data-ttu-id="0af01-133">SyncFolderItems の操作</span><span class="sxs-lookup"><span data-stu-id="0af01-133">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="0af01-134">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="0af01-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

