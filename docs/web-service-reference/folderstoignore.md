---
title: FoldersToIgnore
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b5d18516-a617-4daf-8baf-c7ce29c76f6b
description: FoldersToIgnore 要素は、会話内のアイテムを取得するときに無視されるフォルダーのリストを識別します。 無視されたフォルダー内のすべての会話アイテムは、GetConversationItems 応答で返されません。
ms.openlocfilehash: 07813a54a9a3afa3de23ae94f1c9b191d1cb6fac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44453358"
---
# <a name="folderstoignore"></a><span data-ttu-id="4be16-104">FoldersToIgnore</span><span class="sxs-lookup"><span data-stu-id="4be16-104">FoldersToIgnore</span></span>

<span data-ttu-id="4be16-105">**Folderstoignore**要素は、会話内のアイテムを取得するときに無視されるフォルダーのリストを識別します。</span><span class="sxs-lookup"><span data-stu-id="4be16-105">The **FoldersToIgnore** element identifies a list of folders that are ignored when getting items in a conversation.</span></span> <span data-ttu-id="4be16-106">無視されたフォルダー内のすべての会話アイテムは、 **GetConversationItems**応答で返されません。</span><span class="sxs-lookup"><span data-stu-id="4be16-106">All conversation items in the ignored folders are not returned in a **GetConversationItems** response.</span></span> 
  
```XML
<FoldersToIgnore>
   <FolderId/>
   <DistinguishedFolderId/>
</FoldersToIgnore>
```

 <span data-ttu-id="4be16-107">**非 Emptyarrayofbasefolderidstype**</span><span class="sxs-lookup"><span data-stu-id="4be16-107">**NonEmptyArrayOfBaseFolderIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4be16-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="4be16-108">Attributes and elements</span></span>

<span data-ttu-id="4be16-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4be16-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4be16-110">属性</span><span class="sxs-lookup"><span data-stu-id="4be16-110">Attributes</span></span>

<span data-ttu-id="4be16-111">なし。</span><span class="sxs-lookup"><span data-stu-id="4be16-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4be16-112">子要素</span><span class="sxs-lookup"><span data-stu-id="4be16-112">Child elements</span></span>

<span data-ttu-id="4be16-113">[FolderId](folderid.md)  | [DistinguishedFolderId](distinguishedfolderid.md)</span><span class="sxs-lookup"><span data-stu-id="4be16-113">[FolderId](folderid.md) | [DistinguishedFolderId](distinguishedfolderid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4be16-114">親要素</span><span class="sxs-lookup"><span data-stu-id="4be16-114">Parent elements</span></span>

[<span data-ttu-id="4be16-115">GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="4be16-115">GetConversationItems</span></span>](getconversationitems.md)
  
## <a name="remarks"></a><span data-ttu-id="4be16-116">注釈</span><span class="sxs-lookup"><span data-stu-id="4be16-116">Remarks</span></span>

<span data-ttu-id="4be16-117">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="4be16-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4be16-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="4be16-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4be16-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="4be16-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4be16-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="4be16-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4be16-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4be16-121">Schema name</span></span>  <br/> |<span data-ttu-id="4be16-122">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="4be16-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="4be16-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4be16-123">Validation file</span></span>  <br/> |<span data-ttu-id="4be16-124">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="4be16-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4be16-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4be16-125">Can be empty</span></span>  <br/> |<span data-ttu-id="4be16-126">false</span><span class="sxs-lookup"><span data-stu-id="4be16-126">false</span></span>  <br/> |
   

