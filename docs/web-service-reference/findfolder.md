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
description: FindFolder 要素は、メールボックス内のフォルダーを検索する要求を定義します。
ms.openlocfilehash: 248047206a661afe723543e52c51b57847148423
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462578"
---
# <a name="findfolder"></a><span data-ttu-id="6881d-103">FindFolder</span><span class="sxs-lookup"><span data-stu-id="6881d-103">FindFolder</span></span>

<span data-ttu-id="6881d-104">**Findfolder**要素は、メールボックス内のフォルダーを検索する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="6881d-104">The **FindFolder** element defines a request to find folders in a mailbox.</span></span> 
  
```xml
<FindFolder Traversal="Shallow/Deep/SoftDeleted">
   <FolderShape/>
   <IndexedPageFolderView/>
   <Restriction/>
   <ParentFolderIds/>
</FindFolder>
```

```xml
<FindFolder Traversal="Shallow/Deep/SoftDeleted">
   <FolderShape/>
   <FractionalPageFolderView/>
   <Restriction/>
   <ParentFolderIds/>
</FindFolder>
```

<span data-ttu-id="6881d-105">**FindFolderType**</span><span class="sxs-lookup"><span data-stu-id="6881d-105">**FindFolderType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="6881d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6881d-106">Attributes and elements</span></span>

<span data-ttu-id="6881d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6881d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6881d-108">属性</span><span class="sxs-lookup"><span data-stu-id="6881d-108">Attributes</span></span>

|<span data-ttu-id="6881d-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="6881d-109">**Attribute**</span></span>|<span data-ttu-id="6881d-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="6881d-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6881d-111">走査</span><span class="sxs-lookup"><span data-stu-id="6881d-111">Traversal</span></span>  <br/> |<span data-ttu-id="6881d-112">検索の実行方法を定義します。</span><span class="sxs-lookup"><span data-stu-id="6881d-112">Defines how a search is performed.</span></span> <span data-ttu-id="6881d-113">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="6881d-113">This attribute is required.</span></span>  <br/> |
   
#### <a name="traversal-attribute-values"></a><span data-ttu-id="6881d-114">トラバース属性値</span><span class="sxs-lookup"><span data-stu-id="6881d-114">Traversal attribute values</span></span>

|<span data-ttu-id="6881d-115">**値**</span><span class="sxs-lookup"><span data-stu-id="6881d-115">**Value**</span></span>|<span data-ttu-id="6881d-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="6881d-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6881d-117">浅い</span><span class="sxs-lookup"><span data-stu-id="6881d-117">Shallow</span></span>  <br/> |<span data-ttu-id="6881d-118">FindFolder 操作に対して、識別されたフォルダーのみを検索し、削除されていないアイテムのフォルダー Id のみを返すように指示します。</span><span class="sxs-lookup"><span data-stu-id="6881d-118">Instructs the FindFolder operation to search only the identified folder and to return only the folder IDs for items that have not been deleted.</span></span> <span data-ttu-id="6881d-119">これは、浅い走査と呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="6881d-119">This is called a shallow traversal.</span></span>  <br/> |
|<span data-ttu-id="6881d-120">深い</span><span class="sxs-lookup"><span data-stu-id="6881d-120">Deep</span></span>  <br/> |<span data-ttu-id="6881d-121">FindFolder 操作に対して、識別された親フォルダーのすべての子フォルダーを検索し、削除されていないアイテムのフォルダー Id のみを返すように指示します。</span><span class="sxs-lookup"><span data-stu-id="6881d-121">Instructs the FindFolder operation to search in all child folders of the identified parent folder and to return only the folder IDs for items that have not been deleted.</span></span> <span data-ttu-id="6881d-122">これは deep トラバースと呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="6881d-122">This is called a deep traversal.</span></span>  <br/> |
|<span data-ttu-id="6881d-123">削除済み (回復可能)</span><span class="sxs-lookup"><span data-stu-id="6881d-123">SoftDeleted</span></span>  <br/> |<span data-ttu-id="6881d-124">FindFolder 操作に対して、削除されたアイテムに対して緩斜面検索を実行するように指示します。</span><span class="sxs-lookup"><span data-stu-id="6881d-124">Instructs the FindFolder operation to perform a shallow traversal search for deleted items.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6881d-125">子要素</span><span class="sxs-lookup"><span data-stu-id="6881d-125">Child elements</span></span>

|<span data-ttu-id="6881d-126">**Element**</span><span class="sxs-lookup"><span data-stu-id="6881d-126">**Element**</span></span>|<span data-ttu-id="6881d-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="6881d-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6881d-128">FolderShape</span><span class="sxs-lookup"><span data-stu-id="6881d-128">FolderShape</span></span>](foldershape.md) <br/> |<span data-ttu-id="6881d-129">FindFolder 応答に含めるフォルダーのプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="6881d-129">Identifies the folder properties to include in a FindFolder response.</span></span>  <br/> |
|[<span data-ttu-id="6881d-130">IndexedPageFolderView</span><span class="sxs-lookup"><span data-stu-id="6881d-130">IndexedPageFolderView</span></span>](indexedpagefolderview.md) <br/> |<span data-ttu-id="6881d-131">ページアイテムの情報が FindFolder 応答で返される方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="6881d-131">Describes how paged item information is returned in a FindFolder response.</span></span> <span data-ttu-id="6881d-132">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="6881d-132">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="6881d-133">FractionalPageFolderView</span><span class="sxs-lookup"><span data-stu-id="6881d-133">FractionalPageFolderView</span></span>](fractionalpagefolderview.md) <br/> |<span data-ttu-id="6881d-134">ページビューの開始位置と、FindFolder 要求で返されるフォルダーの最大数を指定します。</span><span class="sxs-lookup"><span data-stu-id="6881d-134">Describes where the paged view starts and the maximum number of folders returned in a FindFolder request.</span></span> <span data-ttu-id="6881d-135">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="6881d-135">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="6881d-136">Restriction</span><span class="sxs-lookup"><span data-stu-id="6881d-136">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="6881d-137">FindFolder 操作でフォルダーにフィルターを適用するために使用される制限またはクエリを定義します。</span><span class="sxs-lookup"><span data-stu-id="6881d-137">Defines a restriction or query that is used to filter folders in a FindFolder operation.</span></span> <span data-ttu-id="6881d-138">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="6881d-138">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="6881d-139">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="6881d-139">ParentFolderIds</span></span>](parentfolderids.md) <br/> |<span data-ttu-id="6881d-140">検索する FindFolder 操作のフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="6881d-140">Identifies folders for the FindFolder operation to search.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6881d-141">親要素</span><span class="sxs-lookup"><span data-stu-id="6881d-141">Parent elements</span></span>

<span data-ttu-id="6881d-142">なし。</span><span class="sxs-lookup"><span data-stu-id="6881d-142">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6881d-143">注釈</span><span class="sxs-lookup"><span data-stu-id="6881d-143">Remarks</span></span>

<span data-ttu-id="6881d-144">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="6881d-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="6881d-145">例</span><span class="sxs-lookup"><span data-stu-id="6881d-145">Example</span></span>

<span data-ttu-id="6881d-146">FindFolder 要求の次の例は、受信トレイ内のすべてのフォルダーを検索するための要求を形成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="6881d-146">The following example of a FindFolder request shows how to form a request to find all the folders located in an Inbox.</span></span>
  
```xml
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

## <a name="element-information"></a><span data-ttu-id="6881d-147">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6881d-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6881d-148">Namespace</span><span class="sxs-lookup"><span data-stu-id="6881d-148">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6881d-149">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6881d-149">Schema Name</span></span>  <br/> |<span data-ttu-id="6881d-150">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="6881d-150">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6881d-151">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6881d-151">Validation File</span></span>  <br/> |<span data-ttu-id="6881d-152">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="6881d-152">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6881d-153">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6881d-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="6881d-154">正しくない</span><span class="sxs-lookup"><span data-stu-id="6881d-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6881d-155">関連項目</span><span class="sxs-lookup"><span data-stu-id="6881d-155">See also</span></span>

- <span data-ttu-id="6881d-156">
  [FindFolder 操作](findfolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="6881d-156">[FindFolder operation](findfolder-operation.md)</span></span>

