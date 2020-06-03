---
title: DisplayName (文字列)
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
description: DisplayName 要素は、フォルダー、連絡先、配布リスト、代理人のユーザー、場所、またはルールの表示名を定義します。
ms.openlocfilehash: 9b566ec1938ec206e45cddf9c7f00083af2d8a9c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463617"
---
# <a name="displayname-string"></a><span data-ttu-id="8d220-103">DisplayName (文字列)</span><span class="sxs-lookup"><span data-stu-id="8d220-103">DisplayName (string)</span></span>

<span data-ttu-id="8d220-104">**DisplayName**要素は、フォルダー、連絡先、配布リスト、代理人のユーザー、場所、またはルールの表示名を定義します。</span><span class="sxs-lookup"><span data-stu-id="8d220-104">The **DisplayName** element defines the display name of a folder, contact, distribution list, delegate user, location, or rule.</span></span> 
  
```XML
<DisplayName/>
```

 <span data-ttu-id="8d220-105">**String**</span><span class="sxs-lookup"><span data-stu-id="8d220-105">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8d220-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="8d220-106">Attributes and elements</span></span>

<span data-ttu-id="8d220-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8d220-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8d220-108">属性</span><span class="sxs-lookup"><span data-stu-id="8d220-108">Attributes</span></span>

<span data-ttu-id="8d220-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8d220-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8d220-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8d220-110">Child elements</span></span>

<span data-ttu-id="8d220-111">なし。</span><span class="sxs-lookup"><span data-stu-id="8d220-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8d220-112">親要素</span><span class="sxs-lookup"><span data-stu-id="8d220-112">Parent elements</span></span>

|<span data-ttu-id="8d220-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="8d220-113">**Element**</span></span>|<span data-ttu-id="8d220-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="8d220-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8d220-115">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="8d220-115">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="8d220-116">メールボックス内の予定表フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="8d220-116">Represents a calendar folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="8d220-117">Contact</span><span class="sxs-lookup"><span data-stu-id="8d220-117">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="8d220-118">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="8d220-118">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="8d220-119">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="8d220-119">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="8d220-120">メールボックス内の連絡先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="8d220-120">Represents a contact folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="8d220-121">DistributionList</span><span class="sxs-lookup"><span data-stu-id="8d220-121">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="8d220-122">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="8d220-122">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="8d220-123">Folder</span><span class="sxs-lookup"><span data-stu-id="8d220-123">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="8d220-124">メールボックス内のフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="8d220-124">Represents a folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="8d220-125">ルール (RuleType)</span><span class="sxs-lookup"><span data-stu-id="8d220-125">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="8d220-126">ユーザーのメールボックス内のルールを表します。</span><span class="sxs-lookup"><span data-stu-id="8d220-126">Represents a rule in a user's mailbox.</span></span>  <br/> |
|[<span data-ttu-id="8d220-127">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="8d220-127">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="8d220-128">メールボックス内の検索フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="8d220-128">Represents a search folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="8d220-129">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="8d220-129">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="8d220-130">メールボックス内のタスクフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="8d220-130">Represents a task folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="8d220-131">UserId</span><span class="sxs-lookup"><span data-stu-id="8d220-131">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="8d220-132">代理ユーザーまたはフォルダーのアクセス許可を持つユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="8d220-132">Identifies a delegate user or a user who has folder access permissions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8d220-133">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8d220-133">Text value</span></span>

<span data-ttu-id="8d220-134">この要素を使用する場合は、表示名を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="8d220-134">A text value that represents the display name is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8d220-135">注釈</span><span class="sxs-lookup"><span data-stu-id="8d220-135">Remarks</span></span>

<span data-ttu-id="8d220-136">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="8d220-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="8d220-137">例</span><span class="sxs-lookup"><span data-stu-id="8d220-137">Example</span></span>

<span data-ttu-id="8d220-138">次の例は、新しいフォルダーを作成し、フォルダーの DisplayName を "TestFolder" に設定する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="8d220-138">This following example shows how to create a new folder and to set the DisplayName of the folder to "TestFolder".</span></span>
  
```cs
FolderType folder = new FolderType();
folder.DisplayName = "TestFolder";
```

## <a name="element-information"></a><span data-ttu-id="8d220-139">要素の情報</span><span class="sxs-lookup"><span data-stu-id="8d220-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8d220-140">Namespace</span><span class="sxs-lookup"><span data-stu-id="8d220-140">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8d220-141">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8d220-141">Schema name</span></span>  <br/> |<span data-ttu-id="8d220-142">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="8d220-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="8d220-143">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8d220-143">Validation file</span></span>  <br/> |<span data-ttu-id="8d220-144">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="8d220-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8d220-145">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="8d220-145">Can be empty</span></span>  <br/> |<span data-ttu-id="8d220-146">正しくない</span><span class="sxs-lookup"><span data-stu-id="8d220-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8d220-147">関連項目</span><span class="sxs-lookup"><span data-stu-id="8d220-147">See also</span></span>

- [<span data-ttu-id="8d220-148">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="8d220-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

