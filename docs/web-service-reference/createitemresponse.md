---
title: CreateItemResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItemResponse
api_type:
- schema
ms.assetid: 742a46a0-2475-45a0-b44f-90639a3f5a43
description: CreateItemResponse 要素は、CreateItem 要求への応答を定義します。
ms.openlocfilehash: a05f222721e5b16695415e74a8e77e0fec495ef5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759841"
---
# <a name="createitemresponse"></a><span data-ttu-id="96d58-103">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="96d58-103">CreateItemResponse</span></span>

<span data-ttu-id="96d58-104">**CreateItemResponse**要素は、CreateItem 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="96d58-104">The **CreateItemResponse** element defines a response to a CreateItem request.</span></span> 
  
```xml
<CreateItemResponse>
   <ResponseMessages/>
</CreateItemResponse>
```

 <span data-ttu-id="96d58-105">**CreateItemResponseType**</span><span class="sxs-lookup"><span data-stu-id="96d58-105">**CreateItemResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="96d58-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="96d58-106">Attributes and elements</span></span>

<span data-ttu-id="96d58-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="96d58-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="96d58-108">属性</span><span class="sxs-lookup"><span data-stu-id="96d58-108">Attributes</span></span>

<span data-ttu-id="96d58-109">なし。</span><span class="sxs-lookup"><span data-stu-id="96d58-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="96d58-110">子要素</span><span class="sxs-lookup"><span data-stu-id="96d58-110">Child elements</span></span>

|<span data-ttu-id="96d58-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="96d58-111">**Element**</span></span>|<span data-ttu-id="96d58-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="96d58-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="96d58-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="96d58-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="96d58-114">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="96d58-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="96d58-115">親要素</span><span class="sxs-lookup"><span data-stu-id="96d58-115">Parent elements</span></span>

<span data-ttu-id="96d58-116">なし。</span><span class="sxs-lookup"><span data-stu-id="96d58-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="96d58-117">備考</span><span class="sxs-lookup"><span data-stu-id="96d58-117">Remarks</span></span>

<span data-ttu-id="96d58-118">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="96d58-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="96d58-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="96d58-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="96d58-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="96d58-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="96d58-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="96d58-121">Schema name</span></span>  <br/> |<span data-ttu-id="96d58-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="96d58-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="96d58-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="96d58-123">Validation file</span></span>  <br/> |<span data-ttu-id="96d58-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="96d58-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="96d58-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="96d58-125">Can be empty</span></span>  <br/> |<span data-ttu-id="96d58-126">False</span><span class="sxs-lookup"><span data-stu-id="96d58-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="96d58-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="96d58-127">See also</span></span>



<span data-ttu-id="96d58-128">
  [CreateItem 操作](createitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="96d58-128">[CreateItem operation](createitem-operation.md)</span></span>
  
[<span data-ttu-id="96d58-129">CreateItem</span><span class="sxs-lookup"><span data-stu-id="96d58-129">CreateItem</span></span>](createitem.md)


- [<span data-ttu-id="96d58-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="96d58-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

