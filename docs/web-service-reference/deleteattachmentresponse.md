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
description: DeleteAttachmentResponse は、DeleteAttachment 要求に対する応答を定義します。
ms.openlocfilehash: 352318ef54687b0d1d4ce73b075248b79238d555
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457327"
---
# <a name="deleteattachmentresponse"></a><span data-ttu-id="5d867-103">DeleteAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="5d867-103">DeleteAttachmentResponse</span></span>

<span data-ttu-id="5d867-104">**Deleteattachmentresponse**は、deleteattachment 要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="5d867-104">The **DeleteAttachmentResponse** defines a response to a DeleteAttachment request.</span></span> 
  
```xml
<DeleteAttachmentResponse>
   <ResponseMessages/>
</DeleteAttachmentResponse>
```

<span data-ttu-id="5d867-105">**DeleteAttachmentResponseType**</span><span class="sxs-lookup"><span data-stu-id="5d867-105">**DeleteAttachmentResponseType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="5d867-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="5d867-106">Attributes and elements</span></span>

<span data-ttu-id="5d867-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5d867-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5d867-108">属性</span><span class="sxs-lookup"><span data-stu-id="5d867-108">Attributes</span></span>

<span data-ttu-id="5d867-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5d867-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5d867-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5d867-110">Child elements</span></span>

|<span data-ttu-id="5d867-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="5d867-111">**Element**</span></span>|<span data-ttu-id="5d867-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="5d867-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5d867-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5d867-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="5d867-114">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="5d867-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5d867-115">親要素</span><span class="sxs-lookup"><span data-stu-id="5d867-115">Parent elements</span></span>

<span data-ttu-id="5d867-116">なし。</span><span class="sxs-lookup"><span data-stu-id="5d867-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5d867-117">注釈</span><span class="sxs-lookup"><span data-stu-id="5d867-117">Remarks</span></span>

<span data-ttu-id="5d867-118">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="5d867-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5d867-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="5d867-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5d867-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="5d867-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5d867-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5d867-121">Schema name</span></span>  <br/> |<span data-ttu-id="5d867-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="5d867-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5d867-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5d867-123">Validation file</span></span>  <br/> |<span data-ttu-id="5d867-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="5d867-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5d867-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="5d867-125">Can be empty</span></span>  <br/> |<span data-ttu-id="5d867-126">正しくない</span><span class="sxs-lookup"><span data-stu-id="5d867-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5d867-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="5d867-127">See also</span></span>

- [<span data-ttu-id="5d867-128">DeleteAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="5d867-128">DeleteAttachment operation</span></span>](deleteattachment-operation.md)  
- [<span data-ttu-id="5d867-129">DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="5d867-129">DeleteAttachment</span></span>](deleteattachment.md)
- [<span data-ttu-id="5d867-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="5d867-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

