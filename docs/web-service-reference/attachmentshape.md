---
title: AttachmentShape
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttachmentShape
api_type:
- schema
ms.assetid: 734914b5-3a16-4744-90a5-741fd30c4676
description: AttachmentShape 要素は、GetAttachment 要求に対する応答で返される追加のプロパティを識別します。
ms.openlocfilehash: e70fbaad0f649c5afdc151b777efef0f8927ba1c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529666"
---
# <a name="attachmentshape"></a><span data-ttu-id="9fd9e-103">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="9fd9e-103">AttachmentShape</span></span>

<span data-ttu-id="9fd9e-104">**Attachmentshape**要素は、 [getattachment](getattachment.md)要求に対する応答で返される追加のプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="9fd9e-104">The **AttachmentShape** element identifies additional properties to return in a response to a [GetAttachment](getattachment.md) request.</span></span> 
  
- [<span data-ttu-id="9fd9e-105">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="9fd9e-105">GetAttachment</span></span>](getattachment.md)
  
- [<span data-ttu-id="9fd9e-106">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="9fd9e-106">AttachmentShape</span></span>](attachmentshape.md)
  
```xml
<AttachmentShape>
   <IncludeMimeContent/>
   <BodyType/>
   <FilterHtmlContent/>
   <AdditionalProperties/>
</AttachmentShape>
```

 <span data-ttu-id="9fd9e-107">**AttachmentResponseShapeType**</span><span class="sxs-lookup"><span data-stu-id="9fd9e-107">**AttachmentResponseShapeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9fd9e-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9fd9e-108">Attributes and elements</span></span>

<span data-ttu-id="9fd9e-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9fd9e-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9fd9e-110">属性</span><span class="sxs-lookup"><span data-stu-id="9fd9e-110">Attributes</span></span>

<span data-ttu-id="9fd9e-111">なし。</span><span class="sxs-lookup"><span data-stu-id="9fd9e-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9fd9e-112">子要素</span><span class="sxs-lookup"><span data-stu-id="9fd9e-112">Child elements</span></span>

|<span data-ttu-id="9fd9e-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="9fd9e-113">**Element**</span></span>|<span data-ttu-id="9fd9e-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="9fd9e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9fd9e-115">IncludeMimeContent</span><span class="sxs-lookup"><span data-stu-id="9fd9e-115">IncludeMimeContent</span></span>](includemimecontent.md) <br/> |<span data-ttu-id="9fd9e-116">アイテムまたは添付ファイルのマルチパーパスインターネットメール内線 (MIME) コンテンツを応答で返すかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="9fd9e-116">Specifies whether the Multipurpose Internet Mail Extensions (MIME) content of an item or attachment is returned in the response.</span></span> <span data-ttu-id="9fd9e-117">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="9fd9e-117">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="9fd9e-118">BodyType</span><span class="sxs-lookup"><span data-stu-id="9fd9e-118">BodyType</span></span>](bodytype.md) <br/> |<span data-ttu-id="9fd9e-119">応答で本文テキストを書式設定する方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="9fd9e-119">Identifies how the body text is formatted in the response.</span></span> <span data-ttu-id="9fd9e-120">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="9fd9e-120">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="9fd9e-121">FilterHtmlContent</span><span class="sxs-lookup"><span data-stu-id="9fd9e-121">FilterHtmlContent</span></span>](filterhtmlcontent.md) <br/> |<span data-ttu-id="9fd9e-122">安全でない可能性のある HTML コンテンツを添付ファイルからフィルター処理するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="9fd9e-122">Specifies whether potentially unsafe HTML content is filtered from an attachment.</span></span> <span data-ttu-id="9fd9e-123">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="9fd9e-123">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="9fd9e-124">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="9fd9e-124">AdditionalProperties</span></span>](additionalproperties.md) <br/> |<span data-ttu-id="9fd9e-125">応答で返される追加のプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="9fd9e-125">Identifies additional properties to return in a response.</span></span> <span data-ttu-id="9fd9e-126">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="9fd9e-126">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9fd9e-127">親要素</span><span class="sxs-lookup"><span data-stu-id="9fd9e-127">Parent elements</span></span>

|<span data-ttu-id="9fd9e-128">**要素**</span><span class="sxs-lookup"><span data-stu-id="9fd9e-128">**Element**</span></span>|<span data-ttu-id="9fd9e-129">**説明**</span><span class="sxs-lookup"><span data-stu-id="9fd9e-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9fd9e-130">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="9fd9e-130">GetAttachment</span></span>](getattachment.md) <br/> |<span data-ttu-id="9fd9e-131">Exchange ストア内のメールボックスから添付ファイルを取得するための要求を定義する要素。</span><span class="sxs-lookup"><span data-stu-id="9fd9e-131">The element that defines a request to get an attachment from a mailbox in the Exchange store.</span></span>  <br/> <span data-ttu-id="9fd9e-132">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9fd9e-132">The following is the XPath expression to this element:</span></span>  <br/>  `/GetAttachment` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9fd9e-133">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9fd9e-133">Text value</span></span>

<span data-ttu-id="9fd9e-134">なし。</span><span class="sxs-lookup"><span data-stu-id="9fd9e-134">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9fd9e-135">注釈</span><span class="sxs-lookup"><span data-stu-id="9fd9e-135">Remarks</span></span>

<span data-ttu-id="9fd9e-136">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9fd9e-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9fd9e-137">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9fd9e-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9fd9e-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="9fd9e-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9fd9e-139">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9fd9e-139">Schema Name</span></span>  <br/> |<span data-ttu-id="9fd9e-140">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="9fd9e-140">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9fd9e-141">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9fd9e-141">Validation File</span></span>  <br/> |<span data-ttu-id="9fd9e-142">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="9fd9e-142">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9fd9e-143">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9fd9e-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="9fd9e-144">正しくない</span><span class="sxs-lookup"><span data-stu-id="9fd9e-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9fd9e-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="9fd9e-145">See also</span></span>

- [<span data-ttu-id="9fd9e-146">GetAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="9fd9e-146">GetAttachment operation</span></span>](getattachment-operation.md)
- [<span data-ttu-id="9fd9e-147">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="9fd9e-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

