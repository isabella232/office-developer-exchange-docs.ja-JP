---
title: FolderChanges 変更
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderChanges
api_type:
- schema
ms.assetid: d3f611ed-56a4-43f8-aa65-cbd7844b827f
description: FolderChanges 要素は、フォルダーに対する変更のコレクションを表します。
ms.openlocfilehash: 5481496100512584fd0b9745ee42d5b9516bd7fb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458384"
---
# <a name="folderchanges"></a><span data-ttu-id="4bdfa-103">FolderChanges 変更</span><span class="sxs-lookup"><span data-stu-id="4bdfa-103">FolderChanges</span></span>

<span data-ttu-id="4bdfa-104">**Folderchanges**要素は、フォルダーに対する変更のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="4bdfa-104">The **FolderChanges** element represents a collection of changes for a folder.</span></span> 
  
[<span data-ttu-id="4bdfa-105">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="4bdfa-105">UpdateFolder</span></span>](updatefolder.md)
  
[<span data-ttu-id="4bdfa-106">FolderChanges 変更</span><span class="sxs-lookup"><span data-stu-id="4bdfa-106">FolderChanges</span></span>](folderchanges.md)
  
```xml
<FolderChanges>
   <FolderChange/>
</FolderChanges>
```

 <span data-ttu-id="4bdfa-107">**非 Emptyarrayoffolderchangestん**</span><span class="sxs-lookup"><span data-stu-id="4bdfa-107">**NonEmptyArrayOfFolderChangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4bdfa-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="4bdfa-108">Attributes and elements</span></span>

<span data-ttu-id="4bdfa-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4bdfa-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4bdfa-110">属性</span><span class="sxs-lookup"><span data-stu-id="4bdfa-110">Attributes</span></span>

<span data-ttu-id="4bdfa-111">なし。</span><span class="sxs-lookup"><span data-stu-id="4bdfa-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4bdfa-112">子要素</span><span class="sxs-lookup"><span data-stu-id="4bdfa-112">Child elements</span></span>

|<span data-ttu-id="4bdfa-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="4bdfa-113">**Element**</span></span>|<span data-ttu-id="4bdfa-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="4bdfa-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4bdfa-115">FolderChange</span><span class="sxs-lookup"><span data-stu-id="4bdfa-115">FolderChange</span></span>](folderchange.md) <br/> |<span data-ttu-id="4bdfa-116">単一のフォルダーに対して実行される1つの変更を表します。</span><span class="sxs-lookup"><span data-stu-id="4bdfa-116">Represents a single change to be performed on a single folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4bdfa-117">親要素</span><span class="sxs-lookup"><span data-stu-id="4bdfa-117">Parent elements</span></span>

|<span data-ttu-id="4bdfa-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="4bdfa-118">**Element**</span></span>|<span data-ttu-id="4bdfa-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="4bdfa-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4bdfa-120">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="4bdfa-120">UpdateFolder</span></span>](updatefolder.md) <br/> |<span data-ttu-id="4bdfa-121">フォルダーのプロパティを更新するために使用される操作を表します。</span><span class="sxs-lookup"><span data-stu-id="4bdfa-121">Represents the operation that is used to update properties for a folder.</span></span>  <br/> <span data-ttu-id="4bdfa-122">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4bdfa-122">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateFolder` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4bdfa-123">注釈</span><span class="sxs-lookup"><span data-stu-id="4bdfa-123">Remarks</span></span>

<span data-ttu-id="4bdfa-124">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="4bdfa-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4bdfa-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="4bdfa-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4bdfa-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="4bdfa-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4bdfa-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4bdfa-127">Schema Name</span></span>  <br/> |<span data-ttu-id="4bdfa-128">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="4bdfa-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4bdfa-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4bdfa-129">Validation File</span></span>  <br/> |<span data-ttu-id="4bdfa-130">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="4bdfa-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4bdfa-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4bdfa-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="4bdfa-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="4bdfa-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4bdfa-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="4bdfa-133">See also</span></span>



<span data-ttu-id="4bdfa-134">
  [UpdateFolder 操作](updatefolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="4bdfa-134">[UpdateFolder operation](updatefolder-operation.md)</span></span>

