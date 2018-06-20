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
description: UpdateFolder 要素は、指定したフォルダーのプロパティを更新するために使用される演算を表します。
ms.openlocfilehash: 9a86bf6b3b5917600b3b09f23b3ee4e9cdc0364f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839837"
---
# <a name="updatefolder"></a><span data-ttu-id="99ca5-103">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="99ca5-103">UpdateFolder</span></span>

<span data-ttu-id="99ca5-104">**UpdateFolder**要素は、指定したフォルダーのプロパティを更新するために使用される演算を表します。</span><span class="sxs-lookup"><span data-stu-id="99ca5-104">The **UpdateFolder** element represents the operation that is used to update properties for a specified folder.</span></span> 
  
```xml
<UpdateFolder>
   <FolderChanges/>
</UpdateFolder>
```

 <span data-ttu-id="99ca5-105">**UpdateFolderType**</span><span class="sxs-lookup"><span data-stu-id="99ca5-105">**UpdateFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="99ca5-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="99ca5-106">Attributes and elements</span></span>

<span data-ttu-id="99ca5-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="99ca5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="99ca5-108">属性</span><span class="sxs-lookup"><span data-stu-id="99ca5-108">Attributes</span></span>

<span data-ttu-id="99ca5-109">なし。</span><span class="sxs-lookup"><span data-stu-id="99ca5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="99ca5-110">子要素</span><span class="sxs-lookup"><span data-stu-id="99ca5-110">Child elements</span></span>

|<span data-ttu-id="99ca5-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="99ca5-111">**Element**</span></span>|<span data-ttu-id="99ca5-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="99ca5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="99ca5-113">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="99ca5-113">FolderChanges</span></span>](folderchanges.md) <br/> |<span data-ttu-id="99ca5-114">指定したフォルダーの変更のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="99ca5-114">Contains a collection of changes for a specified folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="99ca5-115">親要素</span><span class="sxs-lookup"><span data-stu-id="99ca5-115">Parent elements</span></span>

<span data-ttu-id="99ca5-116">なし。</span><span class="sxs-lookup"><span data-stu-id="99ca5-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="99ca5-117">備考</span><span class="sxs-lookup"><span data-stu-id="99ca5-117">Remarks</span></span>

<span data-ttu-id="99ca5-118">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="99ca5-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="99ca5-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="99ca5-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="99ca5-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="99ca5-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="99ca5-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="99ca5-121">Schema Name</span></span>  <br/> |<span data-ttu-id="99ca5-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="99ca5-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="99ca5-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="99ca5-123">Validation File</span></span>  <br/> |<span data-ttu-id="99ca5-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="99ca5-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="99ca5-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="99ca5-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="99ca5-126">False</span><span class="sxs-lookup"><span data-stu-id="99ca5-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="99ca5-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="99ca5-127">See also</span></span>



<span data-ttu-id="99ca5-128">
  [UpdateFolder 操作](updatefolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="99ca5-128">[UpdateFolder operation](updatefolder-operation.md)</span></span>

