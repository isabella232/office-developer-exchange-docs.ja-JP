---
title: ArchiveItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c2172e61-876a-4f76-bc9c-263c8be11429
description: アーカイブアイテム要素には、ソースフォルダー Id と、関連付けられたアーカイブアイテムのアイテム Id の配列が含まれています。
ms.openlocfilehash: e1694619c90160084980cb8f3a7c8a0ed1876295
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463406"
---
# <a name="archiveitem"></a><span data-ttu-id="e7bac-103">ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="e7bac-103">ArchiveItem</span></span>

<span data-ttu-id="e7bac-104">アーカイブ**アイテム要素には、** ソースフォルダー Id と、関連付けられたアーカイブアイテムのアイテム id の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e7bac-104">The **ArchiveItem** element contains the source folder Id and an array of item Ids for the associated archive item.</span></span> 
  
```XML
<ArchiveItem>
   <ArchiveSourceFolderId/>
   <ItemIds/>
</ArchiveItem>
```

 <span data-ttu-id="e7bac-105">**アーカイブ Itemtype**</span><span class="sxs-lookup"><span data-stu-id="e7bac-105">**ArchiveItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e7bac-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e7bac-106">Attributes and elements</span></span>

<span data-ttu-id="e7bac-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e7bac-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e7bac-108">属性</span><span class="sxs-lookup"><span data-stu-id="e7bac-108">Attributes</span></span>

<span data-ttu-id="e7bac-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e7bac-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e7bac-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e7bac-110">Child elements</span></span>

<span data-ttu-id="e7bac-111">[ArchiveSourceFolderId](archivesourcefolderid.md)  | [Itemids](itemids.md)</span><span class="sxs-lookup"><span data-stu-id="e7bac-111">[ArchiveSourceFolderId](archivesourcefolderid.md) | [ItemIds](itemids.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e7bac-112">親要素</span><span class="sxs-lookup"><span data-stu-id="e7bac-112">Parent elements</span></span>

<span data-ttu-id="e7bac-113">なし。</span><span class="sxs-lookup"><span data-stu-id="e7bac-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e7bac-114">注釈</span><span class="sxs-lookup"><span data-stu-id="e7bac-114">Remarks</span></span>

<span data-ttu-id="e7bac-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e7bac-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e7bac-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e7bac-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e7bac-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e7bac-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e7bac-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="e7bac-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e7bac-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e7bac-119">Schema name</span></span>  <br/> |<span data-ttu-id="e7bac-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="e7bac-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e7bac-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e7bac-121">Validation file</span></span>  <br/> |<span data-ttu-id="e7bac-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="e7bac-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e7bac-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e7bac-123">Can be empty</span></span>  <br/> |<span data-ttu-id="e7bac-124">false</span><span class="sxs-lookup"><span data-stu-id="e7bac-124">false</span></span>  <br/> |
   

