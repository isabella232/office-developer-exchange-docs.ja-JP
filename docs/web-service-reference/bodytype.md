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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465948"
---
# <a name="bodytype"></a><span data-ttu-id="94909-103">BodyType</span><span class="sxs-lookup"><span data-stu-id="94909-103">BodyType</span></span>

<span data-ttu-id="94909-104">**Bodytype**要素は、本文テキストがどのように応答で書式設定されるかを識別します。</span><span class="sxs-lookup"><span data-stu-id="94909-104">The **BodyType** element identifies how the body text is formatted in the response.</span></span> 
  
```xml
<BodyType>Best or HTML or Text</BodyType>
```

<span data-ttu-id="94909-105">**BodyTypeResponseType**</span><span class="sxs-lookup"><span data-stu-id="94909-105">**BodyTypeResponseType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="94909-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="94909-106">Attributes and elements</span></span>

<span data-ttu-id="94909-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="94909-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="94909-108">属性</span><span class="sxs-lookup"><span data-stu-id="94909-108">Attributes</span></span>

<span data-ttu-id="94909-109">なし。</span><span class="sxs-lookup"><span data-stu-id="94909-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="94909-110">子要素</span><span class="sxs-lookup"><span data-stu-id="94909-110">Child elements</span></span>

<span data-ttu-id="94909-111">なし。</span><span class="sxs-lookup"><span data-stu-id="94909-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="94909-112">親要素</span><span class="sxs-lookup"><span data-stu-id="94909-112">Parent elements</span></span>

|<span data-ttu-id="94909-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="94909-113">**Element**</span></span>|<span data-ttu-id="94909-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="94909-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="94909-115">ItemShape</span><span class="sxs-lookup"><span data-stu-id="94909-115">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="94909-116">GetItem、FindItem、または SyncFolderItems 応答に含めるアイテムのプロパティとコンテンツを指定します。</span><span class="sxs-lookup"><span data-stu-id="94909-116">Identifies the item properties and content to include in a GetItem, FindItem, or SyncFolderItems response.</span></span>  <br/><br/><span data-ttu-id="94909-117">この要素の XPath 式は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="94909-117">The following are the XPath expressions to this element:</span></span><br/><br/>  `/GetItem/ItemShape`<br/><br/>`/FindItem/ItemShape`<br/><br/>`/SyncFolderItems/ItemShape` <br/> |
|[<span data-ttu-id="94909-118">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="94909-118">AttachmentShape</span></span>](attachmentshape.md) <br/> |<span data-ttu-id="94909-119">[Getattachment](getattachment.md)要求に対する応答で返される追加の拡張アイテムプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="94909-119">Identifies additional extended item properties to return in a response to a [GetAttachment](getattachment.md) request.</span></span>  <br/><br/><span data-ttu-id="94909-120">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="94909-120">The following is the XPath expression to this element:</span></span><br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="94909-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="94909-121">Text value</span></span>

<span data-ttu-id="94909-122">**Bodytype**要素に使用できる値を次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="94909-122">The following table lists the possible values for the **BodyType** element.</span></span> 
  
|<span data-ttu-id="94909-123">**値**</span><span class="sxs-lookup"><span data-stu-id="94909-123">**Value**</span></span>|<span data-ttu-id="94909-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="94909-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="94909-125">高</span><span class="sxs-lookup"><span data-stu-id="94909-125">Best</span></span>  <br/> |<span data-ttu-id="94909-126">応答によって、本文の中で最も豊富な利用可能なコンテンツが返されます。</span><span class="sxs-lookup"><span data-stu-id="94909-126">The response will return the richest available content of body text.</span></span> <span data-ttu-id="94909-127">これは、コンテンツがテキストであるか HTML であるかにかかわらず、不明な場合に便利です。</span><span class="sxs-lookup"><span data-stu-id="94909-127">This is useful if it is unknown whether the content is text or HTML.</span></span><br/><br/> <span data-ttu-id="94909-128">保存された本文がプレーンテキストの場合、返される本文はテキストになります。</span><span class="sxs-lookup"><span data-stu-id="94909-128">The returned body will be text if the stored body is plain text.</span></span> <span data-ttu-id="94909-129">それ以外の場合、保存された本文が HTML または RTF 形式の場合、応答は HTML を返します。</span><span class="sxs-lookup"><span data-stu-id="94909-129">Otherwise, the response will return HTML if the stored body is in either HTML or RTF format.</span></span><br/><br/> <span data-ttu-id="94909-130">これは既定の値です。</span><span class="sxs-lookup"><span data-stu-id="94909-130">This is the default value.</span></span>  <br/> |
|<span data-ttu-id="94909-131">HTML</span><span class="sxs-lookup"><span data-stu-id="94909-131">HTML</span></span>  <br/> |<span data-ttu-id="94909-132">応答は、アイテムの本文を HTML として返します。</span><span class="sxs-lookup"><span data-stu-id="94909-132">The response will return an item body as HTML.</span></span>  <br/> |
|<span data-ttu-id="94909-133">テキスト</span><span class="sxs-lookup"><span data-stu-id="94909-133">Text</span></span>  <br/> |<span data-ttu-id="94909-134">応答は、アイテムの本文をプレーンテキストとして返します。</span><span class="sxs-lookup"><span data-stu-id="94909-134">The response will return an item body as plain text.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="94909-135">注釈</span><span class="sxs-lookup"><span data-stu-id="94909-135">Remarks</span></span>

<span data-ttu-id="94909-136">応答で返される本文の種類を特定するには、 [body](body.md)要素の**bodytype**属性をチェックします。</span><span class="sxs-lookup"><span data-stu-id="94909-136">You can identify the type of body returned in the response by checking the **BodyType** attribute of the [Body](body.md) element.</span></span> <span data-ttu-id="94909-137">**Bodytype**属性は、本文を HTML またはテキストのいずれかとして識別します。</span><span class="sxs-lookup"><span data-stu-id="94909-137">The **BodyType** attribute will identify the body as either HTML or text.</span></span> 
  
<span data-ttu-id="94909-138">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="94909-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="94909-139">例</span><span class="sxs-lookup"><span data-stu-id="94909-139">Example</span></span>

<span data-ttu-id="94909-140">次の要求の例は、 **Bodytype**要素が使用されている場所を示しています。</span><span class="sxs-lookup"><span data-stu-id="94909-140">The following example of a request shows where a **BodyType** element is used.</span></span> 
  
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

<span data-ttu-id="94909-141">Id 属性は読みやすくするために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="94909-141">The Id attribute has been shortened to preserve readability.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="94909-142">要素の情報</span><span class="sxs-lookup"><span data-stu-id="94909-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="94909-143">Namespace</span><span class="sxs-lookup"><span data-stu-id="94909-143">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="94909-144">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="94909-144">Schema Name</span></span>  <br/> |<span data-ttu-id="94909-145">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="94909-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="94909-146">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="94909-146">Validation File</span></span>  <br/> |<span data-ttu-id="94909-147">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="94909-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="94909-148">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="94909-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="94909-149">いいえ</span><span class="sxs-lookup"><span data-stu-id="94909-149">False</span></span>  <br/> |
   

