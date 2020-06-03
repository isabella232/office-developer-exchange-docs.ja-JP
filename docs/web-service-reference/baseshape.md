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
description: BaseShape 要素は、アイテムまたはフォルダーの応答で返されるプロパティのセットを識別します。
ms.openlocfilehash: 9b3f00ff94fbfe6ad6373b16ad95eb9136f81c64
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464491"
---
# <a name="baseshape"></a><span data-ttu-id="3cde0-103">BaseShape</span><span class="sxs-lookup"><span data-stu-id="3cde0-103">BaseShape</span></span>

<span data-ttu-id="3cde0-104">**Baseshape**要素は、アイテムまたはフォルダーの応答で返されるプロパティのセットを識別します。</span><span class="sxs-lookup"><span data-stu-id="3cde0-104">The **BaseShape** element identifies the set of properties to return in an item or folder response.</span></span> 
  
```xml
<BaseShape>IdOnly or Default or AllProperties</BaseShape>
```

 <span data-ttu-id="3cde0-105">**DefaultShapeNamesType**</span><span class="sxs-lookup"><span data-stu-id="3cde0-105">**DefaultShapeNamesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3cde0-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="3cde0-106">Attributes and elements</span></span>

<span data-ttu-id="3cde0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3cde0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3cde0-108">属性</span><span class="sxs-lookup"><span data-stu-id="3cde0-108">Attributes</span></span>

<span data-ttu-id="3cde0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3cde0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3cde0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3cde0-110">Child elements</span></span>

<span data-ttu-id="3cde0-111">なし</span><span class="sxs-lookup"><span data-stu-id="3cde0-111">None</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3cde0-112">親要素</span><span class="sxs-lookup"><span data-stu-id="3cde0-112">Parent elements</span></span>

|<span data-ttu-id="3cde0-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="3cde0-113">**Element**</span></span>|<span data-ttu-id="3cde0-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="3cde0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3cde0-115">FolderShape</span><span class="sxs-lookup"><span data-stu-id="3cde0-115">FolderShape</span></span>](foldershape.md) <br/> | <span data-ttu-id="3cde0-116">GetFolder、FindFolder、または SyncFolderHierarchy の応答に含めるフォルダーのプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="3cde0-116">Identifies the folder properties to include in the GetFolder, FindFolder, or SyncFolderHierarchy response.</span></span><br/><br/><span data-ttu-id="3cde0-117">この要素の XPath 式は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="3cde0-117">The following are the XPath expressions to this element:</span></span><br/><br/>`/GetFolder/FolderShape` <br/>  `/FindFolder/FolderShape` <br/>  `/SyncFolderHierarchy/FolderShape` <br/> |
|[<span data-ttu-id="3cde0-118">ItemShape</span><span class="sxs-lookup"><span data-stu-id="3cde0-118">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="3cde0-119">GetItem、FindItem、または SyncFolderItems 応答に含めるアイテムのプロパティとコンテンツを指定します。</span><span class="sxs-lookup"><span data-stu-id="3cde0-119">Identifies the item properties and content to include in a GetItem, FindItem, or SyncFolderItems response.</span></span><br/><br/><span data-ttu-id="3cde0-120">この要素の XPath 式は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="3cde0-120">The following are the XPath expressions to this element:</span></span><br/><br/>`/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3cde0-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3cde0-121">Text value</span></span>

<span data-ttu-id="3cde0-122">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="3cde0-122">A text value is required.</span></span> <span data-ttu-id="3cde0-123">次の表に、使用可能なテキスト値を示します。</span><span class="sxs-lookup"><span data-stu-id="3cde0-123">The following table lists the possible text values.</span></span>
  
<span data-ttu-id="3cde0-124">**BaseShape 要素のテキスト値**</span><span class="sxs-lookup"><span data-stu-id="3cde0-124">**Text values for the BaseShape element**</span></span>

|<span data-ttu-id="3cde0-125">**値**</span><span class="sxs-lookup"><span data-stu-id="3cde0-125">**Value**</span></span>|<span data-ttu-id="3cde0-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="3cde0-126">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3cde0-127">IdOnly</span><span class="sxs-lookup"><span data-stu-id="3cde0-127">IdOnly</span></span>  <br/> |<span data-ttu-id="3cde0-128">アイテムまたはフォルダーの ID のみを返します。</span><span class="sxs-lookup"><span data-stu-id="3cde0-128">Returns only the item or folder ID.</span></span>  <br/> |
|<span data-ttu-id="3cde0-129">既定値</span><span class="sxs-lookup"><span data-stu-id="3cde0-129">Default</span></span>  <br/> |<span data-ttu-id="3cde0-130">アイテムまたはフォルダーの既定値として定義されているプロパティのセットを返します。</span><span class="sxs-lookup"><span data-stu-id="3cde0-130">Returns a set of properties that are defined as the default for the item or folder.</span></span>  <br/> |
|<span data-ttu-id="3cde0-131">AllProperties</span><span class="sxs-lookup"><span data-stu-id="3cde0-131">AllProperties</span></span>  <br/> |<span data-ttu-id="3cde0-132">フォルダーを作成するために Exchange ビジネスロジック層で使用されるすべてのプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="3cde0-132">Returns all the properties used by the Exchange Business Logic layer to construct a folder.</span></span>  <br/> |
   
<span data-ttu-id="3cde0-133">次の表に、FindFolder 要求に対して返される既定のプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3cde0-133">The following table lists the default properties that are returned for a FindFolder request.</span></span> <span data-ttu-id="3cde0-134">指定したフォルダーのすべてのサブフォルダーが名前で順に返されます。</span><span class="sxs-lookup"><span data-stu-id="3cde0-134">All subfolders of a given folder are returned in order by name.</span></span>
  
<span data-ttu-id="3cde0-135">**既定のプロパティ**</span><span class="sxs-lookup"><span data-stu-id="3cde0-135">**Default properties**</span></span>

|<span data-ttu-id="3cde0-136">**Folder**</span><span class="sxs-lookup"><span data-stu-id="3cde0-136">**Folder**</span></span>|<span data-ttu-id="3cde0-137">**既定のプロパティ**</span><span class="sxs-lookup"><span data-stu-id="3cde0-137">**Default Properties**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3cde0-138">受信トレイ</span><span class="sxs-lookup"><span data-stu-id="3cde0-138">Inbox</span></span>  <br/> |<span data-ttu-id="3cde0-139">FolderId、表示名、未読数、合計数、サブフォルダー数</span><span class="sxs-lookup"><span data-stu-id="3cde0-139">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="3cde0-140">連絡先</span><span class="sxs-lookup"><span data-stu-id="3cde0-140">Contacts</span></span>  <br/> |<span data-ttu-id="3cde0-141">FolderId、表示名、合計数、サブフォルダー数</span><span class="sxs-lookup"><span data-stu-id="3cde0-141">FolderId, display name, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="3cde0-142">カレンダー</span><span class="sxs-lookup"><span data-stu-id="3cde0-142">Calendar</span></span>  <br/> |<span data-ttu-id="3cde0-143">FolderId、表示名、サブフォルダー数</span><span class="sxs-lookup"><span data-stu-id="3cde0-143">FolderId, display name, subfolder count</span></span>  <br/> |
|<span data-ttu-id="3cde0-144">下書き</span><span class="sxs-lookup"><span data-stu-id="3cde0-144">Drafts</span></span>  <br/> |<span data-ttu-id="3cde0-145">FolderId、表示名、未読数、合計数、サブフォルダー数</span><span class="sxs-lookup"><span data-stu-id="3cde0-145">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="3cde0-146">削除済みアイテム</span><span class="sxs-lookup"><span data-stu-id="3cde0-146">Deleted items</span></span>  <br/> |<span data-ttu-id="3cde0-147">FolderId、表示名、未読数、合計数、サブフォルダー数</span><span class="sxs-lookup"><span data-stu-id="3cde0-147">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="3cde0-148">その他のフォルダー</span><span class="sxs-lookup"><span data-stu-id="3cde0-148">Other folders</span></span>  <br/> |<span data-ttu-id="3cde0-149">FolderId、表示名、未読数、合計数、サブフォルダー数</span><span class="sxs-lookup"><span data-stu-id="3cde0-149">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="3cde0-150">送信トレイ</span><span class="sxs-lookup"><span data-stu-id="3cde0-150">Outbox</span></span>  <br/> |<span data-ttu-id="3cde0-151">FolderId、表示名、未読数、合計数、サブフォルダー数</span><span class="sxs-lookup"><span data-stu-id="3cde0-151">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="3cde0-152">タスク</span><span class="sxs-lookup"><span data-stu-id="3cde0-152">Tasks</span></span>  <br/> |<span data-ttu-id="3cde0-153">FolderId、表示名、過去の期限数、合計数、サブフォルダー数</span><span class="sxs-lookup"><span data-stu-id="3cde0-153">FolderId, display name, past due count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="3cde0-154">メモ</span><span class="sxs-lookup"><span data-stu-id="3cde0-154">Notes</span></span>  <br/> |<span data-ttu-id="3cde0-155">FolderId、表示名、合計数、サブフォルダー数</span><span class="sxs-lookup"><span data-stu-id="3cde0-155">FolderId, display name, total count, subfolder count</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3cde0-156">注釈</span><span class="sxs-lookup"><span data-stu-id="3cde0-156">Remarks</span></span>

<span data-ttu-id="3cde0-157">[Baseshape](baseshape.md)要素によって識別されるプロパティに加えて、プロパティを返すには、 [additionalproperties](additionalproperties.md)要素を使用します。</span><span class="sxs-lookup"><span data-stu-id="3cde0-157">To return properties in addition to those identified by the [BaseShape](baseshape.md) element, use the [AdditionalProperties](additionalproperties.md) element.</span></span> 
  
## <a name="example"></a><span data-ttu-id="3cde0-158">例</span><span class="sxs-lookup"><span data-stu-id="3cde0-158">Example</span></span>

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

## <a name="element-information"></a><span data-ttu-id="3cde0-159">要素の情報</span><span class="sxs-lookup"><span data-stu-id="3cde0-159">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3cde0-160">Namespace</span><span class="sxs-lookup"><span data-stu-id="3cde0-160">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3cde0-161">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3cde0-161">Schema Name</span></span>  <br/> |<span data-ttu-id="3cde0-162">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="3cde0-162">Types schema</span></span>  <br/> |
|<span data-ttu-id="3cde0-163">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3cde0-163">Validation File</span></span>  <br/> |<span data-ttu-id="3cde0-164">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="3cde0-164">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3cde0-165">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3cde0-165">Can be Empty</span></span>  <br/> |<span data-ttu-id="3cde0-166">正しくない</span><span class="sxs-lookup"><span data-stu-id="3cde0-166">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3cde0-167">関連項目</span><span class="sxs-lookup"><span data-stu-id="3cde0-167">See also</span></span>

- [<span data-ttu-id="3cde0-168">FolderShape</span><span class="sxs-lookup"><span data-stu-id="3cde0-168">FolderShape</span></span>](foldershape.md)
- [<span data-ttu-id="3cde0-169">ItemShape</span><span class="sxs-lookup"><span data-stu-id="3cde0-169">ItemShape</span></span>](itemshape.md)

