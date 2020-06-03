---
title: AdditionalProperties
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AdditionalProperties
api_type:
- schema
ms.assetid: 7a269aed-dcfd-4c3e-9e14-094e53828101
description: AdditionalProperties 要素は、GetItem、UpdateItem、CreateItem、FindItem、または FindFolder 要求で使用する追加のプロパティを示します。
ms.openlocfilehash: 90a307ba4d5ece10e15d2cec56cf5042c3d38685
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455815"
---
# <a name="additionalproperties"></a><span data-ttu-id="d20a5-103">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="d20a5-103">AdditionalProperties</span></span>

<span data-ttu-id="d20a5-104">**Additionalproperties**要素は、 [GetItem](getitem.md)、 [updateitem](updateitem.md)、 [CreateItem](createitem.md)、 [FindItem](finditem.md)、または[findfolder](findfolder.md)要求で使用する追加のプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d20a5-104">The **AdditionalProperties** element identifies additional properties for use in [GetItem](getitem.md), [UpdateItem](updateitem.md), [CreateItem](createitem.md), [FindItem](finditem.md), or [FindFolder](findfolder.md) requests.</span></span> 
  
```xml
<AdditionalProperties>
   <ExtendedFieldURI/>
   <FieldURI/>
   <IndexedFieldURI/>
</AdditionalProperties>
```

 <span data-ttu-id="d20a5-105">**NonEmptyArrayOfPathsToElementType**</span><span class="sxs-lookup"><span data-stu-id="d20a5-105">**NonEmptyArrayOfPathsToElementType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d20a5-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d20a5-106">Attributes and elements</span></span>

<span data-ttu-id="d20a5-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d20a5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d20a5-108">属性</span><span class="sxs-lookup"><span data-stu-id="d20a5-108">Attributes</span></span>

<span data-ttu-id="d20a5-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d20a5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d20a5-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d20a5-110">Child elements</span></span>

|<span data-ttu-id="d20a5-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="d20a5-111">**Element**</span></span>|<span data-ttu-id="d20a5-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d20a5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d20a5-113">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="d20a5-113">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="d20a5-114">取得、設定、または作成する拡張 MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="d20a5-114">Identifies extended MAPI properties to get, set, or create.</span></span>  <br/> |
|[<span data-ttu-id="d20a5-115">FieldURI</span><span class="sxs-lookup"><span data-stu-id="d20a5-115">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="d20a5-116">URI で頻繁に参照されるプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="d20a5-116">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="d20a5-117">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="d20a5-117">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="d20a5-118">URI で頻繁に参照される dictionary プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="d20a5-118">Identifies frequently referenced dictionary properties by URI.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d20a5-119">親要素</span><span class="sxs-lookup"><span data-stu-id="d20a5-119">Parent elements</span></span>

|<span data-ttu-id="d20a5-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="d20a5-120">**Element**</span></span>|<span data-ttu-id="d20a5-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="d20a5-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d20a5-122">FolderShape</span><span class="sxs-lookup"><span data-stu-id="d20a5-122">FolderShape</span></span>](foldershape.md) <br/> | <span data-ttu-id="d20a5-123">[Getfolder](getfolder.md)、 [findfolder](findfolder.md)、または[syncfolderhierarchy](syncfolderhierarchy.md)の応答に含めるフォルダーのプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="d20a5-123">Identifies the folder properties to include in a [GetFolder](getfolder.md), [FindFolder](findfolder.md), or [SyncFolderHierarchy](syncfolderhierarchy.md) response.</span></span><br/><br/>  <span data-ttu-id="d20a5-124">この要素の XPath 式は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="d20a5-124">The following are the XPath expressions to this element:</span></span><br/><br/>  `/FindFolder/FolderShape` <br/>  `/GetFolder/FolderShape` <br/>  `/SyncFolderHierarchy/FolderShape` <br/> |
|[<span data-ttu-id="d20a5-125">ItemShape</span><span class="sxs-lookup"><span data-stu-id="d20a5-125">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="d20a5-126">[GetItem](getitem.md)、 [FindItem](finditem.md)、または[syncfolderitems](syncfolderitems.md)応答に含めるアイテムのプロパティとコンテンツを指定します。</span><span class="sxs-lookup"><span data-stu-id="d20a5-126">Identifies the item properties and content to include in a [GetItem](getitem.md), [FindItem](finditem.md), or [SyncFolderItems](syncfolderitems.md) response.</span></span><br/><br/>  <span data-ttu-id="d20a5-127">この要素の XPath 式は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="d20a5-127">The following are the XPath expressions to this element:</span></span><br/><br/>  `/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/> |
|[<span data-ttu-id="d20a5-128">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="d20a5-128">AttachmentShape</span></span>](attachmentshape.md) <br/> |<span data-ttu-id="d20a5-129">[GetItem](getitem.md)要求に対する応答で返される追加の拡張アイテムプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="d20a5-129">Identifies additional extended item properties to return in a response to a [GetItem](getitem.md) request.</span></span><br/><br/> <span data-ttu-id="d20a5-130">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d20a5-130">The following is the XPath expression to this element:</span></span><br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d20a5-131">注釈</span><span class="sxs-lookup"><span data-stu-id="d20a5-131">Remarks</span></span>

<span data-ttu-id="d20a5-132">[GetItem](getitem.md)、 [updateitem](updateitem.md)、 [CreateItem](createitem.md)、 [FindItem](finditem.md)、または[findfolder](findfolder.md)要求では、すべての子要素を使用できるわけではありません。</span><span class="sxs-lookup"><span data-stu-id="d20a5-132">Not all the child elements can be used with [GetItem](getitem.md), [UpdateItem](updateitem.md), [CreateItem](createitem.md), [FindItem](finditem.md), or [FindFolder](findfolder.md) requests.</span></span> <span data-ttu-id="d20a5-133">このプロパティは、アクセスされるフォルダーまたはアイテムに適用される必要があります。</span><span class="sxs-lookup"><span data-stu-id="d20a5-133">The property must be applicable to the folder or item that is accessed.</span></span> <span data-ttu-id="d20a5-134">他のプロパティにアクセスするには、拡張プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="d20a5-134">Use extended properties to access other properties.</span></span> <span data-ttu-id="d20a5-135">指定したアイテムのプロパティが存在しない場合、対応する要素は結果の XML に出力されません。</span><span class="sxs-lookup"><span data-stu-id="d20a5-135">If the property does not exist for a given item, no corresponding element will be emitted into the resulting XML.</span></span> 
  
<span data-ttu-id="d20a5-136">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="d20a5-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="d20a5-137">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="d20a5-137">This element is optional.</span></span>
  
## <a name="example"></a><span data-ttu-id="d20a5-138">例</span><span class="sxs-lookup"><span data-stu-id="d20a5-138">Example</span></span>

<span data-ttu-id="d20a5-139">次の要求例は、 **Additionalproperties**要素を使用してアイテムの件名を取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="d20a5-139">The following request example shows how to get an item subject by using the **AdditionalProperties** element.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject"/>
        </t:AdditionalProperties>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="ASkAS="/>
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="d20a5-140">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d20a5-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d20a5-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="d20a5-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d20a5-142">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d20a5-142">Schema Name</span></span>  <br/> |<span data-ttu-id="d20a5-143">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d20a5-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="d20a5-144">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d20a5-144">Validation File</span></span>  <br/> |<span data-ttu-id="d20a5-145">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d20a5-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d20a5-146">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d20a5-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="d20a5-147">いいえ</span><span class="sxs-lookup"><span data-stu-id="d20a5-147">False</span></span>  <br/> |
   

