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
description: GetAttachment 要素は、Exchange ストアからの添付ファイルを取得する要求のルート要素です。
ms.openlocfilehash: fb639c86a0654e8f9e9601310f7c2f5b0fc7d729
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760640"
---
# <a name="getattachment"></a><span data-ttu-id="b732b-103">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="b732b-103">GetAttachment</span></span>

<span data-ttu-id="b732b-104">**GetAttachment**要素は、Exchange ストアからの添付ファイルを取得する要求のルート要素です。</span><span class="sxs-lookup"><span data-stu-id="b732b-104">The **GetAttachment** element is the root element in a request to get an attachment from the Exchange store.</span></span> 
  
```xml
<GetAttachment>
   <AttachmentShape/>
   <AttachmentIds/>
</GetAttachment>
```

 <span data-ttu-id="b732b-105">**GetAttachmentType**</span><span class="sxs-lookup"><span data-stu-id="b732b-105">**GetAttachmentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b732b-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b732b-106">Attributes and elements</span></span>

<span data-ttu-id="b732b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b732b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b732b-108">属性</span><span class="sxs-lookup"><span data-stu-id="b732b-108">Attributes</span></span>

<span data-ttu-id="b732b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b732b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b732b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b732b-110">Child elements</span></span>

|<span data-ttu-id="b732b-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="b732b-111">**Element**</span></span>|<span data-ttu-id="b732b-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="b732b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b732b-113">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="b732b-113">AttachmentShape</span></span>](attachmentshape.md) <br/> |<span data-ttu-id="b732b-114">[GetAttachment](getattachment.md)要求への応答で返されるその他の拡張アイテム プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="b732b-114">Identifies additional extended item properties to return in a response to a [GetAttachment](getattachment.md) request.</span></span> <span data-ttu-id="b732b-115">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="b732b-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="b732b-116">AttachmentIds</span><span class="sxs-lookup"><span data-stu-id="b732b-116">AttachmentIds</span></span>](attachmentids.md) <br/> |<span data-ttu-id="b732b-117">添付ファイル識別子の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b732b-117">Contains an array of attachment identifiers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b732b-118">親要素</span><span class="sxs-lookup"><span data-stu-id="b732b-118">Parent elements</span></span>

<span data-ttu-id="b732b-119">なし。</span><span class="sxs-lookup"><span data-stu-id="b732b-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b732b-120">備考</span><span class="sxs-lookup"><span data-stu-id="b732b-120">Remarks</span></span>

<span data-ttu-id="b732b-121">[AttachmentShape](attachmentshape.md)要素は、応答で返されるプロパティを識別するために必要ではありません。</span><span class="sxs-lookup"><span data-stu-id="b732b-121">The [AttachmentShape](attachmentshape.md) element is not required to identify the properties returned in the response.</span></span> <span data-ttu-id="b732b-122">[GetAttachment 操作](getattachment-operation.md)には、名前、コンテンツ タイプ、ContentId、ContentLocation、および添付ファイルのコンテンツのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b732b-122">The [GetAttachment operation](getattachment-operation.md) returns the Name, ContentType, ContentId, ContentLocation, and the Content properties for file attachments.</span></span> <span data-ttu-id="b732b-123">項目の添付ファイルは、返されるプロパティは、名前、コンテンツ タイプ、ContentId、ContentLocation、およびすべての接続されているアイテムのプロパティです。</span><span class="sxs-lookup"><span data-stu-id="b732b-123">For item attachments, the returned properties are the Name, ContentType, ContentId, ContentLocation, and all the attached item's properties.</span></span> <span data-ttu-id="b732b-124">これは、 [GetItem](getitem.md)要求で AllProperties の基本図形を使用するのと同じです。</span><span class="sxs-lookup"><span data-stu-id="b732b-124">This is equivalent to using the AllProperties base shape in a [GetItem](getitem.md) request.</span></span> 
  
<span data-ttu-id="b732b-125">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="b732b-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b732b-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="b732b-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b732b-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="b732b-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b732b-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b732b-128">Schema Name</span></span>  <br/> |<span data-ttu-id="b732b-129">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="b732b-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b732b-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b732b-130">Validation File</span></span>  <br/> |<span data-ttu-id="b732b-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b732b-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b732b-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b732b-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="b732b-133">False</span><span class="sxs-lookup"><span data-stu-id="b732b-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b732b-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="b732b-134">See also</span></span>



[<span data-ttu-id="b732b-135">GetAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="b732b-135">GetAttachment operation</span></span>](getattachment-operation.md)
  
[<span data-ttu-id="b732b-136">GetAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="b732b-136">GetAttachmentResponse</span></span>](getattachmentresponse.md)

