---
title: ArchiveSourceFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d5b6a099-3b87-44ef-a197-8198730ff72d
description: ArchiveSourceFolderId 要素は、アーカイブアイテムのソースフォルダーの Id を指定します。
ms.openlocfilehash: 403f40cb4529cf72f07b8a04c0803d757c24e470
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463385"
---
# <a name="archivesourcefolderid"></a><span data-ttu-id="2e731-103">ArchiveSourceFolderId</span><span class="sxs-lookup"><span data-stu-id="2e731-103">ArchiveSourceFolderId</span></span>

<span data-ttu-id="2e731-104">**ArchiveSourceFolderId**要素は、アーカイブアイテムのソースフォルダーの Id を指定します。</span><span class="sxs-lookup"><span data-stu-id="2e731-104">The **ArchiveSourceFolderId** element specifies the Id of the source folder for the archive item.</span></span> 
  
```XML
<ArchiveSourceFolderId>
   <FolderId/>
   <DistinguishedFolderId/>
   <AddressListId/>
</ArchiveSourceFolderId>
```

 <span data-ttu-id="2e731-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="2e731-105">**TargetFolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2e731-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="2e731-106">Attributes and elements</span></span>

<span data-ttu-id="2e731-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2e731-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2e731-108">属性</span><span class="sxs-lookup"><span data-stu-id="2e731-108">Attributes</span></span>

<span data-ttu-id="2e731-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2e731-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2e731-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2e731-110">Child elements</span></span>

<span data-ttu-id="2e731-111">[FolderId](folderid.md)  | [DistinguishedFolderId](distinguishedfolderid.md)  | [AddressListId](addresslistid.md)</span><span class="sxs-lookup"><span data-stu-id="2e731-111">[FolderId](folderid.md) | [DistinguishedFolderId](distinguishedfolderid.md) | [AddressListId](addresslistid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2e731-112">親要素</span><span class="sxs-lookup"><span data-stu-id="2e731-112">Parent elements</span></span>

[<span data-ttu-id="2e731-113">ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="2e731-113">ArchiveItem</span></span>](archiveitem.md)
  
## <a name="remarks"></a><span data-ttu-id="2e731-114">注釈</span><span class="sxs-lookup"><span data-stu-id="2e731-114">Remarks</span></span>

<span data-ttu-id="2e731-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="2e731-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2e731-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2e731-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2e731-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="2e731-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2e731-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="2e731-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2e731-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2e731-119">Schema name</span></span>  <br/> |<span data-ttu-id="2e731-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="2e731-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2e731-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2e731-121">Validation file</span></span>  <br/> |<span data-ttu-id="2e731-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="2e731-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2e731-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2e731-123">Can be empty</span></span>  <br/> |<span data-ttu-id="2e731-124">false</span><span class="sxs-lookup"><span data-stu-id="2e731-124">false</span></span>  <br/> |
   

