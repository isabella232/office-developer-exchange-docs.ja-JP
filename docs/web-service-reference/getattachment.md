---
title: GetAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetAttachment
api_type:
- schema
ms.assetid: 9443cf96-b451-4530-b868-490dff798673
description: GetAttachment 要素は、Exchange ストアから添付ファイルを取得する要求のルート要素です。
ms.openlocfilehash: d03d086ff443db87b0104a2ec83599eb9eaea6b9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463980"
---
# <a name="getattachment"></a><span data-ttu-id="21482-103">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="21482-103">GetAttachment</span></span>

<span data-ttu-id="21482-104">**Getattachment**要素は、Exchange ストアから添付ファイルを取得する要求のルート要素です。</span><span class="sxs-lookup"><span data-stu-id="21482-104">The **GetAttachment** element is the root element in a request to get an attachment from the Exchange store.</span></span> 
  
```xml
<GetAttachment>
   <AttachmentShape/>
   <AttachmentIds/>
</GetAttachment>
```

 <span data-ttu-id="21482-105">**GetAttachmentType**</span><span class="sxs-lookup"><span data-stu-id="21482-105">**GetAttachmentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="21482-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="21482-106">Attributes and elements</span></span>

<span data-ttu-id="21482-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="21482-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="21482-108">属性</span><span class="sxs-lookup"><span data-stu-id="21482-108">Attributes</span></span>

<span data-ttu-id="21482-109">なし。</span><span class="sxs-lookup"><span data-stu-id="21482-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="21482-110">子要素</span><span class="sxs-lookup"><span data-stu-id="21482-110">Child elements</span></span>

|<span data-ttu-id="21482-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="21482-111">**Element**</span></span>|<span data-ttu-id="21482-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="21482-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="21482-113">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="21482-113">AttachmentShape</span></span>](attachmentshape.md) <br/> |<span data-ttu-id="21482-114">[Getattachment](getattachment.md)要求に対する応答で返される追加の拡張アイテムプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="21482-114">Identifies additional extended item properties to return in a response to a [GetAttachment](getattachment.md) request.</span></span> <span data-ttu-id="21482-115">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="21482-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="21482-116">AttachmentIds</span><span class="sxs-lookup"><span data-stu-id="21482-116">AttachmentIds</span></span>](attachmentids.md) <br/> |<span data-ttu-id="21482-117">添付ファイル識別子の配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="21482-117">Contains an array of attachment identifiers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="21482-118">親要素</span><span class="sxs-lookup"><span data-stu-id="21482-118">Parent elements</span></span>

<span data-ttu-id="21482-119">なし。</span><span class="sxs-lookup"><span data-stu-id="21482-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="21482-120">注釈</span><span class="sxs-lookup"><span data-stu-id="21482-120">Remarks</span></span>

<span data-ttu-id="21482-121">[Attachmentshape](attachmentshape.md)要素は、応答で返されるプロパティを識別するために必須ではありません。</span><span class="sxs-lookup"><span data-stu-id="21482-121">The [AttachmentShape](attachmentshape.md) element is not required to identify the properties returned in the response.</span></span> <span data-ttu-id="21482-122">[Getattachment 操作](getattachment-operation.md)は、Name、ContentType、ContentId、contentlocation、および添付ファイルのコンテンツプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="21482-122">The [GetAttachment operation](getattachment-operation.md) returns the Name, ContentType, ContentId, ContentLocation, and the Content properties for file attachments.</span></span> <span data-ttu-id="21482-123">アイテムの添付ファイルの場合、返されるプロパティは、Name、ContentType、ContentId、ContentLocation、および添付されているすべてのアイテムのプロパティです。</span><span class="sxs-lookup"><span data-stu-id="21482-123">For item attachments, the returned properties are the Name, ContentType, ContentId, ContentLocation, and all the attached item's properties.</span></span> <span data-ttu-id="21482-124">これは、 [GetItem](getitem.md)要求で allproperties 基本図形を使用するのと同じです。</span><span class="sxs-lookup"><span data-stu-id="21482-124">This is equivalent to using the AllProperties base shape in a [GetItem](getitem.md) request.</span></span> 
  
<span data-ttu-id="21482-125">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="21482-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="21482-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="21482-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="21482-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="21482-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="21482-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="21482-128">Schema Name</span></span>  <br/> |<span data-ttu-id="21482-129">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="21482-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="21482-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="21482-130">Validation File</span></span>  <br/> |<span data-ttu-id="21482-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="21482-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="21482-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="21482-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="21482-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="21482-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="21482-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="21482-134">See also</span></span>



[<span data-ttu-id="21482-135">GetAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="21482-135">GetAttachment operation</span></span>](getattachment-operation.md)
  
[<span data-ttu-id="21482-136">GetAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="21482-136">GetAttachmentResponse</span></span>](getattachmentresponse.md)

