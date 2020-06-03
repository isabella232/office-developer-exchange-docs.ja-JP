---
title: BodyType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BodyType
api_type:
- schema
ms.assetid: d42ec77b-fb9f-404a-9bf2-1801e8744676
description: BodyType 要素は、本文テキストがどのように応答で書式設定されるかを識別します。
ms.openlocfilehash: 448d20ac54b09a2f4f6a273a1099519371ac7f5b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465948"
---
# <a name="bodytype"></a><span data-ttu-id="e9459-103">BodyType</span><span class="sxs-lookup"><span data-stu-id="e9459-103">BodyType</span></span>

<span data-ttu-id="e9459-104">**Bodytype**要素は、本文テキストがどのように応答で書式設定されるかを識別します。</span><span class="sxs-lookup"><span data-stu-id="e9459-104">The **BodyType** element identifies how the body text is formatted in the response.</span></span> 
  
```xml
<BodyType>Best or HTML or Text</BodyType>
```

<span data-ttu-id="e9459-105">**BodyTypeResponseType**</span><span class="sxs-lookup"><span data-stu-id="e9459-105">**BodyTypeResponseType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="e9459-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e9459-106">Attributes and elements</span></span>

<span data-ttu-id="e9459-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e9459-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e9459-108">属性</span><span class="sxs-lookup"><span data-stu-id="e9459-108">Attributes</span></span>

<span data-ttu-id="e9459-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e9459-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e9459-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e9459-110">Child elements</span></span>

<span data-ttu-id="e9459-111">なし。</span><span class="sxs-lookup"><span data-stu-id="e9459-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e9459-112">親要素</span><span class="sxs-lookup"><span data-stu-id="e9459-112">Parent elements</span></span>

|<span data-ttu-id="e9459-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="e9459-113">**Element**</span></span>|<span data-ttu-id="e9459-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="e9459-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9459-115">ItemShape</span><span class="sxs-lookup"><span data-stu-id="e9459-115">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="e9459-116">GetItem、FindItem、または SyncFolderItems 応答に含めるアイテムのプロパティとコンテンツを指定します。</span><span class="sxs-lookup"><span data-stu-id="e9459-116">Identifies the item properties and content to include in a GetItem, FindItem, or SyncFolderItems response.</span></span>  <br/><br/><span data-ttu-id="e9459-117">この要素の XPath 式は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="e9459-117">The following are the XPath expressions to this element:</span></span><br/><br/>  `/GetItem/ItemShape`<br/><br/>`/FindItem/ItemShape`<br/><br/>`/SyncFolderItems/ItemShape` <br/> |
|[<span data-ttu-id="e9459-118">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="e9459-118">AttachmentShape</span></span>](attachmentshape.md) <br/> |<span data-ttu-id="e9459-119">[Getattachment](getattachment.md)要求に対する応答で返される追加の拡張アイテムプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="e9459-119">Identifies additional extended item properties to return in a response to a [GetAttachment](getattachment.md) request.</span></span>  <br/><br/><span data-ttu-id="e9459-120">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e9459-120">The following is the XPath expression to this element:</span></span><br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e9459-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e9459-121">Text value</span></span>

<span data-ttu-id="e9459-122">**Bodytype**要素に使用できる値を次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="e9459-122">The following table lists the possible values for the **BodyType** element.</span></span> 
  
|<span data-ttu-id="e9459-123">**値**</span><span class="sxs-lookup"><span data-stu-id="e9459-123">**Value**</span></span>|<span data-ttu-id="e9459-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="e9459-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e9459-125">高</span><span class="sxs-lookup"><span data-stu-id="e9459-125">Best</span></span>  <br/> |<span data-ttu-id="e9459-126">応答によって、本文の中で最も豊富な利用可能なコンテンツが返されます。</span><span class="sxs-lookup"><span data-stu-id="e9459-126">The response will return the richest available content of body text.</span></span> <span data-ttu-id="e9459-127">これは、コンテンツがテキストであるか HTML であるかにかかわらず、不明な場合に便利です。</span><span class="sxs-lookup"><span data-stu-id="e9459-127">This is useful if it is unknown whether the content is text or HTML.</span></span><br/><br/> <span data-ttu-id="e9459-128">保存された本文がプレーンテキストの場合、返される本文はテキストになります。</span><span class="sxs-lookup"><span data-stu-id="e9459-128">The returned body will be text if the stored body is plain text.</span></span> <span data-ttu-id="e9459-129">それ以外の場合、保存された本文が HTML または RTF 形式の場合、応答は HTML を返します。</span><span class="sxs-lookup"><span data-stu-id="e9459-129">Otherwise, the response will return HTML if the stored body is in either HTML or RTF format.</span></span><br/><br/> <span data-ttu-id="e9459-130">これは既定の値です。</span><span class="sxs-lookup"><span data-stu-id="e9459-130">This is the default value.</span></span>  <br/> |
|<span data-ttu-id="e9459-131">HTML</span><span class="sxs-lookup"><span data-stu-id="e9459-131">HTML</span></span>  <br/> |<span data-ttu-id="e9459-132">応答は、アイテムの本文を HTML として返します。</span><span class="sxs-lookup"><span data-stu-id="e9459-132">The response will return an item body as HTML.</span></span>  <br/> |
|<span data-ttu-id="e9459-133">テキスト</span><span class="sxs-lookup"><span data-stu-id="e9459-133">Text</span></span>  <br/> |<span data-ttu-id="e9459-134">応答は、アイテムの本文をプレーンテキストとして返します。</span><span class="sxs-lookup"><span data-stu-id="e9459-134">The response will return an item body as plain text.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e9459-135">注釈</span><span class="sxs-lookup"><span data-stu-id="e9459-135">Remarks</span></span>

<span data-ttu-id="e9459-136">応答で返される本文の種類を特定するには、 [body](body.md)要素の**bodytype**属性をチェックします。</span><span class="sxs-lookup"><span data-stu-id="e9459-136">You can identify the type of body returned in the response by checking the **BodyType** attribute of the [Body](body.md) element.</span></span> <span data-ttu-id="e9459-137">**Bodytype**属性は、本文を HTML またはテキストのいずれかとして識別します。</span><span class="sxs-lookup"><span data-stu-id="e9459-137">The **BodyType** attribute will identify the body as either HTML or text.</span></span> 
  
<span data-ttu-id="e9459-138">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="e9459-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="e9459-139">例</span><span class="sxs-lookup"><span data-stu-id="e9459-139">Example</span></span>

<span data-ttu-id="e9459-140">次の要求の例は、 **Bodytype**要素が使用されている場所を示しています。</span><span class="sxs-lookup"><span data-stu-id="e9459-140">The following example of a request shows where a **BodyType** element is used.</span></span> 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape>
        <t:BodyType>Best</t:BodyType>
      </AttachmentShape>
      <AttachmentIds>
        <t:AttachmentId Id="ASkAS="/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="e9459-141">Id 属性は読みやすくするために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="e9459-141">The Id attribute has been shortened to preserve readability.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e9459-142">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e9459-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e9459-143">Namespace</span><span class="sxs-lookup"><span data-stu-id="e9459-143">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e9459-144">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e9459-144">Schema Name</span></span>  <br/> |<span data-ttu-id="e9459-145">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="e9459-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="e9459-146">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e9459-146">Validation File</span></span>  <br/> |<span data-ttu-id="e9459-147">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="e9459-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e9459-148">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e9459-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="e9459-149">いいえ</span><span class="sxs-lookup"><span data-stu-id="e9459-149">False</span></span>  <br/> |
   

