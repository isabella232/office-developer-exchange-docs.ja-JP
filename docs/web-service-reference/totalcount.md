---
title: TotalCount
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TotalCount
api_type:
- schema
ms.assetid: c48c6388-8449-4622-bc38-6f0e84293872
description: TotalCount 要素は、指定したフォルダー内のアイテムの合計数を表します。
ms.openlocfilehash: 3d068b558cddf73265b6bbff9fb0760738e54cec
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467523"
---
# <a name="totalcount"></a><span data-ttu-id="a53a9-103">TotalCount</span><span class="sxs-lookup"><span data-stu-id="a53a9-103">TotalCount</span></span>

<span data-ttu-id="a53a9-104">**Totalcount**要素は、指定したフォルダー内のアイテムの合計数を表します。</span><span class="sxs-lookup"><span data-stu-id="a53a9-104">The **TotalCount** element represents the total count of items within a given folder.</span></span> 
  
```xml
<TotalCount/>
```

 <span data-ttu-id="a53a9-105">**int**</span><span class="sxs-lookup"><span data-stu-id="a53a9-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a53a9-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a53a9-106">Attributes and elements</span></span>

<span data-ttu-id="a53a9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a53a9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a53a9-108">属性</span><span class="sxs-lookup"><span data-stu-id="a53a9-108">Attributes</span></span>

<span data-ttu-id="a53a9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a53a9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a53a9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a53a9-110">Child elements</span></span>

<span data-ttu-id="a53a9-111">なし。</span><span class="sxs-lookup"><span data-stu-id="a53a9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a53a9-112">親要素</span><span class="sxs-lookup"><span data-stu-id="a53a9-112">Parent elements</span></span>

|<span data-ttu-id="a53a9-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="a53a9-113">**Element**</span></span>|<span data-ttu-id="a53a9-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="a53a9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a53a9-115">Folder</span><span class="sxs-lookup"><span data-stu-id="a53a9-115">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="a53a9-116">メールボックス内のフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="a53a9-116">Represents a folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="a53a9-117">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="a53a9-117">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="a53a9-118">メールボックス内の予定表フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="a53a9-118">Represents a calendar folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="a53a9-119">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="a53a9-119">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="a53a9-120">メールボックス内の連絡先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="a53a9-120">Represents a contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="a53a9-121">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="a53a9-121">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="a53a9-122">メールボックス内の検索フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="a53a9-122">Represents a search folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="a53a9-123">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="a53a9-123">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="a53a9-124">メールボックス内のタスクフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="a53a9-124">Represents a task folder in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a53a9-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a53a9-125">Text value</span></span>

<span data-ttu-id="a53a9-126">テキスト値は、整数値を表します。</span><span class="sxs-lookup"><span data-stu-id="a53a9-126">The text value represents an integer value.</span></span> <span data-ttu-id="a53a9-127">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="a53a9-127">This property is read-only.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a53a9-128">注釈</span><span class="sxs-lookup"><span data-stu-id="a53a9-128">Remarks</span></span>

<span data-ttu-id="a53a9-129">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="a53a9-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a53a9-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a53a9-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a53a9-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="a53a9-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a53a9-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a53a9-132">Schema Name</span></span>  <br/> |<span data-ttu-id="a53a9-133">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="a53a9-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="a53a9-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a53a9-134">Validation File</span></span>  <br/> |<span data-ttu-id="a53a9-135">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="a53a9-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a53a9-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a53a9-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="a53a9-137">正しくない</span><span class="sxs-lookup"><span data-stu-id="a53a9-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a53a9-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="a53a9-138">See also</span></span>



- [<span data-ttu-id="a53a9-139">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="a53a9-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

