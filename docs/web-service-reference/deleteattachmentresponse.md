---
title: DeleteAttachmentResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteAttachmentResponse
api_type:
- schema
ms.assetid: 24099a88-4ab6-4bf3-8ed5-efec8e07b9b9
description: DeleteAttachmentResponse は、DeleteAttachment 要求への応答を定義します。
ms.openlocfilehash: f1a6b0ebba7257d02ceeea024486dc002d299dff
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759961"
---
# <a name="deleteattachmentresponse"></a><span data-ttu-id="36b03-103">DeleteAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="36b03-103">DeleteAttachmentResponse</span></span>

<span data-ttu-id="36b03-104">**DeleteAttachmentResponse**は、DeleteAttachment 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="36b03-104">The **DeleteAttachmentResponse** defines a response to a DeleteAttachment request.</span></span> 
  
```xml
<DeleteAttachmentResponse>
   <ResponseMessages/>
</DeleteAttachmentResponse>
```

<span data-ttu-id="36b03-105">**DeleteAttachmentResponseType**</span><span class="sxs-lookup"><span data-stu-id="36b03-105">**DeleteAttachmentResponseType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="36b03-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="36b03-106">Attributes and elements</span></span>

<span data-ttu-id="36b03-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="36b03-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="36b03-108">属性</span><span class="sxs-lookup"><span data-stu-id="36b03-108">Attributes</span></span>

<span data-ttu-id="36b03-109">なし。</span><span class="sxs-lookup"><span data-stu-id="36b03-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="36b03-110">子要素</span><span class="sxs-lookup"><span data-stu-id="36b03-110">Child elements</span></span>

|<span data-ttu-id="36b03-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="36b03-111">**Element**</span></span>|<span data-ttu-id="36b03-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="36b03-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="36b03-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="36b03-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="36b03-114">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="36b03-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="36b03-115">親要素</span><span class="sxs-lookup"><span data-stu-id="36b03-115">Parent elements</span></span>

<span data-ttu-id="36b03-116">なし。</span><span class="sxs-lookup"><span data-stu-id="36b03-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="36b03-117">備考</span><span class="sxs-lookup"><span data-stu-id="36b03-117">Remarks</span></span>

<span data-ttu-id="36b03-118">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="36b03-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="36b03-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="36b03-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="36b03-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="36b03-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="36b03-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="36b03-121">Schema name</span></span>  <br/> |<span data-ttu-id="36b03-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="36b03-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="36b03-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="36b03-123">Validation file</span></span>  <br/> |<span data-ttu-id="36b03-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="36b03-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="36b03-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="36b03-125">Can be empty</span></span>  <br/> |<span data-ttu-id="36b03-126">False</span><span class="sxs-lookup"><span data-stu-id="36b03-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="36b03-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="36b03-127">See also</span></span>

- [<span data-ttu-id="36b03-128">DeleteAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="36b03-128">DeleteAttachment operation</span></span>](deleteattachment-operation.md)  
- [<span data-ttu-id="36b03-129">DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="36b03-129">DeleteAttachment</span></span>](deleteattachment.md)
- [<span data-ttu-id="36b03-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="36b03-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

