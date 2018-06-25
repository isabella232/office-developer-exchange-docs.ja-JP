---
title: UpdateItemResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateItemResponse
api_type:
- schema
ms.assetid: 023b79b4-c675-4669-9112-d85499ec4fc4
description: UpdateItemResponse 要素は、UpdateItem 要求への応答を定義します。
ms.openlocfilehash: 12c1274fa500fe206381d7868393aaa08ca97d54
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839871"
---
# <a name="updateitemresponse"></a><span data-ttu-id="17dea-103">UpdateItemResponse</span><span class="sxs-lookup"><span data-stu-id="17dea-103">UpdateItemResponse</span></span>

<span data-ttu-id="17dea-104">**UpdateItemResponse**要素は、UpdateItem 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="17dea-104">The **UpdateItemResponse** element defines a response to an UpdateItem request.</span></span> 
  
```xml
<UpdateItemResponse>
   <ResponseMessages/>
</UpdateItemResponse>
```

 <span data-ttu-id="17dea-105">**UpdateItemResponseType**</span><span class="sxs-lookup"><span data-stu-id="17dea-105">**UpdateItemResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="17dea-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="17dea-106">Attributes and elements</span></span>

<span data-ttu-id="17dea-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="17dea-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="17dea-108">属性</span><span class="sxs-lookup"><span data-stu-id="17dea-108">Attributes</span></span>

<span data-ttu-id="17dea-109">なし。</span><span class="sxs-lookup"><span data-stu-id="17dea-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="17dea-110">子要素</span><span class="sxs-lookup"><span data-stu-id="17dea-110">Child elements</span></span>

|<span data-ttu-id="17dea-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="17dea-111">**Element**</span></span>|<span data-ttu-id="17dea-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="17dea-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="17dea-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="17dea-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="17dea-114">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="17dea-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="17dea-115">親要素</span><span class="sxs-lookup"><span data-stu-id="17dea-115">Parent elements</span></span>

<span data-ttu-id="17dea-116">なし。</span><span class="sxs-lookup"><span data-stu-id="17dea-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="17dea-117">備考</span><span class="sxs-lookup"><span data-stu-id="17dea-117">Remarks</span></span>

<span data-ttu-id="17dea-118">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="17dea-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="17dea-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="17dea-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="17dea-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="17dea-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="17dea-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="17dea-121">Schema name</span></span>  <br/> |<span data-ttu-id="17dea-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="17dea-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="17dea-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="17dea-123">Validation file</span></span>  <br/> |<span data-ttu-id="17dea-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="17dea-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="17dea-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="17dea-125">Can be empty</span></span>  <br/> |<span data-ttu-id="17dea-126">False</span><span class="sxs-lookup"><span data-stu-id="17dea-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="17dea-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="17dea-127">See also</span></span>



<span data-ttu-id="17dea-128">
  [UpdateItem 操作](updateitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="17dea-128">[UpdateItem operation](updateitem-operation.md)</span></span>
  
[<span data-ttu-id="17dea-129">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="17dea-129">UpdateItem</span></span>](updateitem.md)


- [<span data-ttu-id="17dea-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="17dea-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

