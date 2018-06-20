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
description: ItemShape 要素は、GetItem 操作、FindItem 操作、または SyncFolderItems 操作の応答で返されるプロパティのセットを識別します。
ms.openlocfilehash: 95174a85a8fa05cb2612e1289d46c8db32b6e052
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832191"
---
# <a name="itemshape"></a><span data-ttu-id="9f3f0-103">ItemShape</span><span class="sxs-lookup"><span data-stu-id="9f3f0-103">ItemShape</span></span>

<span data-ttu-id="9f3f0-104">**ItemShape**要素は、 [GetItem 操作](getitem-operation.md)、 [FindItem 操作](finditem-operation.md)、または[SyncFolderItems の操作](syncfolderitems-operation.md)の応答で返されるプロパティのセットを識別します。</span><span class="sxs-lookup"><span data-stu-id="9f3f0-104">The **ItemShape** element identifies a set of properties to return in a [GetItem operation](getitem-operation.md), [FindItem operation](finditem-operation.md), or [SyncFolderItems operation](syncfolderitems-operation.md) response.</span></span> 
  
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

 <span data-ttu-id="9f3f0-105">**ItemResponseShapeType**</span><span class="sxs-lookup"><span data-stu-id="9f3f0-105">**ItemResponseShapeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9f3f0-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9f3f0-106">Attributes and elements</span></span>

<span data-ttu-id="9f3f0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9f3f0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9f3f0-108">属性</span><span class="sxs-lookup"><span data-stu-id="9f3f0-108">Attributes</span></span>

<span data-ttu-id="9f3f0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9f3f0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9f3f0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9f3f0-110">Child elements</span></span>

|<span data-ttu-id="9f3f0-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="9f3f0-111">**Element**</span></span>|<span data-ttu-id="9f3f0-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="9f3f0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f3f0-113">BaseShape</span><span class="sxs-lookup"><span data-stu-id="9f3f0-113">BaseShape</span></span>](baseshape.md) <br/> |<span data-ttu-id="9f3f0-114">アイテムまたはフォルダーの応答で返されるプロパティの基本構成を識別します。</span><span class="sxs-lookup"><span data-stu-id="9f3f0-114">Identifies the basic configuration of properties to return in an item or folder response.</span></span>  <br/> |
|[<span data-ttu-id="9f3f0-115">IncludeMimeContent</span><span class="sxs-lookup"><span data-stu-id="9f3f0-115">IncludeMimeContent</span></span>](includemimecontent.md) <br/> |<span data-ttu-id="9f3f0-116">応答で、多目的インターネット メール拡張 (MIME) のコンテンツ項目を返すかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="9f3f0-116">Specifies whether the Multipurpose Internet Mail Extensions (MIME) content of an item is returned in the response.</span></span>  <br/> |
|[<span data-ttu-id="9f3f0-117">BodyType</span><span class="sxs-lookup"><span data-stu-id="9f3f0-117">BodyType</span></span>](bodytype.md) <br/> |<span data-ttu-id="9f3f0-118">応答の本文のテキストを書式設定する方法を識別します。</span><span class="sxs-lookup"><span data-stu-id="9f3f0-118">Identifies how the body text is formatted in the response.</span></span>  <br/> |
|[<span data-ttu-id="9f3f0-119">ConvertHtmlCodePageToUTF8</span><span class="sxs-lookup"><span data-stu-id="9f3f0-119">ConvertHtmlCodePageToUTF8</span></span>](converthtmlcodepagetoutf8.md) <br/> |<span data-ttu-id="9f3f0-120">項目の HTML 本文が UTF8 に変換されるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9f3f0-120">Indicates whether the item HTML body is converted to UTF8.</span></span>  <br/> |
|[<span data-ttu-id="9f3f0-121">FilterHtmlContent</span><span class="sxs-lookup"><span data-stu-id="9f3f0-121">FilterHtmlContent</span></span>](filterhtmlcontent.md) <br/> |<span data-ttu-id="9f3f0-122">HTML コンテンツのフィルタ リングが有効になっているかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="9f3f0-122">Specifies whether HTML content filtering is enabled.</span></span>  <br/> |
|[<span data-ttu-id="9f3f0-123">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="9f3f0-123">AdditionalProperties</span></span>](additionalproperties.md) <br/> |<span data-ttu-id="9f3f0-124">応答で返される追加プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="9f3f0-124">Identifies additional properties to return in a response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9f3f0-125">親要素</span><span class="sxs-lookup"><span data-stu-id="9f3f0-125">Parent elements</span></span>

|<span data-ttu-id="9f3f0-126">**要素**</span><span class="sxs-lookup"><span data-stu-id="9f3f0-126">**Element**</span></span>|<span data-ttu-id="9f3f0-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="9f3f0-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f3f0-128">GetItem</span><span class="sxs-lookup"><span data-stu-id="9f3f0-128">GetItem</span></span>](getitem.md) <br/> |<span data-ttu-id="9f3f0-129">Exchange ストア内のメールボックスからアイテムを取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="9f3f0-129">Defines a request to retrieve items from a mailbox in the Exchange store.</span></span>  <br/> <span data-ttu-id="9f3f0-130">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="9f3f0-130">The following is the XPath expression to this element:</span></span>  <br/>  `/GetItem` <br/> |
|[<span data-ttu-id="9f3f0-131">FindItem</span><span class="sxs-lookup"><span data-stu-id="9f3f0-131">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="9f3f0-132">フォルダーに含まれるすべての項目を検索するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="9f3f0-132">Defines a request to find all items that are contained in a folder.</span></span>  <br/> <span data-ttu-id="9f3f0-133">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="9f3f0-133">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItem` <br/> |
|[<span data-ttu-id="9f3f0-134">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="9f3f0-134">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="9f3f0-135">Exchange ストア フォルダー内のアイテムを同期するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="9f3f0-135">Defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> <span data-ttu-id="9f3f0-136">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="9f3f0-136">The following is the XPath expression to this element:</span></span>  <br/>  `/SyncFolderItems` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9f3f0-137">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9f3f0-137">Text value</span></span>

<span data-ttu-id="9f3f0-138">なし。</span><span class="sxs-lookup"><span data-stu-id="9f3f0-138">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9f3f0-139">備考</span><span class="sxs-lookup"><span data-stu-id="9f3f0-139">Remarks</span></span>

<span data-ttu-id="9f3f0-140">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9f3f0-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9f3f0-141">要素情報</span><span class="sxs-lookup"><span data-stu-id="9f3f0-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9f3f0-142">名前空間</span><span class="sxs-lookup"><span data-stu-id="9f3f0-142">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9f3f0-143">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9f3f0-143">Schema Name</span></span>  <br/> |<span data-ttu-id="9f3f0-144">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="9f3f0-144">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9f3f0-145">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9f3f0-145">Validation File</span></span>  <br/> |<span data-ttu-id="9f3f0-146">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9f3f0-146">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9f3f0-147">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9f3f0-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="9f3f0-148">False</span><span class="sxs-lookup"><span data-stu-id="9f3f0-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9f3f0-149">関連項目</span><span class="sxs-lookup"><span data-stu-id="9f3f0-149">See also</span></span>



<span data-ttu-id="9f3f0-150">
  [GetItem 操作](getitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="9f3f0-150">[GetItem operation](getitem-operation.md)</span></span>
  
<span data-ttu-id="9f3f0-151">
  [FindItem 操作](finditem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="9f3f0-151">[FindItem operation](finditem-operation.md)</span></span>
  
[<span data-ttu-id="9f3f0-152">SyncFolderItems の操作</span><span class="sxs-lookup"><span data-stu-id="9f3f0-152">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="9f3f0-153">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="9f3f0-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

