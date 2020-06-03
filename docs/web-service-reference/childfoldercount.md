---
title: ChildFolderCount
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ChildFolderCount
api_type:
- schema
ms.assetid: e0e4eabd-802f-4dd0-9911-89e08c66a15e
description: ChildFolderCount 要素は、フォルダー内に含まれる直下の子フォルダーの数を表します。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。
ms.openlocfilehash: 6ea3b9c000c7836b55c6bf359c95870ed28350e0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463945"
---
# <a name="childfoldercount"></a><span data-ttu-id="9cdbd-104">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="9cdbd-104">ChildFolderCount</span></span>

<span data-ttu-id="9cdbd-105">**Childfoldercount**要素は、フォルダー内に含まれる直下の子フォルダーの数を表します。</span><span class="sxs-lookup"><span data-stu-id="9cdbd-105">The **ChildFolderCount** element represents the number of immediate child folders that are contained within a folder.</span></span> <span data-ttu-id="9cdbd-106">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="9cdbd-106">This property is read-only.</span></span> 
  
```xml
<ChildFolderCount/>
```

 <span data-ttu-id="9cdbd-107">**int**</span><span class="sxs-lookup"><span data-stu-id="9cdbd-107">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9cdbd-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9cdbd-108">Attributes and elements</span></span>

<span data-ttu-id="9cdbd-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9cdbd-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9cdbd-110">属性</span><span class="sxs-lookup"><span data-stu-id="9cdbd-110">Attributes</span></span>

<span data-ttu-id="9cdbd-111">なし。</span><span class="sxs-lookup"><span data-stu-id="9cdbd-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9cdbd-112">子要素</span><span class="sxs-lookup"><span data-stu-id="9cdbd-112">Child elements</span></span>

<span data-ttu-id="9cdbd-113">なし。</span><span class="sxs-lookup"><span data-stu-id="9cdbd-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9cdbd-114">親要素</span><span class="sxs-lookup"><span data-stu-id="9cdbd-114">Parent elements</span></span>

|<span data-ttu-id="9cdbd-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="9cdbd-115">**Element**</span></span>|<span data-ttu-id="9cdbd-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="9cdbd-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9cdbd-117">Folder</span><span class="sxs-lookup"><span data-stu-id="9cdbd-117">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="9cdbd-118">メールボックス内のフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="9cdbd-118">Represents a folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="9cdbd-119">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="9cdbd-119">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="9cdbd-120">メールボックス内の予定表フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="9cdbd-120">Represents a Calendar folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="9cdbd-121">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="9cdbd-121">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="9cdbd-122">メールボックス内の連絡先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="9cdbd-122">Represents a Contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="9cdbd-123">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="9cdbd-123">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="9cdbd-124">メールボックス内の検索フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="9cdbd-124">Represents a search folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="9cdbd-125">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="9cdbd-125">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="9cdbd-126">メールボックス内のタスクフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="9cdbd-126">Represents a Tasks folder in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9cdbd-127">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9cdbd-127">Text value</span></span>

<span data-ttu-id="9cdbd-128">テキスト値は、整数を表します。</span><span class="sxs-lookup"><span data-stu-id="9cdbd-128">The text value represents an integer.</span></span> <span data-ttu-id="9cdbd-129">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="9cdbd-129">This property is read-only.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9cdbd-130">注釈</span><span class="sxs-lookup"><span data-stu-id="9cdbd-130">Remarks</span></span>

<span data-ttu-id="9cdbd-131">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="9cdbd-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9cdbd-132">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9cdbd-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9cdbd-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="9cdbd-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9cdbd-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9cdbd-134">Schema Name</span></span>  <br/> |<span data-ttu-id="9cdbd-135">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="9cdbd-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="9cdbd-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9cdbd-136">Validation File</span></span>  <br/> |<span data-ttu-id="9cdbd-137">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="9cdbd-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9cdbd-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9cdbd-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="9cdbd-139">正しくない</span><span class="sxs-lookup"><span data-stu-id="9cdbd-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9cdbd-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="9cdbd-140">See also</span></span>



- [<span data-ttu-id="9cdbd-141">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="9cdbd-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

