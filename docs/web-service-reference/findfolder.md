---
title: FindFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindFolder
api_type:
- schema
ms.assetid: b8a59740-d978-454c-9629-a10792385ba0
description: FindFolder 要素は、メールボックス内のフォルダーを検索するための要求を定義します。
ms.openlocfilehash: d41283547c443e38e2e87379a7224df9c89f901d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760501"
---
# <a name="findfolder"></a><span data-ttu-id="195b9-103">FindFolder</span><span class="sxs-lookup"><span data-stu-id="195b9-103">FindFolder</span></span>

<span data-ttu-id="195b9-104">**FindFolder**要素は、メールボックス内のフォルダーを検索するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="195b9-104">The **FindFolder** element defines a request to find folders in a mailbox.</span></span> 
  
```xml
<FindFolder Traversal="Shallow/Deep/SoftDeleted">
   <FolderShape/>
   <IndexedPageFolderView/>
   <Restriction/>
   <ParentFolderIds/>
</FindFolder>
```

 <span data-ttu-id="195b9-105">**FindFolderType**</span><span class="sxs-lookup"><span data-stu-id="195b9-105">**FindFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="195b9-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="195b9-106">Attributes and elements</span></span>

<span data-ttu-id="195b9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="195b9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="195b9-108">属性</span><span class="sxs-lookup"><span data-stu-id="195b9-108">Attributes</span></span>

|<span data-ttu-id="195b9-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="195b9-109">**Attribute**</span></span>|<span data-ttu-id="195b9-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="195b9-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="195b9-111">トラバーサル</span><span class="sxs-lookup"><span data-stu-id="195b9-111">Traversal</span></span>  <br/> |<span data-ttu-id="195b9-112">検索を実行する方法を定義します。</span><span class="sxs-lookup"><span data-stu-id="195b9-112">Defines how a search is performed.</span></span> <span data-ttu-id="195b9-113">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="195b9-113">This attribute is required.</span></span>  <br/> |
   
#### <a name="traversal-attribute-values"></a><span data-ttu-id="195b9-114">検査の属性値</span><span class="sxs-lookup"><span data-stu-id="195b9-114">Traversal attribute values</span></span>

|<span data-ttu-id="195b9-115">**値**</span><span class="sxs-lookup"><span data-stu-id="195b9-115">**Value**</span></span>|<span data-ttu-id="195b9-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="195b9-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="195b9-117">浅い</span><span class="sxs-lookup"><span data-stu-id="195b9-117">Shallow</span></span>  <br/> |<span data-ttu-id="195b9-118">識別されたフォルダーのみを検索し、削除されていないアイテムのフォルダー Id のみを取得するために、FindFolder 操作を指示します。</span><span class="sxs-lookup"><span data-stu-id="195b9-118">Instructs the FindFolder operation to search only the identified folder and to return only the folder IDs for items that have not been deleted.</span></span> <span data-ttu-id="195b9-119">これは簡易走査と呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="195b9-119">This is called a shallow traversal.</span></span>  <br/> |
|<span data-ttu-id="195b9-120">深い</span><span class="sxs-lookup"><span data-stu-id="195b9-120">Deep</span></span>  <br/> |<span data-ttu-id="195b9-121">識別された親フォルダーのすべての子フォルダーで検索して、削除されていないアイテムのフォルダー Id だけを返すには、FindFolder 操作を指示します。</span><span class="sxs-lookup"><span data-stu-id="195b9-121">Instructs the FindFolder operation to search in all child folders of the identified parent folder and to return only the folder IDs for items that have not been deleted.</span></span> <span data-ttu-id="195b9-122">これは、詳細走査と呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="195b9-122">This is called a deep traversal.</span></span>  <br/> |
|<span data-ttu-id="195b9-123">削除済み (回復可能)</span><span class="sxs-lookup"><span data-stu-id="195b9-123">SoftDeleted</span></span>  <br/> |<span data-ttu-id="195b9-124">FindFolder 操作削除済みアイテムの簡易走査の検索を実行するように指示します。</span><span class="sxs-lookup"><span data-stu-id="195b9-124">Instructs the FindFolder operation to perform a shallow traversal search for deleted items.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="195b9-125">子要素</span><span class="sxs-lookup"><span data-stu-id="195b9-125">Child elements</span></span>

|<span data-ttu-id="195b9-126">**要素**</span><span class="sxs-lookup"><span data-stu-id="195b9-126">**Element**</span></span>|<span data-ttu-id="195b9-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="195b9-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="195b9-128">FolderShape</span><span class="sxs-lookup"><span data-stu-id="195b9-128">FolderShape</span></span>](foldershape.md) <br/> |<span data-ttu-id="195b9-129">FindFolder の応答に含めるフォルダーのプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="195b9-129">Identifies the folder properties to include in a FindFolder response.</span></span>  <br/> |
|[<span data-ttu-id="195b9-130">IndexedPageFolderView</span><span class="sxs-lookup"><span data-stu-id="195b9-130">IndexedPageFolderView</span></span>](indexedpagefolderview.md) <br/> |<span data-ttu-id="195b9-131">どのページの項目の情報について説明します FindFolder 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="195b9-131">Describes how paged item information is returned in a FindFolder response.</span></span> <span data-ttu-id="195b9-132">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="195b9-132">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="195b9-133">FractionalPageFolderView</span><span class="sxs-lookup"><span data-stu-id="195b9-133">FractionalPageFolderView</span></span>](fractionalpagefolderview.md) <br/> |<span data-ttu-id="195b9-134">ページ ビューが起動し、フォルダーの最大数は、FindFolder 要求で返されるについて説明します。</span><span class="sxs-lookup"><span data-stu-id="195b9-134">Describes where the paged view starts and the maximum number of folders returned in a FindFolder request.</span></span> <span data-ttu-id="195b9-135">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="195b9-135">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="195b9-136">Restriction</span><span class="sxs-lookup"><span data-stu-id="195b9-136">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="195b9-137">FindFolder 操作でフォルダーをフィルター処理するために使用されるクエリの制限を定義します。</span><span class="sxs-lookup"><span data-stu-id="195b9-137">Defines a restriction or query that is used to filter folders in a FindFolder operation.</span></span> <span data-ttu-id="195b9-138">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="195b9-138">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="195b9-139">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="195b9-139">ParentFolderIds</span></span>](parentfolderids.md) <br/> |<span data-ttu-id="195b9-140">FindFolder 操作が検索するフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="195b9-140">Identifies folders for the FindFolder operation to search.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="195b9-141">親要素</span><span class="sxs-lookup"><span data-stu-id="195b9-141">Parent elements</span></span>

<span data-ttu-id="195b9-142">なし。</span><span class="sxs-lookup"><span data-stu-id="195b9-142">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="195b9-143">備考</span><span class="sxs-lookup"><span data-stu-id="195b9-143">Remarks</span></span>

<span data-ttu-id="195b9-144">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="195b9-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="195b9-145">例</span><span class="sxs-lookup"><span data-stu-id="195b9-145">Example</span></span>

<span data-ttu-id="195b9-146">FindFolder 要求の次の例では、受信トレイ内にあるすべてのフォルダーを検索する要求を作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="195b9-146">The following example of a FindFolder request shows how to form a request to find all the folders located in an Inbox.</span></span>
  
```
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

## <a name="element-information"></a><span data-ttu-id="195b9-147">要素情報</span><span class="sxs-lookup"><span data-stu-id="195b9-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="195b9-148">名前空間</span><span class="sxs-lookup"><span data-stu-id="195b9-148">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="195b9-149">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="195b9-149">Schema Name</span></span>  <br/> |<span data-ttu-id="195b9-150">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="195b9-150">Messages schema</span></span>  <br/> |
|<span data-ttu-id="195b9-151">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="195b9-151">Validation File</span></span>  <br/> |<span data-ttu-id="195b9-152">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="195b9-152">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="195b9-153">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="195b9-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="195b9-154">False</span><span class="sxs-lookup"><span data-stu-id="195b9-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="195b9-155">関連項目</span><span class="sxs-lookup"><span data-stu-id="195b9-155">See also</span></span>



<span data-ttu-id="195b9-156">
  [FindFolder 操作](findfolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="195b9-156">[FindFolder operation](findfolder-operation.md)</span></span>

