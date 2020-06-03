---
title: GetAttachmentResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetAttachmentResponse
api_type:
- schema
ms.assetid: cb65f449-309b-4b6e-8d22-d1967135490c
description: GetAttachmentResponse 要素は、GetAttachment 要求に対する応答を定義します。
ms.openlocfilehash: f0daf778f1248eabc5d51ee6155c460d9248549f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461255"
---
# <a name="getattachmentresponse"></a><span data-ttu-id="b55f5-103">GetAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="b55f5-103">GetAttachmentResponse</span></span>

<span data-ttu-id="b55f5-104">**Getattachmentresponse**要素は、getattachment 要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="b55f5-104">The **GetAttachmentResponse** element defines a response to a GetAttachment request.</span></span> 
  
```xml
<GetAttachmentResponse>
   <ResponseMessages/>
</GetAttachmentResponse>
```

 <span data-ttu-id="b55f5-105">**GetAttachmentResponseType**</span><span class="sxs-lookup"><span data-stu-id="b55f5-105">**GetAttachmentResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b55f5-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b55f5-106">Attributes and elements</span></span>

<span data-ttu-id="b55f5-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b55f5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b55f5-108">属性</span><span class="sxs-lookup"><span data-stu-id="b55f5-108">Attributes</span></span>

<span data-ttu-id="b55f5-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b55f5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b55f5-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b55f5-110">Child elements</span></span>

|<span data-ttu-id="b55f5-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="b55f5-111">**Element**</span></span>|<span data-ttu-id="b55f5-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="b55f5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b55f5-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b55f5-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="b55f5-114">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="b55f5-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b55f5-115">親要素</span><span class="sxs-lookup"><span data-stu-id="b55f5-115">Parent elements</span></span>

<span data-ttu-id="b55f5-116">なし。</span><span class="sxs-lookup"><span data-stu-id="b55f5-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b55f5-117">注釈</span><span class="sxs-lookup"><span data-stu-id="b55f5-117">Remarks</span></span>

<span data-ttu-id="b55f5-118">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="b55f5-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b55f5-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b55f5-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b55f5-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="b55f5-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b55f5-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b55f5-121">Schema name</span></span>  <br/> |<span data-ttu-id="b55f5-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="b55f5-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b55f5-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b55f5-123">Validation file</span></span>  <br/> |<span data-ttu-id="b55f5-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="b55f5-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b55f5-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b55f5-125">Can be empty</span></span>  <br/> |<span data-ttu-id="b55f5-126">正しくない</span><span class="sxs-lookup"><span data-stu-id="b55f5-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b55f5-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="b55f5-127">See also</span></span>



[<span data-ttu-id="b55f5-128">GetAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="b55f5-128">GetAttachment operation</span></span>](getattachment-operation.md)
  
[<span data-ttu-id="b55f5-129">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="b55f5-129">GetAttachment</span></span>](getattachment.md)

