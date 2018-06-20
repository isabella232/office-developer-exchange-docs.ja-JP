---
title: ArchiveItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c2172e61-876a-4f76-bc9c-263c8be11429
description: ArchiveItem 要素には、ソース フォルダー Id と関連付けられているアーカイブの項目の項目 Id の配列が含まれています。
ms.openlocfilehash: 7f2d79f5a9e6798fafcf64e8b1bb680390800992
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759430"
---
# <a name="archiveitem"></a><span data-ttu-id="35986-103">ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="35986-103">ArchiveItem</span></span>

<span data-ttu-id="35986-104">**ArchiveItem**要素には、ソース フォルダー Id と関連付けられているアーカイブの項目の項目 Id の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="35986-104">The **ArchiveItem** element contains the source folder Id and an array of item Ids for the associated archive item.</span></span> 
  
```XML
<ArchiveItem>
   <ArchiveSourceFolderId/>
   <ItemIds/>
</ArchiveItem>
```

 <span data-ttu-id="35986-105">**ArchiveItemType**</span><span class="sxs-lookup"><span data-stu-id="35986-105">**ArchiveItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="35986-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="35986-106">Attributes and elements</span></span>

<span data-ttu-id="35986-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="35986-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="35986-108">属性</span><span class="sxs-lookup"><span data-stu-id="35986-108">Attributes</span></span>

<span data-ttu-id="35986-109">なし。</span><span class="sxs-lookup"><span data-stu-id="35986-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="35986-110">子要素</span><span class="sxs-lookup"><span data-stu-id="35986-110">Child elements</span></span>

<span data-ttu-id="35986-111">[ArchiveSourceFolderId](archivesourcefolderid.md) | [Itemid](itemids.md)</span><span class="sxs-lookup"><span data-stu-id="35986-111">[ArchiveSourceFolderId](archivesourcefolderid.md) | [ItemIds](itemids.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="35986-112">親要素</span><span class="sxs-lookup"><span data-stu-id="35986-112">Parent elements</span></span>

<span data-ttu-id="35986-113">なし。</span><span class="sxs-lookup"><span data-stu-id="35986-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="35986-114">備考</span><span class="sxs-lookup"><span data-stu-id="35986-114">Remarks</span></span>

<span data-ttu-id="35986-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="35986-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="35986-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="35986-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="35986-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="35986-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="35986-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="35986-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="35986-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="35986-119">Schema name</span></span>  <br/> |<span data-ttu-id="35986-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="35986-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="35986-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="35986-121">Validation file</span></span>  <br/> |<span data-ttu-id="35986-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="35986-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="35986-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="35986-123">Can be empty</span></span>  <br/> |<span data-ttu-id="35986-124">false</span><span class="sxs-lookup"><span data-stu-id="35986-124">false</span></span>  <br/> |
   

