---
title: GetMailTipsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetMailTipsResponse
api_type:
- schema
ms.assetid: fe270e34-566e-4f9e-9e73-fbf38e06436d
description: GetMailTipsResponse 要素は、GetMailTips 操作の応答メッセージを表します。
ms.openlocfilehash: e7a18e8818761af931d32b26aeaf58a2853fa684
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760787"
---
# <a name="getmailtipsresponse"></a><span data-ttu-id="6eb73-103">GetMailTipsResponse</span><span class="sxs-lookup"><span data-stu-id="6eb73-103">GetMailTipsResponse</span></span>

<span data-ttu-id="6eb73-104">**GetMailTipsResponse**要素は、 [GetMailTips 操作](getmailtips-operation.md)の応答メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="6eb73-104">The **GetMailTipsResponse** element represents the response message for a [GetMailTips operation](getmailtips-operation.md).</span></span>
  
```XML
<GetMailTipsResponse>
   <ResponseMessages/>
</GetMailTipsResponse>
```

 <span data-ttu-id="6eb73-105">**GetMailTipsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="6eb73-105">**GetMailTipsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6eb73-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6eb73-106">Attributes and elements</span></span>

<span data-ttu-id="6eb73-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6eb73-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6eb73-108">属性</span><span class="sxs-lookup"><span data-stu-id="6eb73-108">Attributes</span></span>

<span data-ttu-id="6eb73-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6eb73-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6eb73-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6eb73-110">Child elements</span></span>

|<span data-ttu-id="6eb73-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="6eb73-111">**Element**</span></span>|<span data-ttu-id="6eb73-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="6eb73-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6eb73-113">ResponseMessages (ArrayOfMailTipsResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="6eb73-113">ResponseMessages (ArrayOfMailTipsResponseMessageType)</span></span>](responsemessages-arrayofmailtipsresponsemessagetype.md) <br/> |<span data-ttu-id="6eb73-114">メール ヒントの応答メッセージの一覧を表します。</span><span class="sxs-lookup"><span data-stu-id="6eb73-114">Represents a list of mail tips response messages.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6eb73-115">親要素</span><span class="sxs-lookup"><span data-stu-id="6eb73-115">Parent elements</span></span>

<span data-ttu-id="6eb73-116">なし。</span><span class="sxs-lookup"><span data-stu-id="6eb73-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="6eb73-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6eb73-117">Text value</span></span>

<span data-ttu-id="6eb73-118">なし。</span><span class="sxs-lookup"><span data-stu-id="6eb73-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6eb73-119">備考</span><span class="sxs-lookup"><span data-stu-id="6eb73-119">Remarks</span></span>

<span data-ttu-id="6eb73-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6eb73-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6eb73-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="6eb73-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6eb73-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="6eb73-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6eb73-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6eb73-123">Schema Name</span></span>  <br/> |<span data-ttu-id="6eb73-124">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="6eb73-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6eb73-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6eb73-125">Validation File</span></span>  <br/> |<span data-ttu-id="6eb73-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6eb73-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6eb73-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6eb73-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="6eb73-128">False</span><span class="sxs-lookup"><span data-stu-id="6eb73-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6eb73-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="6eb73-129">See also</span></span>



[<span data-ttu-id="6eb73-130">GetMailTips 操作</span><span class="sxs-lookup"><span data-stu-id="6eb73-130">GetMailTips operation</span></span>](getmailtips-operation.md)


- [<span data-ttu-id="6eb73-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="6eb73-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

