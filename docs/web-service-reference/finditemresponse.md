---
title: FindItemResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindItemResponse
api_type:
- schema
ms.assetid: c8b316df-d4ab-49b8-96d4-8e9a016730ef
description: FindItemResponse 要素は、FindItem 要求への応答を定義します。
ms.openlocfilehash: f30aae5637a0c9d1105054a1185c32707820bd8e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760512"
---
# <a name="finditemresponse"></a><span data-ttu-id="5615d-103">FindItemResponse</span><span class="sxs-lookup"><span data-stu-id="5615d-103">FindItemResponse</span></span>

<span data-ttu-id="5615d-104">**FindItemResponse**要素は、FindItem 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="5615d-104">The **FindItemResponse** element defines a response to a FindItem request.</span></span> 
  
[<span data-ttu-id="5615d-105">FindItemResponse</span><span class="sxs-lookup"><span data-stu-id="5615d-105">FindItemResponse</span></span>](finditemresponse.md)
  
```xml
<FindItemResponse>
   <ResponseMessages/>
</FindItemResponse>
```

 <span data-ttu-id="5615d-106">**FindItemResponseType**</span><span class="sxs-lookup"><span data-stu-id="5615d-106">**FindItemResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5615d-107">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5615d-107">Attributes and elements</span></span>

<span data-ttu-id="5615d-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5615d-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5615d-109">属性</span><span class="sxs-lookup"><span data-stu-id="5615d-109">Attributes</span></span>

<span data-ttu-id="5615d-110">なし。</span><span class="sxs-lookup"><span data-stu-id="5615d-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5615d-111">子要素</span><span class="sxs-lookup"><span data-stu-id="5615d-111">Child elements</span></span>

|<span data-ttu-id="5615d-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="5615d-112">**Element**</span></span>|<span data-ttu-id="5615d-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="5615d-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5615d-114">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5615d-114">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="5615d-115">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5615d-115">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5615d-116">親要素</span><span class="sxs-lookup"><span data-stu-id="5615d-116">Parent elements</span></span>

<span data-ttu-id="5615d-117">なし。</span><span class="sxs-lookup"><span data-stu-id="5615d-117">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5615d-118">備考</span><span class="sxs-lookup"><span data-stu-id="5615d-118">Remarks</span></span>

<span data-ttu-id="5615d-119">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="5615d-119">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5615d-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="5615d-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5615d-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="5615d-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5615d-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5615d-122">Schema name</span></span>  <br/> |<span data-ttu-id="5615d-123">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="5615d-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5615d-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5615d-124">Validation file</span></span>  <br/> |<span data-ttu-id="5615d-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5615d-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5615d-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="5615d-126">Can be empty</span></span>  <br/> |<span data-ttu-id="5615d-127">False</span><span class="sxs-lookup"><span data-stu-id="5615d-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5615d-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="5615d-128">See also</span></span>



<span data-ttu-id="5615d-129">
  [FindItem 操作](finditem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="5615d-129">[FindItem operation](finditem-operation.md)</span></span>
  
[<span data-ttu-id="5615d-130">FindItem</span><span class="sxs-lookup"><span data-stu-id="5615d-130">FindItem</span></span>](finditem.md)


[<span data-ttu-id="5615d-131">項目を検索します。</span><span class="sxs-lookup"><span data-stu-id="5615d-131">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

