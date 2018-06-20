---
title: GetItemResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItemResponse
api_type:
- schema
ms.assetid: 8b66de1b-26a6-476c-9585-a96059125716
description: GetItemResponse 要素は、GetItem 要求への応答を定義します。
ms.openlocfilehash: 73805cf007a8d9d00d47b2b819935b5229c6e14d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760779"
---
# <a name="getitemresponse"></a><span data-ttu-id="86c9b-103">GetItemResponse</span><span class="sxs-lookup"><span data-stu-id="86c9b-103">GetItemResponse</span></span>

<span data-ttu-id="86c9b-104">**GetItemResponse**要素は、GetItem 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="86c9b-104">The **GetItemResponse** element defines a response to a GetItem request.</span></span> 
  
```xml
<GetItemResponse>
   <ResponseMessages/>
</GetItemResponse>
```

 <span data-ttu-id="86c9b-105">**GetItemResponseType**</span><span class="sxs-lookup"><span data-stu-id="86c9b-105">**GetItemResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="86c9b-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="86c9b-106">Attributes and elements</span></span>

<span data-ttu-id="86c9b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="86c9b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="86c9b-108">属性</span><span class="sxs-lookup"><span data-stu-id="86c9b-108">Attributes</span></span>

<span data-ttu-id="86c9b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="86c9b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="86c9b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="86c9b-110">Child elements</span></span>

|<span data-ttu-id="86c9b-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="86c9b-111">**Element**</span></span>|<span data-ttu-id="86c9b-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="86c9b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="86c9b-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="86c9b-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="86c9b-114">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="86c9b-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="86c9b-115">親要素</span><span class="sxs-lookup"><span data-stu-id="86c9b-115">Parent elements</span></span>

<span data-ttu-id="86c9b-116">なし。</span><span class="sxs-lookup"><span data-stu-id="86c9b-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="86c9b-117">備考</span><span class="sxs-lookup"><span data-stu-id="86c9b-117">Remarks</span></span>

<span data-ttu-id="86c9b-118">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="86c9b-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="86c9b-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="86c9b-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="86c9b-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="86c9b-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="86c9b-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="86c9b-121">Schema name</span></span>  <br/> |<span data-ttu-id="86c9b-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="86c9b-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="86c9b-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="86c9b-123">Validation file</span></span>  <br/> |<span data-ttu-id="86c9b-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="86c9b-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="86c9b-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="86c9b-125">Can be empty</span></span>  <br/> |<span data-ttu-id="86c9b-126">False</span><span class="sxs-lookup"><span data-stu-id="86c9b-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="86c9b-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="86c9b-127">See also</span></span>



[<span data-ttu-id="86c9b-128">GetItem</span><span class="sxs-lookup"><span data-stu-id="86c9b-128">GetItem</span></span>](getitem.md)
  
[<span data-ttu-id="86c9b-129">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="86c9b-129">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
  
<span data-ttu-id="86c9b-130">
  [GetItem 操作](getitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="86c9b-130">[GetItem operation](getitem-operation.md)</span></span>

