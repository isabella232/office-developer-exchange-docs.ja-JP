---
title: ItemShape
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemShape
api_type:
- schema
ms.assetid: c5604161-bbc0-40bc-ad75-ff7e837d745f
description: ItemShape 要素は、GetItem 操作、FindItem 操作、または SyncFolderItems 操作の応答で返される一連のプロパティを識別します。
ms.openlocfilehash: ffb666ee331b55a4f04cad076c705e4bec980e03
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458125"
---
# <a name="itemshape"></a><span data-ttu-id="10bda-103">ItemShape</span><span class="sxs-lookup"><span data-stu-id="10bda-103">ItemShape</span></span>

<span data-ttu-id="10bda-104">**Itemshape**要素は、 [GetItem 操作](getitem-operation.md)、 [FindItem 操作](finditem-operation.md)、または[syncfolderitems 操作](syncfolderitems-operation.md)の応答で返される一連のプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="10bda-104">The **ItemShape** element identifies a set of properties to return in a [GetItem operation](getitem-operation.md), [FindItem operation](finditem-operation.md), or [SyncFolderItems operation](syncfolderitems-operation.md) response.</span></span> 
  
```XML
<ItemShape>
   <BaseShape/>
   <IncludeMimeContent/>
   <BodyType/>
   <FilterHtmlContent/>
   <ConvertHtmlCodePageToUTF8/>
   <AdditionalProperties/>
</ItemShape>
```

 <span data-ttu-id="10bda-105">**ItemResponseShapeType**</span><span class="sxs-lookup"><span data-stu-id="10bda-105">**ItemResponseShapeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="10bda-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="10bda-106">Attributes and elements</span></span>

<span data-ttu-id="10bda-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="10bda-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="10bda-108">属性</span><span class="sxs-lookup"><span data-stu-id="10bda-108">Attributes</span></span>

<span data-ttu-id="10bda-109">なし。</span><span class="sxs-lookup"><span data-stu-id="10bda-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="10bda-110">子要素</span><span class="sxs-lookup"><span data-stu-id="10bda-110">Child elements</span></span>

|<span data-ttu-id="10bda-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="10bda-111">**Element**</span></span>|<span data-ttu-id="10bda-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="10bda-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="10bda-113">BaseShape</span><span class="sxs-lookup"><span data-stu-id="10bda-113">BaseShape</span></span>](baseshape.md) <br/> |<span data-ttu-id="10bda-114">アイテムまたはフォルダーの応答で返されるプロパティの基本的な構成を識別します。</span><span class="sxs-lookup"><span data-stu-id="10bda-114">Identifies the basic configuration of properties to return in an item or folder response.</span></span>  <br/> |
|[<span data-ttu-id="10bda-115">IncludeMimeContent</span><span class="sxs-lookup"><span data-stu-id="10bda-115">IncludeMimeContent</span></span>](includemimecontent.md) <br/> |<span data-ttu-id="10bda-116">アイテムのマルチパーパスインターネットメール内線 (MIME) コンテンツを応答で返すかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="10bda-116">Specifies whether the Multipurpose Internet Mail Extensions (MIME) content of an item is returned in the response.</span></span>  <br/> |
|[<span data-ttu-id="10bda-117">BodyType</span><span class="sxs-lookup"><span data-stu-id="10bda-117">BodyType</span></span>](bodytype.md) <br/> |<span data-ttu-id="10bda-118">応答で本文テキストを書式設定する方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="10bda-118">Identifies how the body text is formatted in the response.</span></span>  <br/> |
|[<span data-ttu-id="10bda-119">ConvertHtmlCodePageToUTF8</span><span class="sxs-lookup"><span data-stu-id="10bda-119">ConvertHtmlCodePageToUTF8</span></span>](converthtmlcodepagetoutf8.md) <br/> |<span data-ttu-id="10bda-120">アイテムの HTML 本文を UTF8 に変換するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="10bda-120">Indicates whether the item HTML body is converted to UTF8.</span></span>  <br/> |
|[<span data-ttu-id="10bda-121">FilterHtmlContent</span><span class="sxs-lookup"><span data-stu-id="10bda-121">FilterHtmlContent</span></span>](filterhtmlcontent.md) <br/> |<span data-ttu-id="10bda-122">HTML コンテンツフィルターを有効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="10bda-122">Specifies whether HTML content filtering is enabled.</span></span>  <br/> |
|[<span data-ttu-id="10bda-123">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="10bda-123">AdditionalProperties</span></span>](additionalproperties.md) <br/> |<span data-ttu-id="10bda-124">応答で返される追加のプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="10bda-124">Identifies additional properties to return in a response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="10bda-125">親要素</span><span class="sxs-lookup"><span data-stu-id="10bda-125">Parent elements</span></span>

|<span data-ttu-id="10bda-126">**要素**</span><span class="sxs-lookup"><span data-stu-id="10bda-126">**Element**</span></span>|<span data-ttu-id="10bda-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="10bda-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="10bda-128">GetItem</span><span class="sxs-lookup"><span data-stu-id="10bda-128">GetItem</span></span>](getitem.md) <br/> |<span data-ttu-id="10bda-129">Exchange ストア内のメールボックスからアイテムを取得するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="10bda-129">Defines a request to retrieve items from a mailbox in the Exchange store.</span></span>  <br/> <span data-ttu-id="10bda-130">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="10bda-130">The following is the XPath expression to this element:</span></span>  <br/>  `/GetItem` <br/> |
|[<span data-ttu-id="10bda-131">FindItem</span><span class="sxs-lookup"><span data-stu-id="10bda-131">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="10bda-132">フォルダーに含まれるすべてのアイテムを検索するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="10bda-132">Defines a request to find all items that are contained in a folder.</span></span>  <br/> <span data-ttu-id="10bda-133">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="10bda-133">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItem` <br/> |
|[<span data-ttu-id="10bda-134">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="10bda-134">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="10bda-135">Exchange ストアフォルダー内のアイテムを同期する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="10bda-135">Defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> <span data-ttu-id="10bda-136">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="10bda-136">The following is the XPath expression to this element:</span></span>  <br/>  `/SyncFolderItems` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="10bda-137">テキスト値</span><span class="sxs-lookup"><span data-stu-id="10bda-137">Text value</span></span>

<span data-ttu-id="10bda-138">なし。</span><span class="sxs-lookup"><span data-stu-id="10bda-138">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="10bda-139">注釈</span><span class="sxs-lookup"><span data-stu-id="10bda-139">Remarks</span></span>

<span data-ttu-id="10bda-140">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="10bda-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="10bda-141">要素の情報</span><span class="sxs-lookup"><span data-stu-id="10bda-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="10bda-142">Namespace</span><span class="sxs-lookup"><span data-stu-id="10bda-142">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="10bda-143">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="10bda-143">Schema Name</span></span>  <br/> |<span data-ttu-id="10bda-144">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="10bda-144">Messages schema</span></span>  <br/> |
|<span data-ttu-id="10bda-145">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="10bda-145">Validation File</span></span>  <br/> |<span data-ttu-id="10bda-146">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="10bda-146">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="10bda-147">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="10bda-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="10bda-148">正しくない</span><span class="sxs-lookup"><span data-stu-id="10bda-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="10bda-149">関連項目</span><span class="sxs-lookup"><span data-stu-id="10bda-149">See also</span></span>



<span data-ttu-id="10bda-150">
  [GetItem 操作](getitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="10bda-150">[GetItem operation](getitem-operation.md)</span></span>
  
<span data-ttu-id="10bda-151">
  [FindItem 操作](finditem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="10bda-151">[FindItem operation](finditem-operation.md)</span></span>
  
[<span data-ttu-id="10bda-152">SyncFolderItems 操作</span><span class="sxs-lookup"><span data-stu-id="10bda-152">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="10bda-153">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="10bda-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

