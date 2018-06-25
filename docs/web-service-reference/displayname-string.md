---
title: 表示名 (文字列)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DisplayName
api_type:
- schema
ms.assetid: e7efbbe1-6629-4d11-bed1-ed899e3f9d77
description: DisplayName 要素では、フォルダー、連絡先、配布リスト、ユーザーの代理人、場所、またはルールの表示名を定義します。
ms.openlocfilehash: 53f4e083d9e6617206e383d4408e08ed7ea0fe08
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760106"
---
# <a name="displayname-string"></a><span data-ttu-id="6f312-103">表示名 (文字列)</span><span class="sxs-lookup"><span data-stu-id="6f312-103">DisplayName (string)</span></span>

<span data-ttu-id="6f312-104">**DisplayName**要素では、フォルダー、連絡先、配布リスト、ユーザーの代理人、場所、またはルールの表示名を定義します。</span><span class="sxs-lookup"><span data-stu-id="6f312-104">The **DisplayName** element defines the display name of a folder, contact, distribution list, delegate user, location, or rule.</span></span> 
  
```XML
<DisplayName/>
```

 <span data-ttu-id="6f312-105">**文字列型 (String)**</span><span class="sxs-lookup"><span data-stu-id="6f312-105">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6f312-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6f312-106">Attributes and elements</span></span>

<span data-ttu-id="6f312-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6f312-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6f312-108">属性</span><span class="sxs-lookup"><span data-stu-id="6f312-108">Attributes</span></span>

<span data-ttu-id="6f312-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6f312-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6f312-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6f312-110">Child elements</span></span>

<span data-ttu-id="6f312-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6f312-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6f312-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6f312-112">Parent elements</span></span>

|<span data-ttu-id="6f312-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="6f312-113">**Element**</span></span>|<span data-ttu-id="6f312-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="6f312-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6f312-115">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="6f312-115">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="6f312-116">メールボックスの予定表フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="6f312-116">Represents a calendar folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6f312-117">Contact</span><span class="sxs-lookup"><span data-stu-id="6f312-117">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="6f312-118">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="6f312-118">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="6f312-119">メッセージ</span><span class="sxs-lookup"><span data-stu-id="6f312-119">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="6f312-120">メールボックスの連絡先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="6f312-120">Represents a contact folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6f312-121">DistributionList</span><span class="sxs-lookup"><span data-stu-id="6f312-121">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="6f312-122">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="6f312-122">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="6f312-123">Folder</span><span class="sxs-lookup"><span data-stu-id="6f312-123">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="6f312-124">メールボックス内のフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="6f312-124">Represents a folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6f312-125">ルール (RuleType)</span><span class="sxs-lookup"><span data-stu-id="6f312-125">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="6f312-126">ユーザーのメールボックス内のルールを表します。</span><span class="sxs-lookup"><span data-stu-id="6f312-126">Represents a rule in a user's mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6f312-127">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="6f312-127">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="6f312-128">メールボックス内の検索フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="6f312-128">Represents a search folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6f312-129">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="6f312-129">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="6f312-130">メールボックス内のタスク フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="6f312-130">Represents a task folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6f312-131">ユーザー Id</span><span class="sxs-lookup"><span data-stu-id="6f312-131">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="6f312-132">代理ユーザー、またはフォルダーのアクセス許可を持つユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="6f312-132">Identifies a delegate user or a user who has folder access permissions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6f312-133">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6f312-133">Text value</span></span>

<span data-ttu-id="6f312-134">表示名を表すテキスト値は、この要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="6f312-134">A text value that represents the display name is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6f312-135">備考</span><span class="sxs-lookup"><span data-stu-id="6f312-135">Remarks</span></span>

<span data-ttu-id="6f312-136">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6f312-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="6f312-137">例</span><span class="sxs-lookup"><span data-stu-id="6f312-137">Example</span></span>

<span data-ttu-id="6f312-138">[TestFolder] フォルダーの表示名を設定すると、新しいフォルダーを作成する方法を次の例に示します。</span><span class="sxs-lookup"><span data-stu-id="6f312-138">This following example shows how to create a new folder and to set the DisplayName of the folder to "TestFolder".</span></span>
  
```cs
FolderType folder = new FolderType();
folder.DisplayName = "TestFolder";
```

## <a name="element-information"></a><span data-ttu-id="6f312-139">要素情報</span><span class="sxs-lookup"><span data-stu-id="6f312-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6f312-140">名前空間</span><span class="sxs-lookup"><span data-stu-id="6f312-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6f312-141">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6f312-141">Schema name</span></span>  <br/> |<span data-ttu-id="6f312-142">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="6f312-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="6f312-143">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6f312-143">Validation file</span></span>  <br/> |<span data-ttu-id="6f312-144">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6f312-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6f312-145">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6f312-145">Can be empty</span></span>  <br/> |<span data-ttu-id="6f312-146">False</span><span class="sxs-lookup"><span data-stu-id="6f312-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6f312-147">関連項目</span><span class="sxs-lookup"><span data-stu-id="6f312-147">See also</span></span>

- [<span data-ttu-id="6f312-148">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="6f312-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

