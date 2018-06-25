---
title: FolderChanges
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
description: FolderChanges 要素は、フォルダーの変更のコレクションを表します。
ms.openlocfilehash: 7ab89e79f6babb5e93863974835685c6975d96dd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760553"
---
# <a name="folderchanges"></a><span data-ttu-id="bc413-103">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="bc413-103">FolderChanges</span></span>

<span data-ttu-id="bc413-104">**FolderChanges**要素は、フォルダーの変更のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="bc413-104">The **FolderChanges** element represents a collection of changes for a folder.</span></span> 
  
[<span data-ttu-id="bc413-105">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="bc413-105">UpdateFolder</span></span>](updatefolder.md)
  
[<span data-ttu-id="bc413-106">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="bc413-106">FolderChanges</span></span>](folderchanges.md)
  
```xml
<FolderChanges>
   <FolderChange/>
</FolderChanges>
```

 <span data-ttu-id="bc413-107">**NonEmptyArrayOfFolderChangesType**</span><span class="sxs-lookup"><span data-stu-id="bc413-107">**NonEmptyArrayOfFolderChangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bc413-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="bc413-108">Attributes and elements</span></span>

<span data-ttu-id="bc413-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="bc413-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bc413-110">属性</span><span class="sxs-lookup"><span data-stu-id="bc413-110">Attributes</span></span>

<span data-ttu-id="bc413-111">なし。</span><span class="sxs-lookup"><span data-stu-id="bc413-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bc413-112">子要素</span><span class="sxs-lookup"><span data-stu-id="bc413-112">Child elements</span></span>

|<span data-ttu-id="bc413-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="bc413-113">**Element**</span></span>|<span data-ttu-id="bc413-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="bc413-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bc413-115">FolderChange</span><span class="sxs-lookup"><span data-stu-id="bc413-115">FolderChange</span></span>](folderchange.md) <br/> |<span data-ttu-id="bc413-116">1 つのフォルダーに対して実行する 1 つの変更を表します。</span><span class="sxs-lookup"><span data-stu-id="bc413-116">Represents a single change to be performed on a single folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bc413-117">親要素</span><span class="sxs-lookup"><span data-stu-id="bc413-117">Parent elements</span></span>

|<span data-ttu-id="bc413-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="bc413-118">**Element**</span></span>|<span data-ttu-id="bc413-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="bc413-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bc413-120">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="bc413-120">UpdateFolder</span></span>](updatefolder.md) <br/> |<span data-ttu-id="bc413-121">フォルダーのプロパティを更新するために使用される演算を表します。</span><span class="sxs-lookup"><span data-stu-id="bc413-121">Represents the operation that is used to update properties for a folder.</span></span>  <br/> <span data-ttu-id="bc413-122">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="bc413-122">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateFolder` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bc413-123">備考</span><span class="sxs-lookup"><span data-stu-id="bc413-123">Remarks</span></span>

<span data-ttu-id="bc413-124">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="bc413-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bc413-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="bc413-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bc413-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="bc413-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bc413-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="bc413-127">Schema Name</span></span>  <br/> |<span data-ttu-id="bc413-128">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="bc413-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bc413-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="bc413-129">Validation File</span></span>  <br/> |<span data-ttu-id="bc413-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="bc413-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bc413-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="bc413-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="bc413-132">False</span><span class="sxs-lookup"><span data-stu-id="bc413-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bc413-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="bc413-133">See also</span></span>



<span data-ttu-id="bc413-134">
  [UpdateFolder 操作](updatefolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="bc413-134">[UpdateFolder operation](updatefolder-operation.md)</span></span>

