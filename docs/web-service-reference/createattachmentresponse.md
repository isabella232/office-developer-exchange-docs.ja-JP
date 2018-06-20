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
description: CreateAttachmentResponse 要素は、CreateAttachment 要求への応答を定義します。
ms.openlocfilehash: dfc86516c5737296bc32330583fa63c36e9e63a3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759798"
---
# <a name="createattachmentresponse"></a><span data-ttu-id="1047a-103">CreateAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="1047a-103">CreateAttachmentResponse</span></span>

<span data-ttu-id="1047a-104">**CreateAttachmentResponse**要素は、CreateAttachment 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="1047a-104">The **CreateAttachmentResponse** element defines a response to a CreateAttachment request.</span></span> 
  
```xml
<CreateAttachmentResponse>
   <ResponseMessages/>
</CreateAttachmentResponse>
```

 <span data-ttu-id="1047a-105">**CreateAttachmentResponseType**</span><span class="sxs-lookup"><span data-stu-id="1047a-105">**CreateAttachmentResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1047a-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="1047a-106">Attributes and elements</span></span>

<span data-ttu-id="1047a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1047a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1047a-108">属性</span><span class="sxs-lookup"><span data-stu-id="1047a-108">Attributes</span></span>

<span data-ttu-id="1047a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1047a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1047a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1047a-110">Child elements</span></span>

|<span data-ttu-id="1047a-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="1047a-111">**Element**</span></span>|<span data-ttu-id="1047a-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="1047a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1047a-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="1047a-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="1047a-114">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="1047a-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1047a-115">親要素</span><span class="sxs-lookup"><span data-stu-id="1047a-115">Parent elements</span></span>

<span data-ttu-id="1047a-116">なし。</span><span class="sxs-lookup"><span data-stu-id="1047a-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1047a-117">備考</span><span class="sxs-lookup"><span data-stu-id="1047a-117">Remarks</span></span>

<span data-ttu-id="1047a-118">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="1047a-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1047a-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="1047a-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1047a-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="1047a-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1047a-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1047a-121">Schema name</span></span>  <br/> |<span data-ttu-id="1047a-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="1047a-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1047a-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1047a-123">Validation file</span></span>  <br/> |<span data-ttu-id="1047a-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1047a-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1047a-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="1047a-125">Can be empty</span></span>  <br/> |<span data-ttu-id="1047a-126">False</span><span class="sxs-lookup"><span data-stu-id="1047a-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1047a-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="1047a-127">See also</span></span>



[<span data-ttu-id="1047a-128">CreateAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="1047a-128">CreateAttachment operation</span></span>](createattachment-operation.md)
  
[<span data-ttu-id="1047a-129">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="1047a-129">CreateAttachment</span></span>](createattachment.md)


- [<span data-ttu-id="1047a-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="1047a-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

