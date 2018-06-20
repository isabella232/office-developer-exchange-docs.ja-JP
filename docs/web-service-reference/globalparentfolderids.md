---
title: GlobalParentFolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8f5fcbcb-05ed-462a-99cf-a6b112a4aef6
description: GlobalParentFolderIds 要素は、グローバルの親フォルダーの識別子を指定します。
ms.openlocfilehash: b0ff9ab00f3e46351b5a2db9bc4b6282fa4385cd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831747"
---
# <a name="globalparentfolderids"></a><span data-ttu-id="18913-103">GlobalParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="18913-103">GlobalParentFolderIds</span></span>

<span data-ttu-id="18913-104">**GlobalParentFolderIds**要素は、グローバルの親フォルダーの識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="18913-104">The **GlobalParentFolderIds** element specifies the identifiers of the global parent folders.</span></span> 
  
```XML
<GlobalParentFolderIds>
    <FolderId/>
    <DistinguishedFolderId/>
</GlobalParentFolderIds>
```

 <span data-ttu-id="18913-105">**NonEmptyArrayOfBaseFolderIdsType**</span><span class="sxs-lookup"><span data-stu-id="18913-105">**NonEmptyArrayOfBaseFolderIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="18913-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="18913-106">Attributes and elements</span></span>

<span data-ttu-id="18913-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="18913-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="18913-108">属性</span><span class="sxs-lookup"><span data-stu-id="18913-108">Attributes</span></span>

<span data-ttu-id="18913-109">なし。</span><span class="sxs-lookup"><span data-stu-id="18913-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="18913-110">子要素</span><span class="sxs-lookup"><span data-stu-id="18913-110">Child elements</span></span>

|<span data-ttu-id="18913-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="18913-111">**Element**</span></span>|<span data-ttu-id="18913-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="18913-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="18913-113">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="18913-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="18913-114">フォルダーの識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="18913-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="18913-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="18913-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="18913-116">名前で参照可能なフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="18913-116">Identifies folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="18913-117">親要素</span><span class="sxs-lookup"><span data-stu-id="18913-117">Parent elements</span></span>

|<span data-ttu-id="18913-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="18913-118">**Element**</span></span>|<span data-ttu-id="18913-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="18913-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="18913-120">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="18913-120">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="18913-121">1 つのテーマを表します。</span><span class="sxs-lookup"><span data-stu-id="18913-121">Represents a single conversation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="18913-122">備考</span><span class="sxs-lookup"><span data-stu-id="18913-122">Remarks</span></span>

<span data-ttu-id="18913-123">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="18913-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="18913-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="18913-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="18913-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="18913-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="18913-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="18913-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="18913-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="18913-127">Schema Name</span></span>  <br/> |<span data-ttu-id="18913-128">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="18913-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="18913-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="18913-129">Validation File</span></span>  <br/> |<span data-ttu-id="18913-130">types.xsd</span><span class="sxs-lookup"><span data-stu-id="18913-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="18913-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="18913-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="18913-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="18913-132">See also</span></span>



- [<span data-ttu-id="18913-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="18913-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

