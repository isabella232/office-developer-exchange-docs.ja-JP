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
description: BodyType 要素は、応答の本文のテキストを書式設定する方法を識別します。
ms.openlocfilehash: f8be2e96390b40faa367cf0d34c533accc3b8afb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759537"
---
# <a name="bodytype"></a><span data-ttu-id="28023-103">BodyType</span><span class="sxs-lookup"><span data-stu-id="28023-103">BodyType</span></span>

<span data-ttu-id="28023-104">**BodyType**要素は、応答の本文のテキストを書式設定する方法を識別します。</span><span class="sxs-lookup"><span data-stu-id="28023-104">The **BodyType** element identifies how the body text is formatted in the response.</span></span> 
  
```xml
<BodyType>Best or HTML or Text</BodyType>
```

<span data-ttu-id="28023-105">**BodyTypeResponseType**</span><span class="sxs-lookup"><span data-stu-id="28023-105">**BodyTypeResponseType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="28023-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="28023-106">Attributes and elements</span></span>

<span data-ttu-id="28023-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="28023-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="28023-108">属性</span><span class="sxs-lookup"><span data-stu-id="28023-108">Attributes</span></span>

<span data-ttu-id="28023-109">なし。</span><span class="sxs-lookup"><span data-stu-id="28023-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="28023-110">子要素</span><span class="sxs-lookup"><span data-stu-id="28023-110">Child elements</span></span>

<span data-ttu-id="28023-111">なし。</span><span class="sxs-lookup"><span data-stu-id="28023-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="28023-112">親要素</span><span class="sxs-lookup"><span data-stu-id="28023-112">Parent elements</span></span>

|<span data-ttu-id="28023-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="28023-113">**Element**</span></span>|<span data-ttu-id="28023-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="28023-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="28023-115">ItemShape</span><span class="sxs-lookup"><span data-stu-id="28023-115">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="28023-116">GetItem、FindItem、または SyncFolderItems の応答に含めるコンテンツ アイテムのプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="28023-116">Identifies the item properties and content to include in a GetItem, FindItem, or SyncFolderItems response.</span></span>  <br/><br/><span data-ttu-id="28023-117">この要素への XPath 式は、次のように。</span><span class="sxs-lookup"><span data-stu-id="28023-117">The following are the XPath expressions to this element:</span></span><br/><br/>  `/GetItem/ItemShape`<br/><br/>`/FindItem/ItemShape`<br/><br/>`/SyncFolderItems/ItemShape` <br/> |
|[<span data-ttu-id="28023-118">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="28023-118">AttachmentShape</span></span>](attachmentshape.md) <br/> |<span data-ttu-id="28023-119">[GetAttachment](getattachment.md)要求への応答で返されるその他の拡張アイテム プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="28023-119">Identifies additional extended item properties to return in a response to a [GetAttachment](getattachment.md) request.</span></span>  <br/><br/><span data-ttu-id="28023-120">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="28023-120">The following is the XPath expression to this element:</span></span><br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="28023-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="28023-121">Text value</span></span>

<span data-ttu-id="28023-122">**BodyType**要素の有効な値を次の表に一覧します。</span><span class="sxs-lookup"><span data-stu-id="28023-122">The following table lists the possible values for the **BodyType** element.</span></span> 
  
|<span data-ttu-id="28023-123">**値**</span><span class="sxs-lookup"><span data-stu-id="28023-123">**Value**</span></span>|<span data-ttu-id="28023-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="28023-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="28023-125">ベスト</span><span class="sxs-lookup"><span data-stu-id="28023-125">Best</span></span>  <br/> |<span data-ttu-id="28023-126">応答には、本文テキストの豊富な利用可能なコンテンツが返されます。</span><span class="sxs-lookup"><span data-stu-id="28023-126">The response will return the richest available content of body text.</span></span> <span data-ttu-id="28023-127">これは、コンテンツは、テキストまたは html 形式かどうか不明ではない場合に便利です。</span><span class="sxs-lookup"><span data-stu-id="28023-127">This is useful if it is unknown whether the content is text or HTML.</span></span><br/><br/> <span data-ttu-id="28023-128">ストアド本文がテキスト形式の場合は、返された本文をテキストになります。</span><span class="sxs-lookup"><span data-stu-id="28023-128">The returned body will be text if the stored body is plain text.</span></span> <span data-ttu-id="28023-129">それ以外の場合、応答であっても、ストアドの本文が HTML または rtf 形式のいずれかの形式では場合、HTML が返されます。</span><span class="sxs-lookup"><span data-stu-id="28023-129">Otherwise, the response will return HTML if the stored body is in either HTML or RTF format.</span></span><br/><br/> <span data-ttu-id="28023-130">既定値です。</span><span class="sxs-lookup"><span data-stu-id="28023-130">This is the default value.</span></span>  <br/> |
|<span data-ttu-id="28023-131">HTML</span><span class="sxs-lookup"><span data-stu-id="28023-131">HTML</span></span>  <br/> |<span data-ttu-id="28023-132">応答では、アイテムの本文を HTML として返します。</span><span class="sxs-lookup"><span data-stu-id="28023-132">The response will return an item body as HTML.</span></span>  <br/> |
|<span data-ttu-id="28023-133">テキスト型 (Text)</span><span class="sxs-lookup"><span data-stu-id="28023-133">Text</span></span>  <br/> |<span data-ttu-id="28023-134">応答では、アイテムの本文をプレーン テキストとして返します。</span><span class="sxs-lookup"><span data-stu-id="28023-134">The response will return an item body as plain text.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="28023-135">備考</span><span class="sxs-lookup"><span data-stu-id="28023-135">Remarks</span></span>

<span data-ttu-id="28023-136">[Body](body.md)要素の**BodyType**属性を確認することによって応答で返される本文の種類を識別することができます。</span><span class="sxs-lookup"><span data-stu-id="28023-136">You can identify the type of body returned in the response by checking the **BodyType** attribute of the [Body](body.md) element.</span></span> <span data-ttu-id="28023-137">**BodyType**属性は、HTML またはテキストのいずれかとして本体を識別します。</span><span class="sxs-lookup"><span data-stu-id="28023-137">The **BodyType** attribute will identify the body as either HTML or text.</span></span> 
  
<span data-ttu-id="28023-138">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="28023-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="28023-139">例</span><span class="sxs-lookup"><span data-stu-id="28023-139">Example</span></span>

<span data-ttu-id="28023-140">**BodyType**要素が使用されている要求の次の使用例を示しています。</span><span class="sxs-lookup"><span data-stu-id="28023-140">The following example of a request shows where a **BodyType** element is used.</span></span> 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="28023-141">Id 属性が読みやすさを維持するのには小さすぎます。</span><span class="sxs-lookup"><span data-stu-id="28023-141">The Id attribute has been shortened to preserve readability.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="28023-142">要素情報</span><span class="sxs-lookup"><span data-stu-id="28023-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="28023-143">名前空間</span><span class="sxs-lookup"><span data-stu-id="28023-143">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="28023-144">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="28023-144">Schema Name</span></span>  <br/> |<span data-ttu-id="28023-145">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="28023-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="28023-146">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="28023-146">Validation File</span></span>  <br/> |<span data-ttu-id="28023-147">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="28023-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="28023-148">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="28023-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="28023-149">いいえ</span><span class="sxs-lookup"><span data-stu-id="28023-149">False</span></span>  <br/> |
   

