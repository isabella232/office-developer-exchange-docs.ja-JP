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
description: AttachmentShape 要素は、GetAttachment 要求への応答で返される追加のプロパティを識別します。
ms.openlocfilehash: dc6769faa5fd28ce31b796f86c507aec54abff7a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759455"
---
# <a name="attachmentshape"></a><span data-ttu-id="ac9c5-103">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="ac9c5-103">AttachmentShape</span></span>

<span data-ttu-id="ac9c5-104">**AttachmentShape**要素は、 [GetAttachment](getattachment.md)要求への応答で返される追加のプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="ac9c5-104">The **AttachmentShape** element identifies additional properties to return in a response to a [GetAttachment](getattachment.md) request.</span></span> 
  
- [<span data-ttu-id="ac9c5-105">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="ac9c5-105">GetAttachment</span></span>](getattachment.md)
  
- [<span data-ttu-id="ac9c5-106">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="ac9c5-106">AttachmentShape</span></span>](attachmentshape.md)
  
```xml
<AttachmentShape>
   <IncludeMimeContent/>
   <BodyType/>
   <FilterHtmlContent/>
   <AdditionalProperties/>
</AttachmentShape>
```

 <span data-ttu-id="ac9c5-107">**AttachmentResponseShapeType**</span><span class="sxs-lookup"><span data-stu-id="ac9c5-107">**AttachmentResponseShapeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ac9c5-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ac9c5-108">Attributes and elements</span></span>

<span data-ttu-id="ac9c5-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ac9c5-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ac9c5-110">属性</span><span class="sxs-lookup"><span data-stu-id="ac9c5-110">Attributes</span></span>

<span data-ttu-id="ac9c5-111">なし。</span><span class="sxs-lookup"><span data-stu-id="ac9c5-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ac9c5-112">子要素</span><span class="sxs-lookup"><span data-stu-id="ac9c5-112">Child elements</span></span>

|<span data-ttu-id="ac9c5-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="ac9c5-113">**Element**</span></span>|<span data-ttu-id="ac9c5-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="ac9c5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ac9c5-115">IncludeMimeContent</span><span class="sxs-lookup"><span data-stu-id="ac9c5-115">IncludeMimeContent</span></span>](includemimecontent.md) <br/> |<span data-ttu-id="ac9c5-116">応答で、多目的インターネット メール拡張 (MIME) のコンテンツ アイテムまたは添付ファイルが返されるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="ac9c5-116">Specifies whether the Multipurpose Internet Mail Extensions (MIME) content of an item or attachment is returned in the response.</span></span> <span data-ttu-id="ac9c5-117">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="ac9c5-117">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="ac9c5-118">BodyType</span><span class="sxs-lookup"><span data-stu-id="ac9c5-118">BodyType</span></span>](bodytype.md) <br/> |<span data-ttu-id="ac9c5-119">応答の本文のテキストを書式設定する方法を識別します。</span><span class="sxs-lookup"><span data-stu-id="ac9c5-119">Identifies how the body text is formatted in the response.</span></span> <span data-ttu-id="ac9c5-120">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="ac9c5-120">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="ac9c5-121">FilterHtmlContent</span><span class="sxs-lookup"><span data-stu-id="ac9c5-121">FilterHtmlContent</span></span>](filterhtmlcontent.md) <br/> |<span data-ttu-id="ac9c5-122">添付ファイルから安全でない HTML コンテンツがフィルター処理されたかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="ac9c5-122">Specifies whether potentially unsafe HTML content is filtered from an attachment.</span></span> <span data-ttu-id="ac9c5-123">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="ac9c5-123">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="ac9c5-124">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="ac9c5-124">AdditionalProperties</span></span>](additionalproperties.md) <br/> |<span data-ttu-id="ac9c5-125">応答で返される追加プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="ac9c5-125">Identifies additional properties to return in a response.</span></span> <span data-ttu-id="ac9c5-126">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="ac9c5-126">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ac9c5-127">親要素</span><span class="sxs-lookup"><span data-stu-id="ac9c5-127">Parent elements</span></span>

|<span data-ttu-id="ac9c5-128">**要素**</span><span class="sxs-lookup"><span data-stu-id="ac9c5-128">**Element**</span></span>|<span data-ttu-id="ac9c5-129">**説明**</span><span class="sxs-lookup"><span data-stu-id="ac9c5-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ac9c5-130">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="ac9c5-130">GetAttachment</span></span>](getattachment.md) <br/> |<span data-ttu-id="ac9c5-131">Exchange ストア内のメールボックスから添付ファイルを取得する要求を定義する要素。</span><span class="sxs-lookup"><span data-stu-id="ac9c5-131">The element that defines a request to get an attachment from a mailbox in the Exchange store.</span></span>  <br/> <span data-ttu-id="ac9c5-132">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="ac9c5-132">The following is the XPath expression to this element:</span></span>  <br/>  `/GetAttachment` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ac9c5-133">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ac9c5-133">Text value</span></span>

<span data-ttu-id="ac9c5-134">なし。</span><span class="sxs-lookup"><span data-stu-id="ac9c5-134">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ac9c5-135">備考</span><span class="sxs-lookup"><span data-stu-id="ac9c5-135">Remarks</span></span>

<span data-ttu-id="ac9c5-136">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ac9c5-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ac9c5-137">要素情報</span><span class="sxs-lookup"><span data-stu-id="ac9c5-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ac9c5-138">名前空間</span><span class="sxs-lookup"><span data-stu-id="ac9c5-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ac9c5-139">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ac9c5-139">Schema Name</span></span>  <br/> |<span data-ttu-id="ac9c5-140">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="ac9c5-140">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ac9c5-141">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ac9c5-141">Validation File</span></span>  <br/> |<span data-ttu-id="ac9c5-142">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ac9c5-142">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ac9c5-143">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ac9c5-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="ac9c5-144">False</span><span class="sxs-lookup"><span data-stu-id="ac9c5-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ac9c5-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="ac9c5-145">See also</span></span>

- [<span data-ttu-id="ac9c5-146">GetAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="ac9c5-146">GetAttachment operation</span></span>](getattachment-operation.md)
- [<span data-ttu-id="ac9c5-147">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="ac9c5-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

