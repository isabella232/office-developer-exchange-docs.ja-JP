---
title: UpdateFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateFolder
api_type:
- schema
ms.assetid: 412d0683-2819-40c5-a0ae-f613499a7b66
description: UpdateFolder 要素は、指定されたフォルダーのプロパティを更新するために使用される操作を表します。
ms.openlocfilehash: 124ffd02a5ea2e7bf6f21cc7009dde08837906f9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457047"
---
# <a name="updatefolder"></a><span data-ttu-id="06e42-103">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="06e42-103">UpdateFolder</span></span>

<span data-ttu-id="06e42-104">**Updatefolder**要素は、指定されたフォルダーのプロパティを更新するために使用される操作を表します。</span><span class="sxs-lookup"><span data-stu-id="06e42-104">The **UpdateFolder** element represents the operation that is used to update properties for a specified folder.</span></span> 
  
```xml
<UpdateFolder>
   <FolderChanges/>
</UpdateFolder>
```

 <span data-ttu-id="06e42-105">**UpdateFolderType**</span><span class="sxs-lookup"><span data-stu-id="06e42-105">**UpdateFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="06e42-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="06e42-106">Attributes and elements</span></span>

<span data-ttu-id="06e42-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="06e42-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="06e42-108">属性</span><span class="sxs-lookup"><span data-stu-id="06e42-108">Attributes</span></span>

<span data-ttu-id="06e42-109">なし。</span><span class="sxs-lookup"><span data-stu-id="06e42-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="06e42-110">子要素</span><span class="sxs-lookup"><span data-stu-id="06e42-110">Child elements</span></span>

|<span data-ttu-id="06e42-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="06e42-111">**Element**</span></span>|<span data-ttu-id="06e42-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="06e42-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="06e42-113">FolderChanges 変更</span><span class="sxs-lookup"><span data-stu-id="06e42-113">FolderChanges</span></span>](folderchanges.md) <br/> |<span data-ttu-id="06e42-114">指定したフォルダーの変更のコレクションを格納します。</span><span class="sxs-lookup"><span data-stu-id="06e42-114">Contains a collection of changes for a specified folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="06e42-115">親要素</span><span class="sxs-lookup"><span data-stu-id="06e42-115">Parent elements</span></span>

<span data-ttu-id="06e42-116">なし。</span><span class="sxs-lookup"><span data-stu-id="06e42-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="06e42-117">注釈</span><span class="sxs-lookup"><span data-stu-id="06e42-117">Remarks</span></span>

<span data-ttu-id="06e42-118">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="06e42-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="06e42-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="06e42-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="06e42-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="06e42-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="06e42-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="06e42-121">Schema Name</span></span>  <br/> |<span data-ttu-id="06e42-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="06e42-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="06e42-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="06e42-123">Validation File</span></span>  <br/> |<span data-ttu-id="06e42-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="06e42-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="06e42-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="06e42-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="06e42-126">正しくない</span><span class="sxs-lookup"><span data-stu-id="06e42-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="06e42-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="06e42-127">See also</span></span>



<span data-ttu-id="06e42-128">
  [UpdateFolder 操作](updatefolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="06e42-128">[UpdateFolder operation](updatefolder-operation.md)</span></span>

