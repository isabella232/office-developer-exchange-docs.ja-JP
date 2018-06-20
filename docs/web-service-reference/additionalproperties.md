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
description: AdditionalProperties 要素は、GetItem、UpdateItem、CreateItem FindItem で使用するための追加のプロパティを識別するか、FindFolder 要求します。
ms.openlocfilehash: 64e4f1ee6b24cf8015b7893dc4a904ca8b32d58e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759288"
---
# <a name="additionalproperties"></a><span data-ttu-id="46f81-103">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="46f81-103">AdditionalProperties</span></span>

<span data-ttu-id="46f81-104">**AdditionalProperties**要素は、 [GetItem](getitem.md)、 [UpdateItem](updateitem.md)、 [CreateItem](createitem.md) [FindItem](finditem.md)で使用するための追加のプロパティを識別するか、 [FindFolder](findfolder.md)要求します。</span><span class="sxs-lookup"><span data-stu-id="46f81-104">The **AdditionalProperties** element identifies additional properties for use in [GetItem](getitem.md), [UpdateItem](updateitem.md), [CreateItem](createitem.md), [FindItem](finditem.md), or [FindFolder](findfolder.md) requests.</span></span> 
  
```xml
<AdditionalProperties>
   <ExtendedFieldURI/>
   <FieldURI/>
   <IndexedFieldURI/>
</AdditionalProperties>
```

 <span data-ttu-id="46f81-105">**NonEmptyArrayOfPathsToElementType**</span><span class="sxs-lookup"><span data-stu-id="46f81-105">**NonEmptyArrayOfPathsToElementType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="46f81-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="46f81-106">Attributes and elements</span></span>

<span data-ttu-id="46f81-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="46f81-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="46f81-108">属性</span><span class="sxs-lookup"><span data-stu-id="46f81-108">Attributes</span></span>

<span data-ttu-id="46f81-109">なし。</span><span class="sxs-lookup"><span data-stu-id="46f81-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="46f81-110">子要素</span><span class="sxs-lookup"><span data-stu-id="46f81-110">Child elements</span></span>

|<span data-ttu-id="46f81-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="46f81-111">**Element**</span></span>|<span data-ttu-id="46f81-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="46f81-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="46f81-113">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="46f81-113">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="46f81-114">取得、設定、または作成する拡張の MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="46f81-114">Identifies extended MAPI properties to get, set, or create.</span></span>  <br/> |
|[<span data-ttu-id="46f81-115">FieldURI</span><span class="sxs-lookup"><span data-stu-id="46f81-115">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="46f81-116">URI によって頻繁に参照されるプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="46f81-116">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="46f81-117">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="46f81-117">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="46f81-118">URI によって頻繁に参照される辞書のプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="46f81-118">Identifies frequently referenced dictionary properties by URI.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="46f81-119">親要素</span><span class="sxs-lookup"><span data-stu-id="46f81-119">Parent elements</span></span>

|<span data-ttu-id="46f81-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="46f81-120">**Element**</span></span>|<span data-ttu-id="46f81-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="46f81-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="46f81-122">FolderShape</span><span class="sxs-lookup"><span data-stu-id="46f81-122">FolderShape</span></span>](foldershape.md) <br/> | <span data-ttu-id="46f81-123">[GetFolder](getfolder.md)、 [FindFolder](findfolder.md)、または[SyncFolderHierarchy](syncfolderhierarchy.md)の応答に含めるフォルダーのプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="46f81-123">Identifies the folder properties to include in a [GetFolder](getfolder.md), [FindFolder](findfolder.md), or [SyncFolderHierarchy](syncfolderhierarchy.md) response.</span></span><br/><br/>  <span data-ttu-id="46f81-124">この要素への XPath 式は、次のように。</span><span class="sxs-lookup"><span data-stu-id="46f81-124">The following are the XPath expressions to this element:</span></span><br/><br/>  `/FindFolder/FolderShape` <br/>  `/GetFolder/FolderShape` <br/>  `/SyncFolderHierarchy/FolderShape` <br/> |
|[<span data-ttu-id="46f81-125">ItemShape</span><span class="sxs-lookup"><span data-stu-id="46f81-125">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="46f81-126">[GetItem](getitem.md)、 [FindItem](finditem.md)、または[SyncFolderItems](syncfolderitems.md)の応答に含めるコンテンツ アイテムのプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="46f81-126">Identifies the item properties and content to include in a [GetItem](getitem.md), [FindItem](finditem.md), or [SyncFolderItems](syncfolderitems.md) response.</span></span><br/><br/>  <span data-ttu-id="46f81-127">この要素への XPath 式は、次のように。</span><span class="sxs-lookup"><span data-stu-id="46f81-127">The following are the XPath expressions to this element:</span></span><br/><br/>  `/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/> |
|[<span data-ttu-id="46f81-128">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="46f81-128">AttachmentShape</span></span>](attachmentshape.md) <br/> |<span data-ttu-id="46f81-129">[GetItem](getitem.md)要求への応答で返されるその他の拡張アイテム プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="46f81-129">Identifies additional extended item properties to return in a response to a [GetItem](getitem.md) request.</span></span><br/><br/> <span data-ttu-id="46f81-130">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="46f81-130">The following is the XPath expression to this element:</span></span><br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="46f81-131">備考</span><span class="sxs-lookup"><span data-stu-id="46f81-131">Remarks</span></span>

<span data-ttu-id="46f81-132">[GetItem](getitem.md)、 [UpdateItem](updateitem.md)、 [createitem メソッド](createitem.md)、 [FindItem](finditem.md)、 [FindFolder](findfolder.md)要求には、すべての子要素を使用できます。</span><span class="sxs-lookup"><span data-stu-id="46f81-132">Not all the child elements can be used with [GetItem](getitem.md), [UpdateItem](updateitem.md), [CreateItem](createitem.md), [FindItem](finditem.md), or [FindFolder](findfolder.md) requests.</span></span> <span data-ttu-id="46f81-133">プロパティは、フォルダーまたはアクセスされているアイテムに適用可能である必要があります。</span><span class="sxs-lookup"><span data-stu-id="46f81-133">The property must be applicable to the folder or item that is accessed.</span></span> <span data-ttu-id="46f81-134">その他のプロパティにアクセスするのにには、拡張プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="46f81-134">Use extended properties to access other properties.</span></span> <span data-ttu-id="46f81-135">特定のアイテムのプロパティが存在しない場合は、対応する要素を発しない結果の XML にします。</span><span class="sxs-lookup"><span data-stu-id="46f81-135">If the property does not exist for a given item, no corresponding element will be emitted into the resulting XML.</span></span> 
  
<span data-ttu-id="46f81-136">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="46f81-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="46f81-137">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="46f81-137">This element is optional.</span></span>
  
## <a name="example"></a><span data-ttu-id="46f81-138">例</span><span class="sxs-lookup"><span data-stu-id="46f81-138">Example</span></span>

<span data-ttu-id="46f81-139">要求の次の例では、 **AdditionalProperties**要素を使用して、アイテムの件名を取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="46f81-139">The following request example shows how to get an item subject by using the **AdditionalProperties** element.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a><span data-ttu-id="46f81-140">要素情報</span><span class="sxs-lookup"><span data-stu-id="46f81-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="46f81-141">名前空間</span><span class="sxs-lookup"><span data-stu-id="46f81-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="46f81-142">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="46f81-142">Schema Name</span></span>  <br/> |<span data-ttu-id="46f81-143">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="46f81-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="46f81-144">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="46f81-144">Validation File</span></span>  <br/> |<span data-ttu-id="46f81-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="46f81-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="46f81-146">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="46f81-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="46f81-147">いいえ</span><span class="sxs-lookup"><span data-stu-id="46f81-147">False</span></span>  <br/> |
   

