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
description: ParentFolderIds 要素は、検索 FindItem と FindFolder 操作用のフォルダーを識別します。
ms.openlocfilehash: 7c4dcc98d1cabc8e97f2846880c73111dd307dfb
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354170"
---
# <a name="parentfolderids"></a><span data-ttu-id="d5536-103">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="d5536-103">ParentFolderIds</span></span>

<span data-ttu-id="d5536-104">**ParentFolderIds**要素は、検索 FindItem と FindFolder 操作用のフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="d5536-104">The **ParentFolderIds** element identifies folders for the FindItem and FindFolder operations to search.</span></span> 
  
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

<span data-ttu-id="d5536-105">**NonEmptyArrayOfBaseFolderIdsType**</span><span class="sxs-lookup"><span data-stu-id="d5536-105">**NonEmptyArrayOfBaseFolderIdsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d5536-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d5536-106">Attributes and elements</span></span>

<span data-ttu-id="d5536-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d5536-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d5536-108">属性</span><span class="sxs-lookup"><span data-stu-id="d5536-108">Attributes</span></span>

<span data-ttu-id="d5536-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d5536-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d5536-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d5536-110">Child elements</span></span>

|<span data-ttu-id="d5536-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="d5536-111">**Element**</span></span>|<span data-ttu-id="d5536-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d5536-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d5536-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="d5536-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="d5536-114">フォルダーの識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="d5536-114">Contains the identifier and change key of a folder.</span></span> <span data-ttu-id="d5536-115">**ParentFolderIds**要素には、この要素または[DistinguishedFolderId](distinguishedfolderid.md)要素のいずれかを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d5536-115">The **ParentFolderIds** element must use either this element or the [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="d5536-116">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="d5536-116">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="d5536-117">名前で参照できる Microsoft Exchange Server 2007 のフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="d5536-117">Identifies Microsoft Exchange Server 2007 folders that can be referenced by name.</span></span> <span data-ttu-id="d5536-118">**ParentFolderIds**要素には、[フォルダー Id](folderid.md)要素またはこの要素のいずれかを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d5536-118">The **ParentFolderIds** element must use either this element or the [FolderId](folderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d5536-119">親要素</span><span class="sxs-lookup"><span data-stu-id="d5536-119">Parent elements</span></span>

|<span data-ttu-id="d5536-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="d5536-120">**Element**</span></span>|<span data-ttu-id="d5536-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="d5536-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d5536-122">FindFolder</span><span class="sxs-lookup"><span data-stu-id="d5536-122">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="d5536-123">メールボックス内のフォルダーを識別するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="d5536-123">Defines a request to identify folders in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d5536-124">FindItem</span><span class="sxs-lookup"><span data-stu-id="d5536-124">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="d5536-125">メールボックス内のアイテムを検索するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="d5536-125">Defines a request to find items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d5536-126">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="d5536-126">ResolveNames</span></span>](resolvenames.md) <br/> |<span data-ttu-id="d5536-127">あいまいな名前を解決する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="d5536-127">Defines a request to resolve ambiguous names.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d5536-128">注釈</span><span class="sxs-lookup"><span data-stu-id="d5536-128">Remarks</span></span>

<span data-ttu-id="d5536-129">**ParentFolderIds**要素には、[フォルダー Id](folderid.md)または[DistinguishedFolderId](distinguishedfolderid.md)要素のいずれかを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d5536-129">The **ParentFolderIds** element must use either the [FolderId](folderid.md) or the [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span> <span data-ttu-id="d5536-130">検索対象のフォルダーの無制限の数を定義できます。</span><span class="sxs-lookup"><span data-stu-id="d5536-130">An unlimited number of folders can be defined for the search.</span></span> 
  
## <a name="example"></a><span data-ttu-id="d5536-131">例</span><span class="sxs-lookup"><span data-stu-id="d5536-131">Example</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="element-information"></a><span data-ttu-id="d5536-132">要素情報</span><span class="sxs-lookup"><span data-stu-id="d5536-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d5536-133">名前空間</span><span class="sxs-lookup"><span data-stu-id="d5536-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d5536-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d5536-134">Schema Name</span></span>  <br/> |<span data-ttu-id="d5536-135">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="d5536-135">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d5536-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d5536-136">Validation File</span></span>  <br/> |<span data-ttu-id="d5536-137">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d5536-137">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d5536-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d5536-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="d5536-139">False</span><span class="sxs-lookup"><span data-stu-id="d5536-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d5536-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="d5536-140">See also</span></span>

- <span data-ttu-id="d5536-141">
  [FindFolder 操作](findfolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="d5536-141">[FindFolder operation](findfolder-operation.md)</span></span>  
- <span data-ttu-id="d5536-142">
  [FindItem 操作](finditem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="d5536-142">[FindItem operation](finditem-operation.md)</span></span> 
- [<span data-ttu-id="d5536-143">ResolveNames 操作</span><span class="sxs-lookup"><span data-stu-id="d5536-143">ResolveNames operation</span></span>](resolvenames-operation.md)

