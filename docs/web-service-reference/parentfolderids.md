---
title: ParentFolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ParentFolderIds
api_type:
- schema
ms.assetid: e7998023-e5e0-465c-91fa-2aa6d1559f64
description: ParentFolderIds 要素は、検索する FindItem および FindFolder 操作のフォルダーを識別します。
ms.openlocfilehash: 6bc4b9cfe96c6c83cbeb623ec176e33177356bbc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465430"
---
# <a name="parentfolderids"></a><span data-ttu-id="a3a5c-103">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="a3a5c-103">ParentFolderIds</span></span>

<span data-ttu-id="a3a5c-104">**ParentFolderIds**要素は、検索する FindItem および findfolder 操作のフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="a3a5c-104">The **ParentFolderIds** element identifies folders for the FindItem and FindFolder operations to search.</span></span> 
  
```xml
<ParentFolderIds>
   <DistinguishedFolderId/>
<ParentFolderIds>
```

```xml
<ParentFolderIds>
   <FolderId/> 
<ParentFolderIds>
```

<span data-ttu-id="a3a5c-105">**非 Emptyarrayofbasefolderidstype**</span><span class="sxs-lookup"><span data-stu-id="a3a5c-105">**NonEmptyArrayOfBaseFolderIdsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a3a5c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a3a5c-106">Attributes and elements</span></span>

<span data-ttu-id="a3a5c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a3a5c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a3a5c-108">属性</span><span class="sxs-lookup"><span data-stu-id="a3a5c-108">Attributes</span></span>

<span data-ttu-id="a3a5c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a3a5c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a3a5c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a3a5c-110">Child elements</span></span>

|<span data-ttu-id="a3a5c-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="a3a5c-111">**Element**</span></span>|<span data-ttu-id="a3a5c-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="a3a5c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a3a5c-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="a3a5c-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="a3a5c-114">フォルダーの識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a3a5c-114">Contains the identifier and change key of a folder.</span></span> <span data-ttu-id="a3a5c-115">**ParentFolderIds**要素では、この要素または[DistinguishedFolderId](distinguishedfolderid.md)要素のいずれかを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a3a5c-115">The **ParentFolderIds** element must use either this element or the [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="a3a5c-116">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="a3a5c-116">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="a3a5c-117">名前で参照できる Microsoft Exchange Server 2007 フォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="a3a5c-117">Identifies Microsoft Exchange Server 2007 folders that can be referenced by name.</span></span> <span data-ttu-id="a3a5c-118">**ParentFolderIds**要素では、この要素または[FolderId](folderid.md)要素のいずれかを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a3a5c-118">The **ParentFolderIds** element must use either this element or the [FolderId](folderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a3a5c-119">親要素</span><span class="sxs-lookup"><span data-stu-id="a3a5c-119">Parent elements</span></span>

|<span data-ttu-id="a3a5c-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="a3a5c-120">**Element**</span></span>|<span data-ttu-id="a3a5c-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="a3a5c-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a3a5c-122">FindFolder</span><span class="sxs-lookup"><span data-stu-id="a3a5c-122">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="a3a5c-123">メールボックス内のフォルダーを識別する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="a3a5c-123">Defines a request to identify folders in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="a3a5c-124">FindItem</span><span class="sxs-lookup"><span data-stu-id="a3a5c-124">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="a3a5c-125">メールボックス内のアイテムを検索するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="a3a5c-125">Defines a request to find items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="a3a5c-126">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="a3a5c-126">ResolveNames</span></span>](resolvenames.md) <br/> |<span data-ttu-id="a3a5c-127">あいまいな名前を解決する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="a3a5c-127">Defines a request to resolve ambiguous names.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a3a5c-128">注釈</span><span class="sxs-lookup"><span data-stu-id="a3a5c-128">Remarks</span></span>

<span data-ttu-id="a3a5c-129">**ParentFolderIds**要素では、 [FolderId](folderid.md)または[DistinguishedFolderId](distinguishedfolderid.md)要素のいずれかを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a3a5c-129">The **ParentFolderIds** element must use either the [FolderId](folderid.md) or the [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span> <span data-ttu-id="a3a5c-130">検索に対して定義できるフォルダーの数に制限はありません。</span><span class="sxs-lookup"><span data-stu-id="a3a5c-130">An unlimited number of folders can be defined for the search.</span></span> 
  
## <a name="example"></a><span data-ttu-id="a3a5c-131">例</span><span class="sxs-lookup"><span data-stu-id="a3a5c-131">Example</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>Default</t:BaseShape>
      </FolderShape>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindFolder>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="a3a5c-132">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a3a5c-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a3a5c-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="a3a5c-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a3a5c-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a3a5c-134">Schema Name</span></span>  <br/> |<span data-ttu-id="a3a5c-135">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="a3a5c-135">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a3a5c-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a3a5c-136">Validation File</span></span>  <br/> |<span data-ttu-id="a3a5c-137">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="a3a5c-137">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a3a5c-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a3a5c-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="a3a5c-139">正しくない</span><span class="sxs-lookup"><span data-stu-id="a3a5c-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a3a5c-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="a3a5c-140">See also</span></span>

- [<span data-ttu-id="a3a5c-141">FindFolder 操作</span><span class="sxs-lookup"><span data-stu-id="a3a5c-141">FindFolder operation</span></span>](findfolder-operation.md)  
- [<span data-ttu-id="a3a5c-142">FindItem 操作</span><span class="sxs-lookup"><span data-stu-id="a3a5c-142">FindItem operation</span></span>](finditem-operation.md) 
- [<span data-ttu-id="a3a5c-143">ResolveNames 操作</span><span class="sxs-lookup"><span data-stu-id="a3a5c-143">ResolveNames operation</span></span>](resolvenames-operation.md)

