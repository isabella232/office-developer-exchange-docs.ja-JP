---
title: ArchiveSourceFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d5b6a099-3b87-44ef-a197-8198730ff72d
description: ArchiveSourceFolderId 要素は、アーカイブのアイテムの元のフォルダーの Id を指定します。
ms.openlocfilehash: b7a5097de734777a71559703ed2d54199edd952e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759436"
---
# <a name="archivesourcefolderid"></a><span data-ttu-id="de79a-103">ArchiveSourceFolderId</span><span class="sxs-lookup"><span data-stu-id="de79a-103">ArchiveSourceFolderId</span></span>

<span data-ttu-id="de79a-104">**ArchiveSourceFolderId**要素は、アーカイブのアイテムの元のフォルダーの Id を指定します。</span><span class="sxs-lookup"><span data-stu-id="de79a-104">The **ArchiveSourceFolderId** element specifies the Id of the source folder for the archive item.</span></span> 
  
```XML
<ArchiveSourceFolderId>
   <FolderId/>
   <DistinguishedFolderId/>
   <AddressListId/>
</ArchiveSourceFolderId>
```

 <span data-ttu-id="de79a-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="de79a-105">**TargetFolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="de79a-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="de79a-106">Attributes and elements</span></span>

<span data-ttu-id="de79a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="de79a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="de79a-108">属性</span><span class="sxs-lookup"><span data-stu-id="de79a-108">Attributes</span></span>

<span data-ttu-id="de79a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="de79a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="de79a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="de79a-110">Child elements</span></span>

<span data-ttu-id="de79a-111">[フォルダー Id](folderid.md) | [DistinguishedFolderId](distinguishedfolderid.md) | [AddressListId](addresslistid.md)</span><span class="sxs-lookup"><span data-stu-id="de79a-111">[FolderId](folderid.md) | [DistinguishedFolderId](distinguishedfolderid.md) | [AddressListId](addresslistid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="de79a-112">親要素</span><span class="sxs-lookup"><span data-stu-id="de79a-112">Parent elements</span></span>

[<span data-ttu-id="de79a-113">ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="de79a-113">ArchiveItem</span></span>](archiveitem.md)
  
## <a name="remarks"></a><span data-ttu-id="de79a-114">備考</span><span class="sxs-lookup"><span data-stu-id="de79a-114">Remarks</span></span>

<span data-ttu-id="de79a-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="de79a-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="de79a-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="de79a-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="de79a-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="de79a-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="de79a-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="de79a-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="de79a-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="de79a-119">Schema name</span></span>  <br/> |<span data-ttu-id="de79a-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="de79a-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="de79a-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="de79a-121">Validation file</span></span>  <br/> |<span data-ttu-id="de79a-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="de79a-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="de79a-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="de79a-123">Can be empty</span></span>  <br/> |<span data-ttu-id="de79a-124">false</span><span class="sxs-lookup"><span data-stu-id="de79a-124">false</span></span>  <br/> |
   

