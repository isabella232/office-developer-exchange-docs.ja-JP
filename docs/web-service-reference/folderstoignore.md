---
title: FoldersToIgnore
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b5d18516-a617-4daf-8baf-c7ce29c76f6b
description: FoldersToIgnore 要素は、会話でアイテムを取得するときに無視されるフォルダーの一覧を識別します。 無視されたフォルダー内のすべての会話項目は GetConversationItems の応答に返されません。
ms.openlocfilehash: 96c094996c601e685dc1c7e6b869a790ce7d74a1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760580"
---
# <a name="folderstoignore"></a><span data-ttu-id="2b400-104">FoldersToIgnore</span><span class="sxs-lookup"><span data-stu-id="2b400-104">FoldersToIgnore</span></span>

<span data-ttu-id="2b400-105">**FoldersToIgnore**要素は、会話でアイテムを取得するときに無視されるフォルダーの一覧を識別します。</span><span class="sxs-lookup"><span data-stu-id="2b400-105">The **FoldersToIgnore** element identifies a list of folders that are ignored when getting items in a conversation.</span></span> <span data-ttu-id="2b400-106">無視されたフォルダー内のすべての会話項目は**GetConversationItems**の応答に返されません。</span><span class="sxs-lookup"><span data-stu-id="2b400-106">All conversation items in the ignored folders are not returned in a **GetConversationItems** response.</span></span> 
  
```XML
<FoldersToIgnore>
   <FolderId/>
   <DistinguishedFolderId/>
</FoldersToIgnore>
```

 <span data-ttu-id="2b400-107">**NonEmptyArrayOfBaseFolderIdsType**</span><span class="sxs-lookup"><span data-stu-id="2b400-107">**NonEmptyArrayOfBaseFolderIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2b400-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2b400-108">Attributes and elements</span></span>

<span data-ttu-id="2b400-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2b400-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2b400-110">属性</span><span class="sxs-lookup"><span data-stu-id="2b400-110">Attributes</span></span>

<span data-ttu-id="2b400-111">なし。</span><span class="sxs-lookup"><span data-stu-id="2b400-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2b400-112">子要素</span><span class="sxs-lookup"><span data-stu-id="2b400-112">Child elements</span></span>

<span data-ttu-id="2b400-113">[フォルダー Id](folderid.md) | [DistinguishedFolderId](distinguishedfolderid.md)</span><span class="sxs-lookup"><span data-stu-id="2b400-113">[FolderId](folderid.md) | [DistinguishedFolderId](distinguishedfolderid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2b400-114">親要素</span><span class="sxs-lookup"><span data-stu-id="2b400-114">Parent elements</span></span>

[<span data-ttu-id="2b400-115">GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="2b400-115">GetConversationItems</span></span>](getconversationitems.md)
  
## <a name="remarks"></a><span data-ttu-id="2b400-116">備考</span><span class="sxs-lookup"><span data-stu-id="2b400-116">Remarks</span></span>

<span data-ttu-id="2b400-117">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="2b400-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2b400-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2b400-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2b400-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="2b400-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2b400-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="2b400-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2b400-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2b400-121">Schema name</span></span>  <br/> |<span data-ttu-id="2b400-122">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="2b400-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="2b400-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2b400-123">Validation file</span></span>  <br/> |<span data-ttu-id="2b400-124">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2b400-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2b400-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2b400-125">Can be empty</span></span>  <br/> |<span data-ttu-id="2b400-126">false</span><span class="sxs-lookup"><span data-stu-id="2b400-126">false</span></span>  <br/> |
   

