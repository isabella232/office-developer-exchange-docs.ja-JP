---
title: BaseShape
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BaseShape
api_type:
- schema
ms.assetid: 42c04f3b-abaa-4197-a3d6-d21677ffb1c0
description: BaseShape の要素は、アイテムまたはフォルダーの応答で返されるプロパティのセットを識別します。
ms.openlocfilehash: 69b27d23fd75d4c1a274f31dfa419b759dbb2bbe
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759497"
---
# <a name="baseshape"></a><span data-ttu-id="6d2cb-103">BaseShape</span><span class="sxs-lookup"><span data-stu-id="6d2cb-103">BaseShape</span></span>

<span data-ttu-id="6d2cb-104">**BaseShape**の要素は、アイテムまたはフォルダーの応答で返されるプロパティのセットを識別します。</span><span class="sxs-lookup"><span data-stu-id="6d2cb-104">The **BaseShape** element identifies the set of properties to return in an item or folder response.</span></span> 
  
```xml
<BaseShape>IdOnly or Default or AllProperties</BaseShape>
```

 <span data-ttu-id="6d2cb-105">**DefaultShapeNamesType**</span><span class="sxs-lookup"><span data-stu-id="6d2cb-105">**DefaultShapeNamesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6d2cb-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6d2cb-106">Attributes and elements</span></span>

<span data-ttu-id="6d2cb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6d2cb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6d2cb-108">属性</span><span class="sxs-lookup"><span data-stu-id="6d2cb-108">Attributes</span></span>

<span data-ttu-id="6d2cb-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6d2cb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6d2cb-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6d2cb-110">Child elements</span></span>

<span data-ttu-id="6d2cb-111">なし</span><span class="sxs-lookup"><span data-stu-id="6d2cb-111">None</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6d2cb-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6d2cb-112">Parent elements</span></span>

|<span data-ttu-id="6d2cb-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="6d2cb-113">**Element**</span></span>|<span data-ttu-id="6d2cb-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="6d2cb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6d2cb-115">FolderShape</span><span class="sxs-lookup"><span data-stu-id="6d2cb-115">FolderShape</span></span>](foldershape.md) <br/> | <span data-ttu-id="6d2cb-116">GetFolder、FindFolder、または SyncFolderHierarchy の応答に含めるフォルダーのプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="6d2cb-116">Identifies the folder properties to include in the GetFolder, FindFolder, or SyncFolderHierarchy response.</span></span><br/><br/><span data-ttu-id="6d2cb-117">この要素への XPath 式は、次のように。</span><span class="sxs-lookup"><span data-stu-id="6d2cb-117">The following are the XPath expressions to this element:</span></span><br/><br/>`/GetFolder/FolderShape` <br/>  `/FindFolder/FolderShape` <br/>  `/SyncFolderHierarchy/FolderShape` <br/> |
|[<span data-ttu-id="6d2cb-118">ItemShape</span><span class="sxs-lookup"><span data-stu-id="6d2cb-118">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="6d2cb-119">GetItem、FindItem、または SyncFolderItems の応答に含めるコンテンツ アイテムのプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="6d2cb-119">Identifies the item properties and content to include in a GetItem, FindItem, or SyncFolderItems response.</span></span><br/><br/><span data-ttu-id="6d2cb-120">この要素への XPath 式は、次のように。</span><span class="sxs-lookup"><span data-stu-id="6d2cb-120">The following are the XPath expressions to this element:</span></span><br/><br/>`/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6d2cb-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6d2cb-121">Text value</span></span>

<span data-ttu-id="6d2cb-122">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="6d2cb-122">A text value is required.</span></span> <span data-ttu-id="6d2cb-123">次の表は、可能なテキスト値を示します。</span><span class="sxs-lookup"><span data-stu-id="6d2cb-123">The following table lists the possible text values.</span></span>
  
<span data-ttu-id="6d2cb-124">**BaseShape 要素のテキスト値**</span><span class="sxs-lookup"><span data-stu-id="6d2cb-124">**Text values for the BaseShape element**</span></span>

|<span data-ttu-id="6d2cb-125">**値**</span><span class="sxs-lookup"><span data-stu-id="6d2cb-125">**Value**</span></span>|<span data-ttu-id="6d2cb-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="6d2cb-126">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6d2cb-127">IdOnly</span><span class="sxs-lookup"><span data-stu-id="6d2cb-127">IdOnly</span></span>  <br/> |<span data-ttu-id="6d2cb-128">アイテムまたはフォルダーの ID を返します。</span><span class="sxs-lookup"><span data-stu-id="6d2cb-128">Returns only the item or folder ID.</span></span>  <br/> |
|<span data-ttu-id="6d2cb-129">Default</span><span class="sxs-lookup"><span data-stu-id="6d2cb-129">Default</span></span>  <br/> |<span data-ttu-id="6d2cb-130">アイテムまたはフォルダーの既定値として定義されているプロパティのセットを返します。</span><span class="sxs-lookup"><span data-stu-id="6d2cb-130">Returns a set of properties that are defined as the default for the item or folder.</span></span>  <br/> |
|<span data-ttu-id="6d2cb-131">AllProperties</span><span class="sxs-lookup"><span data-stu-id="6d2cb-131">AllProperties</span></span>  <br/> |<span data-ttu-id="6d2cb-132">フォルダーを作成するのには、Exchange ビジネス ロジック層で使用されるすべてのプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="6d2cb-132">Returns all the properties used by the Exchange Business Logic layer to construct a folder.</span></span>  <br/> |
   
<span data-ttu-id="6d2cb-133">FindFolder 要求に対して返される既定のプロパティを次の表に一覧します。</span><span class="sxs-lookup"><span data-stu-id="6d2cb-133">The following table lists the default properties that are returned for a FindFolder request.</span></span> <span data-ttu-id="6d2cb-134">名前の順序で指定されたフォルダーのすべてのサブフォルダーが返されます。</span><span class="sxs-lookup"><span data-stu-id="6d2cb-134">All subfolders of a given folder are returned in order by name.</span></span>
  
<span data-ttu-id="6d2cb-135">**既定のプロパティ**</span><span class="sxs-lookup"><span data-stu-id="6d2cb-135">**Default properties**</span></span>

|<span data-ttu-id="6d2cb-136">**Folder**</span><span class="sxs-lookup"><span data-stu-id="6d2cb-136">**Folder**</span></span>|<span data-ttu-id="6d2cb-137">**既定のプロパティ**</span><span class="sxs-lookup"><span data-stu-id="6d2cb-137">**Default Properties**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6d2cb-138">受信トレイ</span><span class="sxs-lookup"><span data-stu-id="6d2cb-138">Inbox</span></span>  <br/> |<span data-ttu-id="6d2cb-139">フォルダー Id、表示名、未読数、合計数、サブフォルダーの数</span><span class="sxs-lookup"><span data-stu-id="6d2cb-139">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="6d2cb-140">連絡先</span><span class="sxs-lookup"><span data-stu-id="6d2cb-140">Contacts</span></span>  <br/> |<span data-ttu-id="6d2cb-141">フォルダー Id、表示名、合計数、サブフォルダーの数</span><span class="sxs-lookup"><span data-stu-id="6d2cb-141">FolderId, display name, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="6d2cb-142">カレンダー</span><span class="sxs-lookup"><span data-stu-id="6d2cb-142">Calendar</span></span>  <br/> |<span data-ttu-id="6d2cb-143">フォルダー Id、表示名、サブフォルダーの数</span><span class="sxs-lookup"><span data-stu-id="6d2cb-143">FolderId, display name, subfolder count</span></span>  <br/> |
|<span data-ttu-id="6d2cb-144">������</span><span class="sxs-lookup"><span data-stu-id="6d2cb-144">Drafts</span></span>  <br/> |<span data-ttu-id="6d2cb-145">フォルダー Id、表示名、未読数、合計数、サブフォルダーの数</span><span class="sxs-lookup"><span data-stu-id="6d2cb-145">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="6d2cb-146">削除済みアイテム</span><span class="sxs-lookup"><span data-stu-id="6d2cb-146">Deleted items</span></span>  <br/> |<span data-ttu-id="6d2cb-147">フォルダー Id、表示名、未読数、合計数、サブフォルダーの数</span><span class="sxs-lookup"><span data-stu-id="6d2cb-147">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="6d2cb-148">その他のフォルダー</span><span class="sxs-lookup"><span data-stu-id="6d2cb-148">Other folders</span></span>  <br/> |<span data-ttu-id="6d2cb-149">フォルダー Id、表示名、未読数、合計数、サブフォルダーの数</span><span class="sxs-lookup"><span data-stu-id="6d2cb-149">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="6d2cb-150">送信トレイ</span><span class="sxs-lookup"><span data-stu-id="6d2cb-150">Outbox</span></span>  <br/> |<span data-ttu-id="6d2cb-151">フォルダー Id、表示名、未読数、合計数、サブフォルダーの数</span><span class="sxs-lookup"><span data-stu-id="6d2cb-151">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="6d2cb-152">タスク</span><span class="sxs-lookup"><span data-stu-id="6d2cb-152">Tasks</span></span>  <br/> |<span data-ttu-id="6d2cb-153">フォルダー Id、表示名、期限経過のカウント、合計、サブフォルダーの数</span><span class="sxs-lookup"><span data-stu-id="6d2cb-153">FolderId, display name, past due count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="6d2cb-154">���l</span><span class="sxs-lookup"><span data-stu-id="6d2cb-154">Notes</span></span>  <br/> |<span data-ttu-id="6d2cb-155">フォルダー Id、表示名、合計数、サブフォルダーの数</span><span class="sxs-lookup"><span data-stu-id="6d2cb-155">FolderId, display name, total count, subfolder count</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6d2cb-156">備考</span><span class="sxs-lookup"><span data-stu-id="6d2cb-156">Remarks</span></span>

<span data-ttu-id="6d2cb-157">[BaseShape](baseshape.md)の要素で指定されたもの以外のプロパティを取得するには、 [AdditionalProperties](additionalproperties.md)要素を使用します。</span><span class="sxs-lookup"><span data-stu-id="6d2cb-157">To return properties in addition to those identified by the [BaseShape](baseshape.md) element, use the [AdditionalProperties](additionalproperties.md) element.</span></span> 
  
## <a name="example"></a><span data-ttu-id="6d2cb-158">例</span><span class="sxs-lookup"><span data-stu-id="6d2cb-158">Example</span></span>

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

## <a name="element-information"></a><span data-ttu-id="6d2cb-159">要素情報</span><span class="sxs-lookup"><span data-stu-id="6d2cb-159">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6d2cb-160">名前空間</span><span class="sxs-lookup"><span data-stu-id="6d2cb-160">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6d2cb-161">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6d2cb-161">Schema Name</span></span>  <br/> |<span data-ttu-id="6d2cb-162">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="6d2cb-162">Types schema</span></span>  <br/> |
|<span data-ttu-id="6d2cb-163">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6d2cb-163">Validation File</span></span>  <br/> |<span data-ttu-id="6d2cb-164">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6d2cb-164">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6d2cb-165">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6d2cb-165">Can be Empty</span></span>  <br/> |<span data-ttu-id="6d2cb-166">False</span><span class="sxs-lookup"><span data-stu-id="6d2cb-166">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6d2cb-167">関連項目</span><span class="sxs-lookup"><span data-stu-id="6d2cb-167">See also</span></span>

- [<span data-ttu-id="6d2cb-168">FolderShape</span><span class="sxs-lookup"><span data-stu-id="6d2cb-168">FolderShape</span></span>](foldershape.md)
- [<span data-ttu-id="6d2cb-169">ItemShape</span><span class="sxs-lookup"><span data-stu-id="6d2cb-169">ItemShape</span></span>](itemshape.md)

