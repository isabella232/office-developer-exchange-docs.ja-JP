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
description: FolderClass 要素は、フォルダーのフォルダー クラスを表します。
ms.openlocfilehash: 87be00563d0375abebf32159ff38d62d03112b95
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760558"
---
# <a name="folderclass"></a><span data-ttu-id="41019-103">FolderClass</span><span class="sxs-lookup"><span data-stu-id="41019-103">FolderClass</span></span>

<span data-ttu-id="41019-104">**FolderClass**要素は、フォルダーのフォルダー クラスを表します。</span><span class="sxs-lookup"><span data-stu-id="41019-104">The **FolderClass** element represents the folder class for a folder.</span></span> 
  
```xml
<FolderClass/>
```

 <span data-ttu-id="41019-105">**string**</span><span class="sxs-lookup"><span data-stu-id="41019-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="41019-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="41019-106">Attributes and elements</span></span>

<span data-ttu-id="41019-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="41019-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="41019-108">属性</span><span class="sxs-lookup"><span data-stu-id="41019-108">Attributes</span></span>

<span data-ttu-id="41019-109">なし。</span><span class="sxs-lookup"><span data-stu-id="41019-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="41019-110">子要素</span><span class="sxs-lookup"><span data-stu-id="41019-110">Child elements</span></span>

<span data-ttu-id="41019-111">なし。</span><span class="sxs-lookup"><span data-stu-id="41019-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="41019-112">親要素</span><span class="sxs-lookup"><span data-stu-id="41019-112">Parent elements</span></span>

|<span data-ttu-id="41019-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="41019-113">**Element**</span></span>|<span data-ttu-id="41019-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="41019-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="41019-115">Folder</span><span class="sxs-lookup"><span data-stu-id="41019-115">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="41019-116">メールボックス内のフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="41019-116">Represents a folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="41019-117">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="41019-117">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="41019-118">メールボックスの予定表フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="41019-118">Represents a calendar folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="41019-119">メッセージ</span><span class="sxs-lookup"><span data-stu-id="41019-119">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="41019-120">メールボックスの連絡先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="41019-120">Represents a contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="41019-121">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="41019-121">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="41019-122">メールボックス内の検索フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="41019-122">Represents a search folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="41019-123">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="41019-123">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="41019-124">メールボックス内のタスク フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="41019-124">Represents a task folder in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="41019-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="41019-125">Text value</span></span>

<span data-ttu-id="41019-126">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="41019-126">A text value is required.</span></span> <span data-ttu-id="41019-127">フォルダー クラス通常の先頭に"IPF"にします。</span><span class="sxs-lookup"><span data-stu-id="41019-127">Folder classes typically start with "IPF."</span></span>
  
## <a name="remarks"></a><span data-ttu-id="41019-128">備考</span><span class="sxs-lookup"><span data-stu-id="41019-128">Remarks</span></span>

<span data-ttu-id="41019-129">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="41019-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="41019-130">要素情報</span><span class="sxs-lookup"><span data-stu-id="41019-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="41019-131">名前空間</span><span class="sxs-lookup"><span data-stu-id="41019-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="41019-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="41019-132">Schema Name</span></span>  <br/> |<span data-ttu-id="41019-133">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="41019-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="41019-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="41019-134">Validation File</span></span>  <br/> |<span data-ttu-id="41019-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="41019-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="41019-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="41019-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="41019-137">False</span><span class="sxs-lookup"><span data-stu-id="41019-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="41019-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="41019-138">See also</span></span>



- [<span data-ttu-id="41019-139">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="41019-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

