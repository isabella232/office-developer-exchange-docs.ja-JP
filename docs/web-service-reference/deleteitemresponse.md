---
title: DeleteItemResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteItemResponse
api_type:
- schema
ms.assetid: 86463d66-fe47-4a19-a81b-e24841e816ab
description: DeleteItemResponse 要素は、1 つの DeleteItem 要求への応答を定義します。
ms.openlocfilehash: 8a35033c744fbcb0829d2c79a8d79557f77137bb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759987"
---
# <a name="deleteitemresponse"></a><span data-ttu-id="dc073-103">DeleteItemResponse</span><span class="sxs-lookup"><span data-stu-id="dc073-103">DeleteItemResponse</span></span>

<span data-ttu-id="dc073-104">**DeleteItemResponse**要素は、1 つの DeleteItem 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="dc073-104">The **DeleteItemResponse** element defines a response to a single DeleteItem request.</span></span> 
  
```xml
<DeleteItemResponse>
   <ResponseMessages/>
</DeleteItemResponse>
```

 <span data-ttu-id="dc073-105">**DeleteItemResponseType**</span><span class="sxs-lookup"><span data-stu-id="dc073-105">**DeleteItemResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dc073-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="dc073-106">Attributes and elements</span></span>

<span data-ttu-id="dc073-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="dc073-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dc073-108">属性</span><span class="sxs-lookup"><span data-stu-id="dc073-108">Attributes</span></span>

<span data-ttu-id="dc073-109">なし。</span><span class="sxs-lookup"><span data-stu-id="dc073-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dc073-110">子要素</span><span class="sxs-lookup"><span data-stu-id="dc073-110">Child elements</span></span>

|<span data-ttu-id="dc073-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="dc073-111">**Element**</span></span>|<span data-ttu-id="dc073-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="dc073-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dc073-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="dc073-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="dc073-114">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="dc073-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dc073-115">親要素</span><span class="sxs-lookup"><span data-stu-id="dc073-115">Parent elements</span></span>

<span data-ttu-id="dc073-116">なし。</span><span class="sxs-lookup"><span data-stu-id="dc073-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="dc073-117">備考</span><span class="sxs-lookup"><span data-stu-id="dc073-117">Remarks</span></span>

<span data-ttu-id="dc073-118">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="dc073-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dc073-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="dc073-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dc073-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="dc073-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="dc073-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="dc073-121">Schema Name</span></span>  <br/> |<span data-ttu-id="dc073-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="dc073-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="dc073-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="dc073-123">Validation File</span></span>  <br/> |<span data-ttu-id="dc073-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="dc073-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dc073-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="dc073-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="dc073-126">False</span><span class="sxs-lookup"><span data-stu-id="dc073-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dc073-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="dc073-127">See also</span></span>

- [<span data-ttu-id="dc073-128">DeleteItem の操作</span><span class="sxs-lookup"><span data-stu-id="dc073-128">DeleteItem operation</span></span>](deleteitem-operation.md)  
- [<span data-ttu-id="dc073-129">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="dc073-129">DeleteItem</span></span>](deleteitem.md)
- [<span data-ttu-id="dc073-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="dc073-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

