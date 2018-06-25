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
description: SubscribeResponse 要素は、Subscribe 要求への応答を定義します。
ms.openlocfilehash: 9c4fb0e9282acd2dfd8dcb66669815edcbd69ff2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833615"
---
# <a name="subscriberesponse"></a><span data-ttu-id="2603c-103">SubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="2603c-103">SubscribeResponse</span></span>

<span data-ttu-id="2603c-104">**SubscribeResponse**要素は、Subscribe 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="2603c-104">The **SubscribeResponse** element defines a response to a Subscribe request.</span></span> 
  
[<span data-ttu-id="2603c-105">SubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="2603c-105">SubscribeResponse</span></span>](subscriberesponse.md)
  
```xml
<SubscribeResponse>
   <ResponseMessages/>
</SubscribeResponse>
```

 <span data-ttu-id="2603c-106">**SubscribeResponseType**</span><span class="sxs-lookup"><span data-stu-id="2603c-106">**SubscribeResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2603c-107">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2603c-107">Attributes and elements</span></span>

<span data-ttu-id="2603c-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2603c-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2603c-109">属性</span><span class="sxs-lookup"><span data-stu-id="2603c-109">Attributes</span></span>

<span data-ttu-id="2603c-110">なし。</span><span class="sxs-lookup"><span data-stu-id="2603c-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2603c-111">子要素</span><span class="sxs-lookup"><span data-stu-id="2603c-111">Child elements</span></span>

|<span data-ttu-id="2603c-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="2603c-112">**Element**</span></span>|<span data-ttu-id="2603c-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="2603c-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2603c-114">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="2603c-114">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="2603c-115">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="2603c-115">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2603c-116">親要素</span><span class="sxs-lookup"><span data-stu-id="2603c-116">Parent elements</span></span>

<span data-ttu-id="2603c-117">なし。</span><span class="sxs-lookup"><span data-stu-id="2603c-117">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2603c-118">備考</span><span class="sxs-lookup"><span data-stu-id="2603c-118">Remarks</span></span>

<span data-ttu-id="2603c-119">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="2603c-119">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2603c-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="2603c-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2603c-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="2603c-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2603c-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2603c-122">Schema name</span></span>  <br/> |<span data-ttu-id="2603c-123">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="2603c-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2603c-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2603c-124">Validation file</span></span>  <br/> |<span data-ttu-id="2603c-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2603c-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2603c-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2603c-126">Can be empty</span></span>  <br/> |<span data-ttu-id="2603c-127">True</span><span class="sxs-lookup"><span data-stu-id="2603c-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2603c-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="2603c-128">See also</span></span>



[<span data-ttu-id="2603c-129">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="2603c-129">Subscribe operation</span></span>](subscribe-operation.md)

