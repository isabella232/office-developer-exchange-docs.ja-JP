---
title: CreateAttachmentResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateAttachmentResponse
api_type:
- schema
ms.assetid: cf6bd8bb-5317-4a03-bd75-297dd359b5da
description: CreateAttachmentResponse 要素は、CreateAttachment 要求に対する応答を定義します。
ms.openlocfilehash: df2b0e37adaeaef32f845e5a28615ce874cb3447
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466417"
---
# <a name="createattachmentresponse"></a><span data-ttu-id="2ca81-103">CreateAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="2ca81-103">CreateAttachmentResponse</span></span>

<span data-ttu-id="2ca81-104">**Createattachmentresponse**要素は、createattachment 要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="2ca81-104">The **CreateAttachmentResponse** element defines a response to a CreateAttachment request.</span></span> 
  
```xml
<CreateAttachmentResponse>
   <ResponseMessages/>
</CreateAttachmentResponse>
```

 <span data-ttu-id="2ca81-105">**CreateAttachmentResponseType**</span><span class="sxs-lookup"><span data-stu-id="2ca81-105">**CreateAttachmentResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2ca81-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="2ca81-106">Attributes and elements</span></span>

<span data-ttu-id="2ca81-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2ca81-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2ca81-108">属性</span><span class="sxs-lookup"><span data-stu-id="2ca81-108">Attributes</span></span>

<span data-ttu-id="2ca81-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2ca81-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2ca81-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2ca81-110">Child elements</span></span>

|<span data-ttu-id="2ca81-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="2ca81-111">**Element**</span></span>|<span data-ttu-id="2ca81-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="2ca81-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2ca81-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="2ca81-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="2ca81-114">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="2ca81-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2ca81-115">親要素</span><span class="sxs-lookup"><span data-stu-id="2ca81-115">Parent elements</span></span>

<span data-ttu-id="2ca81-116">なし。</span><span class="sxs-lookup"><span data-stu-id="2ca81-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2ca81-117">注釈</span><span class="sxs-lookup"><span data-stu-id="2ca81-117">Remarks</span></span>

<span data-ttu-id="2ca81-118">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="2ca81-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2ca81-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="2ca81-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2ca81-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="2ca81-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2ca81-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2ca81-121">Schema name</span></span>  <br/> |<span data-ttu-id="2ca81-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="2ca81-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2ca81-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2ca81-123">Validation file</span></span>  <br/> |<span data-ttu-id="2ca81-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="2ca81-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2ca81-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2ca81-125">Can be empty</span></span>  <br/> |<span data-ttu-id="2ca81-126">正しくない</span><span class="sxs-lookup"><span data-stu-id="2ca81-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2ca81-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="2ca81-127">See also</span></span>



[<span data-ttu-id="2ca81-128">CreateAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="2ca81-128">CreateAttachment operation</span></span>](createattachment-operation.md)
  
[<span data-ttu-id="2ca81-129">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="2ca81-129">CreateAttachment</span></span>](createattachment.md)


- [<span data-ttu-id="2ca81-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="2ca81-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

