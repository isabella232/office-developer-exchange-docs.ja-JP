---
title: SendItemResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendItemResponse
api_type:
- schema
ms.assetid: 26ac41c7-57d9-473e-ab7a-bae93e1d2aba
description: SendItemResponse 要素は、SendItem 要求への応答を定義します。
ms.openlocfilehash: 41f450e1d4c95f7ba389adcaa2ed7e18ea74d61c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/15/2018
ms.locfileid: "19833339"
---
# <a name="senditemresponse"></a><span data-ttu-id="a09cc-103">SendItemResponse</span><span class="sxs-lookup"><span data-stu-id="a09cc-103">SendItemResponse</span></span>

<span data-ttu-id="a09cc-104">**SendItemResponse**要素は、SendItem 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="a09cc-104">The **SendItemResponse** element defines a response to a SendItem request.</span></span> 
  
```xml
<SendItemResponse>
   <ResponseMessages/>
</SendItemResponse>
```

 <span data-ttu-id="a09cc-105">**SendItemResponseType**</span><span class="sxs-lookup"><span data-stu-id="a09cc-105">**SendItemResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a09cc-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a09cc-106">Attributes and elements</span></span>

<span data-ttu-id="a09cc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a09cc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a09cc-108">属性</span><span class="sxs-lookup"><span data-stu-id="a09cc-108">Attributes</span></span>

<span data-ttu-id="a09cc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a09cc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a09cc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a09cc-110">Child elements</span></span>

|<span data-ttu-id="a09cc-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="a09cc-111">**Element**</span></span>|<span data-ttu-id="a09cc-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="a09cc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a09cc-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a09cc-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="a09cc-114">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a09cc-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a09cc-115">親要素</span><span class="sxs-lookup"><span data-stu-id="a09cc-115">Parent elements</span></span>

<span data-ttu-id="a09cc-116">なし。</span><span class="sxs-lookup"><span data-stu-id="a09cc-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a09cc-117">解説</span><span class="sxs-lookup"><span data-stu-id="a09cc-117">Remarks</span></span>

<span data-ttu-id="a09cc-118">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="a09cc-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a09cc-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="a09cc-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a09cc-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="a09cc-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a09cc-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a09cc-121">Schema name</span></span>  <br/> |<span data-ttu-id="a09cc-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="a09cc-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a09cc-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a09cc-123">Validation file</span></span>  <br/> |<span data-ttu-id="a09cc-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a09cc-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a09cc-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a09cc-125">Can be empty</span></span>  <br/> |<span data-ttu-id="a09cc-126">False</span><span class="sxs-lookup"><span data-stu-id="a09cc-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a09cc-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="a09cc-127">See also</span></span>



<span data-ttu-id="a09cc-128">
  [SendItem 操作](senditem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="a09cc-128">[SendItem operation](senditem-operation.md)</span></span>
  
[<span data-ttu-id="a09cc-129">SendItem</span><span class="sxs-lookup"><span data-stu-id="a09cc-129">SendItem</span></span>](senditem.md)


- [<span data-ttu-id="a09cc-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="a09cc-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

