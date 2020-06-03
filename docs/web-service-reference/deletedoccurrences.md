---
title: DeletedOccurrences
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeletedOccurrences
api_type:
- schema
ms.assetid: 736fb305-9528-4be8-ad37-65d7556edbf2
description: DeletedOccurrences 要素には、定期的な予定表アイテムの削除された出現の配列が含まれています。
ms.openlocfilehash: be39ff95b5529481a36b7549e638818a20e01283
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463707"
---
# <a name="deletedoccurrences"></a><span data-ttu-id="6eee6-103">DeletedOccurrences</span><span class="sxs-lookup"><span data-stu-id="6eee6-103">DeletedOccurrences</span></span>

<span data-ttu-id="6eee6-104">**DeletedOccurrences**要素には、定期的な予定表アイテムの削除された出現の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6eee6-104">The **DeletedOccurrences** element contains an array of deleted occurrences of a recurring calendar item.</span></span> 
  
```xml
<DeletedOccurrences>
   <DeletedOccurrence/>
</DeletedOccurrences>
```

 <span data-ttu-id="6eee6-105">**非 Emptyarrayofdeletedocofencestype**</span><span class="sxs-lookup"><span data-stu-id="6eee6-105">**NonEmptyArrayOfDeletedOccurrencesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6eee6-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6eee6-106">Attributes and elements</span></span>

<span data-ttu-id="6eee6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6eee6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6eee6-108">属性</span><span class="sxs-lookup"><span data-stu-id="6eee6-108">Attributes</span></span>

<span data-ttu-id="6eee6-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6eee6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6eee6-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6eee6-110">Child elements</span></span>

|<span data-ttu-id="6eee6-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="6eee6-111">**Element**</span></span>|<span data-ttu-id="6eee6-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="6eee6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6eee6-113">DeletedOccurrence 頻度</span><span class="sxs-lookup"><span data-stu-id="6eee6-113">DeletedOccurrence</span></span>](deletedoccurrence.md) <br/> |<span data-ttu-id="6eee6-114">定期的な予定表アイテムの削除されたオカレンスを表します。</span><span class="sxs-lookup"><span data-stu-id="6eee6-114">Represents a deleted occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6eee6-115">親要素</span><span class="sxs-lookup"><span data-stu-id="6eee6-115">Parent elements</span></span>

|<span data-ttu-id="6eee6-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="6eee6-116">**Element**</span></span>|<span data-ttu-id="6eee6-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="6eee6-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6eee6-118">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="6eee6-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="6eee6-119">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="6eee6-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="6eee6-120">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="6eee6-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="6eee6-121">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="6eee6-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6eee6-122">注釈</span><span class="sxs-lookup"><span data-stu-id="6eee6-122">Remarks</span></span>

<span data-ttu-id="6eee6-123">この要素は、示す text 値が[Calendaritemtype](calendaritemtype.md)要素に使用されている場合に有効です。</span><span class="sxs-lookup"><span data-stu-id="6eee6-123">This element is valid if the RecurringMaster text value is used for the [CalendarItemType](calendaritemtype.md) element.</span></span> 
  
<span data-ttu-id="6eee6-124">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="6eee6-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6eee6-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6eee6-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6eee6-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="6eee6-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6eee6-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6eee6-127">Schema name</span></span>  <br/> |<span data-ttu-id="6eee6-128">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="6eee6-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="6eee6-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6eee6-129">Validation file</span></span>  <br/> |<span data-ttu-id="6eee6-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="6eee6-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6eee6-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6eee6-131">Can be empty</span></span>  <br/> |<span data-ttu-id="6eee6-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="6eee6-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6eee6-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="6eee6-133">See also</span></span>

- [<span data-ttu-id="6eee6-134">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="6eee6-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)  
- [<span data-ttu-id="6eee6-135">Exchange 用 EWS リファレンス</span><span class="sxs-lookup"><span data-stu-id="6eee6-135">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

