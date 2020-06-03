---
title: SubscribeResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SubscribeResponse
api_type:
- schema
ms.assetid: fd87e9b7-c231-44fa-9f5b-19ae96cda5cc
description: SubscribeResponse 要素は、Subscribe 要求に対する応答を定義します。
ms.openlocfilehash: 1f7079694c873aacbf44b1030e495cbe2f48d163
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530952"
---
# <a name="subscriberesponse"></a><span data-ttu-id="963a9-103">SubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="963a9-103">SubscribeResponse</span></span>

<span data-ttu-id="963a9-104">**SubscribeResponse**要素は、Subscribe 要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="963a9-104">The **SubscribeResponse** element defines a response to a Subscribe request.</span></span> 
  
[<span data-ttu-id="963a9-105">SubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="963a9-105">SubscribeResponse</span></span>](subscriberesponse.md)
  
```xml
<SubscribeResponse>
   <ResponseMessages/>
</SubscribeResponse>
```

 <span data-ttu-id="963a9-106">**電話機の種類**</span><span class="sxs-lookup"><span data-stu-id="963a9-106">**SubscribeResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="963a9-107">属性と要素</span><span class="sxs-lookup"><span data-stu-id="963a9-107">Attributes and elements</span></span>

<span data-ttu-id="963a9-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="963a9-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="963a9-109">属性</span><span class="sxs-lookup"><span data-stu-id="963a9-109">Attributes</span></span>

<span data-ttu-id="963a9-110">なし。</span><span class="sxs-lookup"><span data-stu-id="963a9-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="963a9-111">子要素</span><span class="sxs-lookup"><span data-stu-id="963a9-111">Child elements</span></span>

|<span data-ttu-id="963a9-112">**Element**</span><span class="sxs-lookup"><span data-stu-id="963a9-112">**Element**</span></span>|<span data-ttu-id="963a9-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="963a9-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="963a9-114">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="963a9-114">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="963a9-115">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="963a9-115">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="963a9-116">親要素</span><span class="sxs-lookup"><span data-stu-id="963a9-116">Parent elements</span></span>

<span data-ttu-id="963a9-117">なし。</span><span class="sxs-lookup"><span data-stu-id="963a9-117">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="963a9-118">注釈</span><span class="sxs-lookup"><span data-stu-id="963a9-118">Remarks</span></span>

<span data-ttu-id="963a9-119">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="963a9-119">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="963a9-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="963a9-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="963a9-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="963a9-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="963a9-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="963a9-122">Schema name</span></span>  <br/> |<span data-ttu-id="963a9-123">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="963a9-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="963a9-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="963a9-124">Validation file</span></span>  <br/> |<span data-ttu-id="963a9-125">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="963a9-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="963a9-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="963a9-126">Can be empty</span></span>  <br/> |<span data-ttu-id="963a9-127">正しい</span><span class="sxs-lookup"><span data-stu-id="963a9-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="963a9-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="963a9-128">See also</span></span>



[<span data-ttu-id="963a9-129">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="963a9-129">Subscribe operation</span></span>](subscribe-operation.md)

