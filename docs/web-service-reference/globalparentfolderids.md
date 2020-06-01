---
title: GlobalParentFolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8f5fcbcb-05ed-462a-99cf-a6b112a4aef6
description: GlobalParentFolderIds 要素は、グローバル親フォルダーの識別子を指定します。
ms.openlocfilehash: 11c520fa0f4a1ed6d6c9d694b407e39cd036b9cd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459098"
---
# <a name="globalparentfolderids"></a><span data-ttu-id="6fd6d-103">GlobalParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="6fd6d-103">GlobalParentFolderIds</span></span>

<span data-ttu-id="6fd6d-104">**GlobalParentFolderIds**要素は、グローバル親フォルダーの識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="6fd6d-104">The **GlobalParentFolderIds** element specifies the identifiers of the global parent folders.</span></span> 
  
```XML
<GlobalParentFolderIds>
    <FolderId/>
    <DistinguishedFolderId/>
</GlobalParentFolderIds>
```

 <span data-ttu-id="6fd6d-105">**非 Emptyarrayofbasefolderidstype**</span><span class="sxs-lookup"><span data-stu-id="6fd6d-105">**NonEmptyArrayOfBaseFolderIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6fd6d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6fd6d-106">Attributes and elements</span></span>

<span data-ttu-id="6fd6d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6fd6d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6fd6d-108">属性</span><span class="sxs-lookup"><span data-stu-id="6fd6d-108">Attributes</span></span>

<span data-ttu-id="6fd6d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6fd6d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6fd6d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6fd6d-110">Child elements</span></span>

|<span data-ttu-id="6fd6d-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="6fd6d-111">**Element**</span></span>|<span data-ttu-id="6fd6d-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="6fd6d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6fd6d-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="6fd6d-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="6fd6d-114">フォルダーの識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6fd6d-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="6fd6d-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="6fd6d-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="6fd6d-116">名前で参照できるフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="6fd6d-116">Identifies folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6fd6d-117">親要素</span><span class="sxs-lookup"><span data-stu-id="6fd6d-117">Parent elements</span></span>

|<span data-ttu-id="6fd6d-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="6fd6d-118">**Element**</span></span>|<span data-ttu-id="6fd6d-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="6fd6d-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6fd6d-120">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="6fd6d-120">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="6fd6d-121">単一の会話を表します。</span><span class="sxs-lookup"><span data-stu-id="6fd6d-121">Represents a single conversation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6fd6d-122">注釈</span><span class="sxs-lookup"><span data-stu-id="6fd6d-122">Remarks</span></span>

<span data-ttu-id="6fd6d-123">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6fd6d-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6fd6d-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6fd6d-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6fd6d-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6fd6d-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6fd6d-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="6fd6d-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6fd6d-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6fd6d-127">Schema Name</span></span>  <br/> |<span data-ttu-id="6fd6d-128">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="6fd6d-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="6fd6d-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6fd6d-129">Validation File</span></span>  <br/> |<span data-ttu-id="6fd6d-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="6fd6d-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="6fd6d-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6fd6d-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="6fd6d-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="6fd6d-132">See also</span></span>



- [<span data-ttu-id="6fd6d-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="6fd6d-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

