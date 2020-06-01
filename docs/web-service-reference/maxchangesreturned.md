---
title: Maxの戻り値
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
description: Maxchanges 返される要素は、同期応答で返すことができる変更の最大数を示します。
ms.openlocfilehash: caf96b6e95f2e63d0e544ead26fbea18cd637861
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460086"
---
# <a name="maxchangesreturned"></a><span data-ttu-id="b5807-103">Maxの戻り値</span><span class="sxs-lookup"><span data-stu-id="b5807-103">MaxChangesReturned</span></span>

<span data-ttu-id="b5807-104">**Maxchanges 返さ**れる要素は、同期応答で返すことができる変更の最大数を示します。</span><span class="sxs-lookup"><span data-stu-id="b5807-104">The **MaxChangesReturned** element describes the maximum number of changes that can be returned in a synchronization response.</span></span> 
  
[<span data-ttu-id="b5807-105">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="b5807-105">SyncFolderItems</span></span>](syncfolderitems.md)
  
[<span data-ttu-id="b5807-106">Maxの戻り値</span><span class="sxs-lookup"><span data-stu-id="b5807-106">MaxChangesReturned</span></span>](maxchangesreturned.md)
  
```xml
<MaxChangesReturned/>
```

 <span data-ttu-id="b5807-107">**int**</span><span class="sxs-lookup"><span data-stu-id="b5807-107">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b5807-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b5807-108">Attributes and elements</span></span>

<span data-ttu-id="b5807-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b5807-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b5807-110">属性</span><span class="sxs-lookup"><span data-stu-id="b5807-110">Attributes</span></span>

<span data-ttu-id="b5807-111">なし。</span><span class="sxs-lookup"><span data-stu-id="b5807-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b5807-112">子要素</span><span class="sxs-lookup"><span data-stu-id="b5807-112">Child elements</span></span>

<span data-ttu-id="b5807-113">なし。</span><span class="sxs-lookup"><span data-stu-id="b5807-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b5807-114">親要素</span><span class="sxs-lookup"><span data-stu-id="b5807-114">Parent elements</span></span>

|<span data-ttu-id="b5807-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="b5807-115">**Element**</span></span>|<span data-ttu-id="b5807-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="b5807-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b5807-117">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="b5807-117">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="b5807-118">Exchange ストアフォルダー内のアイテムを同期する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="b5807-118">Defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b5807-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b5807-119">Text value</span></span>

<span data-ttu-id="b5807-120">テキスト値は、単一の同期呼び出しで返されるアイテムの最大数を示す整数を表します。</span><span class="sxs-lookup"><span data-stu-id="b5807-120">The text value represents an integer that describes the maximum number of items that are returned in a single synchronization call.</span></span> <span data-ttu-id="b5807-121">この値は、1 ~ 512 の範囲にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="b5807-121">The value must be between 1 and 512, inclusive.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b5807-122">注釈</span><span class="sxs-lookup"><span data-stu-id="b5807-122">Remarks</span></span>

<span data-ttu-id="b5807-123">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="b5807-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b5807-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b5807-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b5807-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="b5807-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b5807-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b5807-126">Schema name</span></span>  <br/> |<span data-ttu-id="b5807-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="b5807-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="b5807-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b5807-128">Validation file</span></span>  <br/> |<span data-ttu-id="b5807-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="b5807-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b5807-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b5807-130">Can be empty</span></span>  <br/> |<span data-ttu-id="b5807-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="b5807-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b5807-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="b5807-132">See also</span></span>



[<span data-ttu-id="b5807-133">SyncFolderItems 操作</span><span class="sxs-lookup"><span data-stu-id="b5807-133">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="b5807-134">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="b5807-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

