---
title: FolderClass
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderClass
api_type:
- schema
ms.assetid: 0041d135-2869-4612-89a5-d1aa86aa1093
description: FolderClass 要素は、フォルダーのフォルダークラスを表します。
ms.openlocfilehash: ee5d382251a66ab5fbcd8054e6b5cfac82b5f994
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460058"
---
# <a name="folderclass"></a><span data-ttu-id="8760e-103">FolderClass</span><span class="sxs-lookup"><span data-stu-id="8760e-103">FolderClass</span></span>

<span data-ttu-id="8760e-104">**Folderclass**要素は、フォルダーのフォルダークラスを表します。</span><span class="sxs-lookup"><span data-stu-id="8760e-104">The **FolderClass** element represents the folder class for a folder.</span></span> 
  
```xml
<FolderClass/>
```

 <span data-ttu-id="8760e-105">**string**</span><span class="sxs-lookup"><span data-stu-id="8760e-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8760e-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="8760e-106">Attributes and elements</span></span>

<span data-ttu-id="8760e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8760e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8760e-108">属性</span><span class="sxs-lookup"><span data-stu-id="8760e-108">Attributes</span></span>

<span data-ttu-id="8760e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8760e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8760e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8760e-110">Child elements</span></span>

<span data-ttu-id="8760e-111">なし。</span><span class="sxs-lookup"><span data-stu-id="8760e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8760e-112">親要素</span><span class="sxs-lookup"><span data-stu-id="8760e-112">Parent elements</span></span>

|<span data-ttu-id="8760e-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="8760e-113">**Element**</span></span>|<span data-ttu-id="8760e-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="8760e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8760e-115">Folder</span><span class="sxs-lookup"><span data-stu-id="8760e-115">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="8760e-116">メールボックス内のフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="8760e-116">Represents a folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="8760e-117">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="8760e-117">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="8760e-118">メールボックス内の予定表フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="8760e-118">Represents a calendar folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="8760e-119">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="8760e-119">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="8760e-120">メールボックス内の連絡先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="8760e-120">Represents a contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="8760e-121">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="8760e-121">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="8760e-122">メールボックス内の検索フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="8760e-122">Represents a search folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="8760e-123">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="8760e-123">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="8760e-124">メールボックス内のタスクフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="8760e-124">Represents a task folder in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8760e-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8760e-125">Text value</span></span>

<span data-ttu-id="8760e-126">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="8760e-126">A text value is required.</span></span> <span data-ttu-id="8760e-127">通常、フォルダークラスは "IPF" で始まります。</span><span class="sxs-lookup"><span data-stu-id="8760e-127">Folder classes typically start with "IPF."</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8760e-128">注釈</span><span class="sxs-lookup"><span data-stu-id="8760e-128">Remarks</span></span>

<span data-ttu-id="8760e-129">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="8760e-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8760e-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="8760e-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8760e-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="8760e-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8760e-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8760e-132">Schema Name</span></span>  <br/> |<span data-ttu-id="8760e-133">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="8760e-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="8760e-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8760e-134">Validation File</span></span>  <br/> |<span data-ttu-id="8760e-135">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="8760e-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8760e-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="8760e-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="8760e-137">正しくない</span><span class="sxs-lookup"><span data-stu-id="8760e-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8760e-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="8760e-138">See also</span></span>



- [<span data-ttu-id="8760e-139">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="8760e-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

