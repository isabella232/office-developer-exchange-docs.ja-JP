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
description: GetAttachmentResponse 要素は、GetAttachment 要求への応答を定義します。
ms.openlocfilehash: 05a9e84236c791dcec99182dfca0352e44efca46
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760642"
---
# <a name="getattachmentresponse"></a><span data-ttu-id="a073a-103">GetAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="a073a-103">GetAttachmentResponse</span></span>

<span data-ttu-id="a073a-104">**GetAttachmentResponse**要素は、GetAttachment 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="a073a-104">The **GetAttachmentResponse** element defines a response to a GetAttachment request.</span></span> 
  
```xml
<GetAttachmentResponse>
   <ResponseMessages/>
</GetAttachmentResponse>
```

 <span data-ttu-id="a073a-105">**GetAttachmentResponseType**</span><span class="sxs-lookup"><span data-stu-id="a073a-105">**GetAttachmentResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a073a-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a073a-106">Attributes and elements</span></span>

<span data-ttu-id="a073a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a073a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a073a-108">属性</span><span class="sxs-lookup"><span data-stu-id="a073a-108">Attributes</span></span>

<span data-ttu-id="a073a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a073a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a073a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a073a-110">Child elements</span></span>

|<span data-ttu-id="a073a-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="a073a-111">**Element**</span></span>|<span data-ttu-id="a073a-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="a073a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a073a-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a073a-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="a073a-114">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a073a-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a073a-115">親要素</span><span class="sxs-lookup"><span data-stu-id="a073a-115">Parent elements</span></span>

<span data-ttu-id="a073a-116">なし。</span><span class="sxs-lookup"><span data-stu-id="a073a-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a073a-117">備考</span><span class="sxs-lookup"><span data-stu-id="a073a-117">Remarks</span></span>

<span data-ttu-id="a073a-118">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="a073a-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a073a-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="a073a-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a073a-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="a073a-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a073a-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a073a-121">Schema name</span></span>  <br/> |<span data-ttu-id="a073a-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="a073a-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a073a-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a073a-123">Validation file</span></span>  <br/> |<span data-ttu-id="a073a-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a073a-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a073a-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a073a-125">Can be empty</span></span>  <br/> |<span data-ttu-id="a073a-126">False</span><span class="sxs-lookup"><span data-stu-id="a073a-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a073a-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="a073a-127">See also</span></span>



[<span data-ttu-id="a073a-128">GetAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="a073a-128">GetAttachment operation</span></span>](getattachment-operation.md)
  
[<span data-ttu-id="a073a-129">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="a073a-129">GetAttachment</span></span>](getattachment.md)

