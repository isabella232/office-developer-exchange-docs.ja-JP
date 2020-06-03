---
title: DeletedOccurrence 頻度
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeletedOccurrence
api_type:
- schema
ms.assetid: ff24ea15-0cd7-407d-a378-73ec16451870
description: DeletedOccurrence 要素は、定期的な予定表アイテムの削除されたアイテムを表します。
ms.openlocfilehash: 814a81934786963ae5e7ea3a40406834c27b64ce
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457838"
---
# <a name="deletedoccurrence"></a><span data-ttu-id="52c16-103">DeletedOccurrence 頻度</span><span class="sxs-lookup"><span data-stu-id="52c16-103">DeletedOccurrence</span></span>

<span data-ttu-id="52c16-104">**Deletedoccurrence**要素は、定期的な予定表アイテムの削除されたアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="52c16-104">The **DeletedOccurrence** element represents a deleted occurrence of a recurring calendar item.</span></span> 
  
```xml
<DeletedOccurrence>
   <Start/>
</DeletedOccurrence>
```

 <span data-ttu-id="52c16-105">**DeletedOccurrenceInfoType**</span><span class="sxs-lookup"><span data-stu-id="52c16-105">**DeletedOccurrenceInfoType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="52c16-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="52c16-106">Attributes and elements</span></span>

<span data-ttu-id="52c16-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="52c16-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="52c16-108">属性</span><span class="sxs-lookup"><span data-stu-id="52c16-108">Attributes</span></span>

<span data-ttu-id="52c16-109">なし。</span><span class="sxs-lookup"><span data-stu-id="52c16-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="52c16-110">子要素</span><span class="sxs-lookup"><span data-stu-id="52c16-110">Child elements</span></span>

|<span data-ttu-id="52c16-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="52c16-111">**Element**</span></span>|<span data-ttu-id="52c16-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="52c16-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="52c16-113">Start</span><span class="sxs-lookup"><span data-stu-id="52c16-113">Start</span></span>](start.md) <br/> |<span data-ttu-id="52c16-114">定期的な予定表アイテムの削除された予定の開始時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="52c16-114">Represents the start time of a deleted occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="52c16-115">親要素</span><span class="sxs-lookup"><span data-stu-id="52c16-115">Parent elements</span></span>

|<span data-ttu-id="52c16-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="52c16-116">**Element**</span></span>|<span data-ttu-id="52c16-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="52c16-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="52c16-118">DeletedOccurrences</span><span class="sxs-lookup"><span data-stu-id="52c16-118">DeletedOccurrences</span></span>](deletedoccurrences.md) <br/> |<span data-ttu-id="52c16-119">定期的な予定表アイテムの削除された出現の配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="52c16-119">Contains an array of deleted occurrences of a recurring calendar item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="52c16-120">注釈</span><span class="sxs-lookup"><span data-stu-id="52c16-120">Remarks</span></span>

<span data-ttu-id="52c16-121">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="52c16-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="52c16-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="52c16-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="52c16-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="52c16-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="52c16-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="52c16-124">Schema name</span></span>  <br/> |<span data-ttu-id="52c16-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="52c16-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="52c16-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="52c16-126">Validation file</span></span>  <br/> |<span data-ttu-id="52c16-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="52c16-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="52c16-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="52c16-128">Can be empty</span></span>  <br/> |<span data-ttu-id="52c16-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="52c16-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="52c16-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="52c16-130">See also</span></span>

- [<span data-ttu-id="52c16-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="52c16-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)  
- [<span data-ttu-id="52c16-132">Exchange 用 EWS リファレンス</span><span class="sxs-lookup"><span data-stu-id="52c16-132">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

